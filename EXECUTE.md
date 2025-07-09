## 🚀 Como Executar os Testes de Performance Localmente

### 📌 Requisitos

- Java 23+  
- [Apache JMeter v5.6.3](https://jmeter.apache.org/)  
- BlazeMeter Plugin v6.6.7

---

### 🔹 1. Clonar o Repositório

```bash
git clone https://github.com/bibiellabraz/jmeter-performance-tests.git
cd jmeter-performance-tests


🔹 2. Executar Testes de Carga
➤ Teste com 10 usuários

jmeter -n \
  -t load-tests/Plans/TestPlan10.jmx \
  -l results/load_10.jtl \
  -e -o load-tests/Report/10-users


➤ Teste com 30 usuários

jmeter -n \
  -t load-tests/Plans/TestPlan30.jmx \
  -l results/load_30.jtl \
  -e -o load-tests/Report/30-users


🔹 3. Executar Testes de Estresse

➤ Teste com 100 usuários (simulação progressiva)

jmeter -n \
  -t stress-tests/Plans/TestPlan100.jmx \
  -l results/stress_100.jtl \
  -e -o stress-tests/Report\ 1

Obs: Você pode salvar múltiplos relatórios separadamente como Report 2, Report 3 etc., alterando o caminho de saída (-o).
