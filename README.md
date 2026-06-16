# GLPI-11-NGINX-MySQL-Zabbix7-Integration

## 📋 Visão Geral

Este projeto documenta a instalação e configuração integrada de:
- GLPI (Helpdesk)
- Zabbix 7.2 (Monitoramento)
- Grafana (Dashboards)
- NGINX + MySQL

---

## 📚 Documentação Completa

| Componente | Documentação | Status |
|------------|--------------|--------|
| 🖥️ **GLPI** | [glpi.md](glpi.md) | ✅ Completo |
| 📊 **Zabbix 7.2** | [zabbix.md](zabbix.md) | ✅ Completo |
| 📈 **Grafana** | [grafana.md](grafana.md) | ✅ Completo |
| 🔗 **Integração** | [integracao.md](integracao.md) | ✅ Completo |

---

## 🚀 Cenários Utilizados

### 1. GLPI
- **Sistema:** Ubuntu Server 26.04
- **FQDN:** glpi.connect.local
- **Stack:** NGINX + MySQL + PHP
- 📄 [Guia de Instalação do GLPI →](glpi.md)

### 2. Zabbix + Grafana
- **Sistema:** Ubuntu Server 26.04
- **FQDN:** zabbix.connect.local e grafana.connect.local
- **Stack:** NGINX + MySQL + PHP
- 📄 [Guia de Instalação do Zabbix →](zabbix.md)
- 📄 [Guia de Configuração do Grafana →](grafana.md)

---

## 🔗 Integração

- 📄 [Como integrar Zabbix com GLPI](integracao.md)

---