# Nöroform Teknik Referansı

Ana teknik plan [`../PLAN.md`](../PLAN.md) dosyasındadır. Landing revizyonundan itibaren aşağıdaki kararlar geçerlidir:

## Tasarım sistemi güncellemesi

Landing sayfası WebGL/Canvas kullanmaz. Dört bilişsel alan, özgün SVG tabanlı Zihin Dostları maskotlarıyla temsil edilir. Başlık fontu Nunito 800, gövde fontu Inter’dir. Maskotlar CSS/SVG gradient, yumuşak gölge, idle zıplama, göz kırpma, requestAnimationFrame göz takibi ve reduced-motion desteği kullanır.

3D/WebGL yalnızca Yankı Küreleri, Döndür, Kule oyunları ve Zihin Heykeli profil deneyimlerinde kullanılacaktır. `three`, `@react-three/fiber` ve `@react-three/drei` bağımlılıkları sonraki aşamalar için korunur.

## Landing güncellemesi

Hero’da solda mevcut Türkçe başlık, alt başlık ve CTA’lar; sağda pastel, yuvarlak köşeli 2D sahne kartı bulunur. Dört maskot hover’da mutlu ifadeye ve “Oyna” balonuna geçer; tıklama ilgili `/oyun/:gameId` rotasına gider. Mobilde maskotlar başlığın altında yan yana görünür. Dürüst bilim çubuklarının değerleri `0.88`, `0.27` ve `0.12` olarak kalır.
