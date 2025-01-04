// HTML elemanlarını seçme
const oyunAlani = document.getElementById('oyunAlani');
const kare = document.getElementById('kare');
const puanGosterge = document.getElementById('puanGosterge');
const oyunBittiMesaji = document.getElementById('oyunBitti');
const tiklamaSesi = document.getElementById('tiklamaSesi');
const oyunBittiSesi = document.getElementById('oyunBittiSesi');

// Değişken tanımları
let puan = 0; // Kullanıcının puanı
let kalanSure = 30; // Oyun süresi (saniye)
let kareBoyutu = 50; // Karenin başlangıç boyutu (piksel)
let zorlukSeviyesi = 1; // Oyunun zorluk seviyesi

// Kareyi rastgele bir konuma yerleştiren fonksiyon
function kareyiHareketEttir() {
    // Oyun alanının boyutlarına göre maksimum x ve y koordinatlarını belirle
    const maxX = oyunAlani.offsetWidth - kare.offsetWidth;
    const maxY = oyunAlani.offsetHeight - kare.offsetHeight;

    // Rastgele bir x ve y koordinatı oluştur
    const rastgeleX = Math.floor(Math.random() * maxX);
    const rastgeleY = Math.floor(Math.random() * maxY);

    // Karenin yeni pozisyonunu ayarla
    kare.style.left = `${rastgeleX}px`;
    kare.style.top = `${rastgeleY}px`;
}

// Kullanıcı kareye tıkladığında puan artıran fonksiyon
kare.addEventListener('click', () => {
    puan++; // Puanı bir artır
    puanGosterge.textContent = `Puan: ${puan}`; // Puanı ekranda güncelle
    tiklamaSesi.play(); // Tıklama sesini oynat
    kareyiHareketEttir(); // Kareyi yeni bir konuma taşı

    // Puan her 5 arttığında zorluk seviyesi yükselsin
    if (puan % 5 === 0) {
        zorlukSeviyesi++;
        kareBoyutu = Math.max(20, kareBoyutu - 5); // Karenin boyutunu küçült (en az 20 piksel)
        kare.style.width = `${kareBoyutu}px`;
        kare.style.height = `${kareBoyutu}px`;
    }
});

// Fare kareye yaklaştığında kaçar
kare.addEventListener('mouseover', kareyiHareketEttir);

// Oyunun süresini geri saydıran fonksiyon
function zamanlayiciyiBaslat() {
    const zamanlayici = setInterval(() => {
        kalanSure--; // Süreyi bir azalt
        if (kalanSure === 0) {
            clearInterval(zamanlayici); // Zamanlayıcıyı durdur
            oyunBitir(); // Oyunu bitir
        }
    }, 1000); // Her saniye çalışır
}

// Oyun bittiğinde yapılacaklar
function oyunBitir() {
    kare.style.display = 'none'; // Kareyi gizle
    oyunBittiMesaji.style.display = 'block'; // "Oyun Bitti" mesajını göster
    oyunBittiMesaji.textContent = `Oyun Bitti! Skorunuz: ${puan}`;
    oyunBittiSesi.play(); // Oyun bitti sesini çal
}

// Mobil cihazlarda dokunma desteği
kare.addEventListener('touchstart', (event) => {
    event.preventDefault(); // Dokunma olayının varsayılan davranışını engelle
    puan++;
    puanGosterge.textContent = `Puan: ${puan}`;
    tiklamaSesi.play();
    kareyiHareketEttir();
});

// Oyunu başlatan kodlar
kareyiHareketEttir(); // Kareyi başlangıçta rastgele bir yere koy
zamanlayiciyiBaslat(); // Süreyi başlat