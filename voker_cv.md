# Vojtěch Krupička

+420 721 749 393 · voker@email.cz · linkedin.com/in/vojtech-krupicka · github.com/vojtech-krupicka · Brno, Czech Republic

**Senior Software Engineer / Backend Developer**

Software Engineer / Backend Developer with 17 years of industry experience, including nearly 14 years as a member of the development team for Seznam.cz's Mapy.com (formerly Mapy.cz) map application. Achievements, among other projects, included working with large volumes of geospatial data (using PostGIS, GDAL, OGR, ...), contributing to the development of software for the Panorama Car (Python, C++), developing and maintaining a bug-reporting system for routing end-user feedback to the helpdesk (PHP, Python), building a platform for managing, validating, and serving user-uploaded media handling hundreds of requests/second (Python, Flask, RPC, PostgreSQL, CDN), and developing automated pipelines based on machine learning and AI/LLM models (Python, TensorFlow, ONNX, PyTorch, NumPy). This work was planned using Agile & Scrum and relied on CI/CD for deploying components across multiple environments using GitLab CI, Docker and Kubernetes. Earlier career experience includes founding development work on the Smartsupp instant-messaging application and a CMS for the Sportisimo.cz e-commerce platform.

---

## EXPERIENCE

### Seznam.cz a.s., Brno — *Software Engineer (Mapy.cz / Mapy.com)* — Dec. 2012 – Aug. 2026

**User Media Platform — Solo Developer (2018 – 2026)**

- Inherited, rewrote, and optimized the media backend service for storing, handling, and serving Mapy.com's geo-referenced media to web and mobile apps — migrated largely solo from Python2/RPC to a Python3/Flask/Pydantic architecture, using PostgreSQL/CDN for storing 20M+ media files and metadata and handling hundreds of requests/second (with response times reduced from 300ms to 50ms through the rewrite for key endpoints) (2019-2026)
- Integrated ML-based (neural networks) automatic photo validation/moderation using TensorFlow, ONNX, PyTorch, NumPy, and scikit-image (2018-2026)
- Collaborated on continuous migration of media metadata from other Seznam.cz's services to Mapy.com's media infrastructure using Kafka messaging (2025-2026)

**Panorama Imaging System (2014 – 2018)**

- Contributed to the development of software and the panorama photography pipeline for the Panorama Car with a custom-made camera rig, including the car-crew tablet application, used to navigate the planned route and operate the camera rig from the car seat
- Co-rewrote (2017, 2-person team) most of the panorama photography pipeline to suit a new data supplier, processing terabytes of imagery data
- Built first version of the panorama-photography serving platform (2014)

**Geospatial Data Processing — DEMs, Elevation & Contours (2015 – 2019)**

- Processed global digital elevation models (DEMs, 200GB+ source data), wrote scripts for generating better hillshades and contours lines
- Built a pipeline generating and storing 15M+ contour lines (1.5TB) across the globe using GDAL, OGR, and PostGIS
- Built a backend service for on-demand computing of elevation profiles across multi-point routes from multiple DEM sources
- Collaborated with the Teiresias Centre (Masaryk University) on Mapnik styles and street abbreviations for tactile maps (Haptické Mapy)

**Internal Tools & Emerging Tech**

- Built a pipeline for automated text translations from multiple sources via AI/LLM models (2025 – 2026)
- Built a Kafka consumer pipeline for transactional email notifications (2025)
- Solo developer and maintainer of the Mapy.com end-user bug tracking system using external MantisBT — including new plugins (PHP Full-stack), and components connecting frontends with MantisBT (Python, PostgreSQL) for the entire Mapy.com issue-reporting system — connecting the helpdesk to end-user feedback loops with a Mantis BT 1.3 → 2.x migration and MySQL → PostgreSQL migration (2014 – 2026)
- Contributed to the distributed rendering system of map tiles from multiple data sources (PostgreSQL, shapefiles, DEMs, mapnik styles) with distribution of final data (500GB+ per version) to production servers (2013); then co-rewrote it in 2017 (as a part of 4-person team), which reduced map tiles update time from weeks to days

**DevOps & Miscellaneous**

- Formerly using Debian packages for deployment components to production; later moved to deploying Docker images to Kubernetes via CI pipelines (GitLab CI, Jenkins) across dev/staging/production environments and using Prometheus monitoring with Grafana dashboards
- Using Agile & Scrum for planning (YouTrack, Trello)

### Prezentuji.cz, Brno — *Full-stack Web Developer / Smartsupp Co-Founder* (2011 – 2012)

- Built tailor-made web applications (e-shops, blogs, presentation sites) and converted Photoshop designs into HTML/CSS templates (using PHP, MySQL, JavaScript, HTML, and CSS) (2011 – mid 2012)
- Co-founded Smartsupp, an early-stage startup building embeded live web instant-messaging software for website owners and support staff (a concept rare in 2012, now an industry standard), co-created the architecture for the first version of the system; contributed mainly to backend/server-side development in C++, including client/server communication (Jun – Nov 2012)

### Symedia s.r.o., Hlinsko — *Full-stack Web Developer* (2009 – 2011)

- Joined as part of the founding team building Sportisimo.cz's e-commerce platform from scratch (Symedia was later acquired by Sportisimo — a major Czech sports retailer); contributed as a Full-stack developer across PHP, MySQL, JavaScript (jQuery), HTML, and CSS
- Designed and built a custom CMS used by Sportisimo staff to create the e-shop's public-facing pages, including custom widgets (galleries, carousels, polls, menus, and more) for brand and product content — the system remained in production for nearly a decade

---

## TECHNICAL SKILLS

- **Languages:** Python (3.10+, daily use), PHP 7.4, C++17, C#/.NET (Unity), Web (HTML, CSS, JavaScript), Go/Lua (basics)
- **Databases/Storage:** PostgreSQL (daily), MySQL, ETCD, MongoDB and Redis (basics)
- **Infrastructure:** Git, CI/CD (GitLab CI, Jenkins), Docker, Kubernetes, Kafka, Prometheus, Grafana, Apache/nginx configuration
- **ML/AI:** TensorFlow, ONNX, PyTorch, NumPy, scikit-image (applied); working knowledge of LLM-based tooling/prompting
- **Frameworks:** Flask, uWSGI, poetry, Jinja, FastAPI, Nette, Boost, wxWidgets, Qt
- **Geospatial Tools:** PostGIS, GDAL, OGR, QGIS, Mapnik
- **Operating Systems:** Debian Linux, Windows
- **Methodologies:** Agile & Scrum (YouTrack, Trello)

---

## EDUCATION

**Brno University of Technology** — Faculty of Information Technology

- M.Sc., Computer Graphics and Multimedia (2009–2012) — Thesis: *Frameless Rendering* (C++, OpenGL)
- B.Sc., Information Technology (2006–2009) — Thesis: *Education Computer Program for Demonstration of 2D Shapes Rasterization* (C++, wxWidgets)

---

## LANGUAGES

- Czech — Native
- English — Reading/Listening: Advanced · Writing/Speaking: Intermediate

---

## HOBBIES

Programming and technologies, game development (Unity/C#), game level design (Source engine), digital art (Krita), computer games, outdoor activities
