# 🎨 Gerador de padrões artísticos abstratos utilizando Deep Convolutional Generative Adversarial Network (DCGAN)

Este projeto explora o uso de Deep Convolutional Generative Adversarial Networks (DCGANs) para gerar imagens sintéticas de arte abstrata. O modelo foi implementado como parte de um trabalho acadêmico para a disciplina de Redes Neurais.

---

## ✨ Resultados

O modelo foi capaz de aprender padrões visuais a partir de um conjunto de imagens de arte abstrata, gerando imagens criativas e diversas. Embora algumas imagens apresentem artefatos comuns em GANs, muitas exibem elementos visualmente convincentes e esteticamente interessantes.

---

## 🧠 Arquitetura DCGAN

- **Gerador**: camadas densas e convolucionais transpostas com `BatchNorm` e `LeakyReLU`. A ativação final é `tanh`.
- **Discriminador**: camadas convolucionais com `SpectralNorm`, `LeakyReLU` e `Dropout`, finalizando com uma camada densa.
- **Função de perda**: Binary Cross-Entropy com *label smoothing*.
- **Otimizador**: Adam (lr = 0.0002, beta1 = 0.5).

---

## 📊 Comparação com StyleGAN2-ADA

Foi realizada uma breve comparação com a arquitetura [StyleGAN2-ADA](https://github.com/NVlabs/stylegan2-ada-pytorch), mais recente e avançada. O StyleGAN2-ADA apresentou desempenho significativamente superior em benchmarks como o CIFAR-10, alcançando valores de FID muito menores.

📊 Fonte: [paperswithcode.com/sota/image-generation-on-cifar-10](https://paperswithcode.com/sota/image-generation-on-cifar-10)

Apesar dos bons resultados obtidos com a DCGAN no contexto deste projeto, arquiteturas modernas como a StyleGAN2-ADA representam o estado da arte e podem ser exploradas em trabalhos futuros para gerar imagens com maior qualidade e realismo.

---

## 👥 Autoria

- Maria Lago — [@marialago](https://github.com/marialago)
- Victor Hermes - [@VictorHAS](https://github.com/VictorHAS)

---

## 📜 Licença

Este projeto está licenciado sob a Licença MIT.  
Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
