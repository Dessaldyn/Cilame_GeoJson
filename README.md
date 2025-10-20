# Cilame_GeoJson

## Dokumentasi Data Geospasial
Data ini berisi jalur jalan (LineString) yang telah diubah dari format GeoJSON FeatureCollection menjadi array dokumen JSON individual, siap untuk di-insert ke MongoDB.

## Format Data & Struktur MongoDB
Setiap objek dalam array merepresentasikan satu dokumen di koleksi Anda dan mengikuti standar GeoJSON untuk kolom geometry.

```
{
  "name": "Nama Lokasi/Jalan",
  "geometry": {
    "type": "LineString", // atau "Point", "Polygon"
    "coordinates": [
      // array koordinat [longitude, latitude]
    ]
  }
}
```