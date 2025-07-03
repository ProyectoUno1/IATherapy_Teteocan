asistente_emocional/
├── android/                          ← Proyecto nativo Android
├── ios/                              ← Proyecto nativo iOS
├── assets/                           ← Imágenes, íconos, sonidos, etc.
│   ├── images/
│   └── icons/
├── lib/                              ← Carpeta principal del código Flutter
│   ├── main.dart                     ← 📌 Archivo inicial de la app
│   ├── app.dart                      ← Configuración global (tema, rutas)
│
│   ├── core/                         ← Servicios compartidos
│   │   ├── constants/                ← Colores, textos globales, rutas
│   │   ├── utils/                    ← Validaciones, helpers
│   │   └── services/                 ← APIs externas, IA, emails, etc.
│
│   ├── data/                         ← 📦 Lógica de datos (como backend interno)
│   │   ├── models/                   ← Clases como Usuario, Mensaje, Psicólogo
│   │   ├── datasources/             ← Fuente de datos (local/remota)
│   │   │   ├── local/               ← Guardado en dispositivo
│   │   │   └── remote/              ← API, Firebase, etc.
│   │   └── repositories/            ← Lógica que une la fuente de datos con la app
│
│   ├── features/                     ← Pantallas divididas por funcionalidad
│   │   ├── auth/                    ← Login, registro
│   │   ├── home/                    ← Pantalla principal
│   │   ├── chat/                    ← Chat con IA o humano
│   │   └── psicologos/              ← Buscar y agendar profesionales
│
│   └── shared/
│       ├── widgets/                  ← Botones, cards, etc. reutilizables
│       └── theme/                    ← Temas personalizados (colores, fuentes)
├── pubspec.yaml                      ← Configuración del proyecto
└── README.md                         ← Descripción general