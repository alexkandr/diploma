- IR techniques - information retrieval?
- filtered back projection - что это?
Текущие бенчмарки: RMSE, SSIM, PSNR (peak signal to noise ratio )
Лучшие бенчмарки: VIF (variance inflation factor) и [human ] Reader studies
Подготовка данных:
- по 50 сканов живота, груди и головы с стандартным уровнем облучения
- симулированные реконструкции для 25% облучения для живота и головы, 10% для груди
- каждый отдел раздён на 70/20/10
- каждый сет отнормирован на m/v = 0/1
// Нормализация может быть гипермараметром
код для повтора разделения представлен
Алгоритмы:
- CNN-10
- RED-CNN
- ResNet
- WGAN-VGG
- DU-GAN
- QAE
- TransCT
- Bilateral
обучение по ssim
evaluation по ssim, psnr, vif - более высокая корреляция с human reader

результаты:
все алгоритмы сходятся до 50 итераций
RED-CNN лучше всего в общем случае
ResNet лучше для груди