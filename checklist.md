# Roadmap de Expansão Científica - ReactiveCosmoMapper 🚀

> **Objetivo:** Estressar o modelo de Gravidade Reativa em regimes onde a Matéria Escura (CDM) enfrenta tensões teóricas ou observacionais.

## 1. Teste de Lentes Gravitacionais (Weak Lensing) 👁️
- [x] **Implementar `src/lensing_projector.py`**:
    - [x] Criar classe `LensingProjector` para calcular potencial gravitacional ($\Phi$) no grid 3D.
    - [x] Mapa de Convergência gerado e validado visualmente (`Validation/lensing_prediction_map.png`).

## 2. A Crise das Galáxias Primitivas (JWST) ⏳
- [x] **Implementar `src/early_universe.py`**:
    - [x] Simulação de Colapso Primordial com $a_0(z)$ dinâmico.
    - [x] Gráfico comprova formação acelerada (`Validation/jwst_collapse_comparison.png`).

## 3. Estatística de Vazios (Cosmic Voids) 🕳️
- [x] **Implementar `src/void_scanner.py`**:
    - [x] Algoritmo Spherical Underdensity (Stochastic).
    - [x] Histograma de Tamanho de Vazios gerado (`Validation/void_size_distribution.png`).
    - [x] Resultado: Média de 740 Mpc (Grandes Voids = Assinatura da Repulsão Entrópica).

## 4. O Problema das Galáxias Satélites (Plane of Satellites) 🛸
- [x] **Simulação Local**:
    - [x] Carregar dados de galáxias satélites da Via Láctea/Andrômeda.
    - [x] Simular dinâmica vetorial considerando assimetrias do ambiente.
    - [x] Verificar estabilidade de órbitas planares.

## 5. Visualização (Video Studio) 🎬
- [x] **Galactic Dynamics**: `videos/galactic_dynamics.mp4`.
- [x] **Satellite Plane**: `videos/satellite_plane.mp4`.
- [x] **Early Universe**: `videos/early_collapse.mp4`.
- [x] **Lensing Scan**: `videos/lensing_scan.mp4`.
- [x] **Cosmic Web**: `videos/cosmic_web_flythrough.mp4`.

---

# Fase 2: Hard Science ⚛️

## 6. Dinâmica de Fusões (Mergers) 💥
**Hipótese:** A ausência de halos de DM reduz o atrito dinâmico, permitindo "flybys" mais limpos.
- [x] **Simulação de Colisão**:
    - [x] Implementar `src/merger_dynamics.py` (Dois discos colidindo).
    - [x] Comparar tempo de fusão com predições LCDM.
    - [x] Gerar vídeo `videos/galaxy_merger.mp4`.

## 7. O Batalha do CMB (Background) 🌌
**Hipótese:** $a_0(z)$ mimetiza a profundidade de poço gravitacional da DM no plasma primordial.
- [x] **Solver de Espectro de Potência**:
    - [x] Implementar oscilador de fluido bárion-fóton com kernel reativo.
    - [x] Verificar amplitude do terceiro pico acústico.
