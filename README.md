# AI-Powered Early Wildfire Detection System

Final project for the Building AI course

## Summary
An AI system that uses satellite imagery and weather data to detect wildfires hours earlier than current methods, giving firefighters and communities precious extra time to respond and reduce damage.

## Background
Wildfires are increasing due to climate change. Millions of hectares burn every year in Europe, Australia, Canada and the Amazon. Many fires start in remote areas and are only noticed when they are already large. Early detection can save lives, homes and forests. I live in a high-risk area and have seen friends lose their houses — this is personal.

## How is it used?
- Fire departments receive automatic alerts with GPS coordinates and confidence level
- Citizens in high-risk zones get SMS/push notifications
- A public real-time map shows current risks (like NASA FIRMS but faster)
Users: firefighters, forest services, local governments and residents.

## Data sources and AI methods
| Data                  | Source                     | Frequency    |
|-----------------------|----------------------------|--------------|
| Thermal hotspots      | NASA FIRMS (MODIS + VIIRS) | every 3–6 h  |
| High-resolution images| Sentinel-2                 | every 5 days |
| Weather data          | ECMWF / OpenWeatherMap     | hourly       |

Planned AI techniques:
- CNN / Vision Transformer for smoke & heat detection
- Time-series LSTM for anomaly detection
- Ensemble model + weather risk index

## Challenges
- Clouds can hide fires
- False positives from factories or controlled burns
- Small underground fires are hard to detect from space
- Need fair distribution of alerts (rich vs. poor regions)

## What next?
- Build prototype for my country first
- Partner with local fire service
- Add cheap IoT ground sensors and drone verification
- Expand to illegal logging detection

## Acknowledgments
- NASA FIRMS, ESA Copernicus, ECMWF open data
- Inspiration from fast.ai courses and the Building AI course
- All code will be based on open-source PyTorch/fast.ai libraries

Building AI course project – 2025
Update README.md
