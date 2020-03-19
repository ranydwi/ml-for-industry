# Retail



## Customer Segmentation

### Background

FMCG (Fast Moving Consumer Goods) adalah produk-produk yang sifatnya cepat habis yang biasanya terdiri dari kebutuhan sehari-hari, sehingga dapat terjual dalam waktu singkat dan biaya yang relatif rendah. Suatu perusahaan FMCG mendistribusikan penjualannya ke berbagai macam sektor seperti hotel, restoran, kafe, dan semua macam outlet retail. Bagian CRM (Customer Relationship Management) mengumpulkan transaksi penjualan satu tahun terakhir untuk setiap kategori produk. Perusahaan ingin membuat model machine learning yang secara otomatis dapat mengkategorikan customer mereka menjadi dua kelas yaitu, horeca (Hotel, Restaurant, and Cafe) dan
retail industry.

### Expected Outcome

Harapannya setelah mempunyai model machine learning, pihak CRM dapat melakukan prediksi mengenai customer yang membeli product mereka berasal dari industry mana yang dilihat dari transaksi setiap customer untuk setiap kategori.

### Recommendation


```r
data.frame(
  "Model" = rep("KNN", 4),
  "Evaluation" = c("Accuracy", "Specificity", "Precision", "Recall")  ,
  "Estimate" = c(0.920, 0.898, 0.823, 0.965)
)
```

```
#>   Model  Evaluation Estimate
#> 1   KNN    Accuracy    0.920
#> 2   KNN Specificity    0.898
#> 3   KNN   Precision    0.823
#> 4   KNN      Recall    0.965
```


Perfomance model yang diperoleh sudah cukup baik untuk mengkategorikan customer berasal dari kelas horeca atau retail. Langkah selanjutnya, setelah mengetahui industry dari customer tersebut pihak perusahaan dapat mengamati perilaku customer tersebut cenderung lebih banyak membeli produk pada kategori apa dan dapat dijadikan pertimbangan untuk memberikan promosi yang sesuai kebutuhan customer.