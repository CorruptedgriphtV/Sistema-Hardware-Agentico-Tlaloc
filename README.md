# Sistema Hardware Agentico Tlaloc

Sistema de microclimas Mexicano de Precisión - Framework agrícola automatizado de Hardware in the Loop.

## Arquitectura Dual-Brain

- **MPU (Qualcomm Dragonwing - Linux Debian)**: Modelos LLM locales (Qwen 2.5 / LLaMA) + Ecosistema de agentes en Python
- **MCU (STM32 - Tiempo Real)**: Maestro I2C, comunicación RPC/Serial con MPU
- **Nodos (ATmega 328p)**: Esclavos I2C - Control de bombas, luces y lectura de sensores

## Agentes de IA

- **Donai**: Interfaz de usuario (NLP)
- **Tloque**: Orquestador lógico y tomador de decisiones agronómicas
- **Nuu**: Sistema de Visión Computacional (análisis foliar y estrés térmico)
- **Kanda**: Ejecutor de hardware (traductor JSON �� comandos serial/I2C)
