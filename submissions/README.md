# Submissions

| model | model repo | results | engine / code | hardware | settings |
|---|---|---|---|---|---|
| NTele-Hybrid-27B-v1 | [ZTE-AIM/NTele-Hybrid-27B-v1](https://huggingface.co/ZTE-AIM/NTele-Hybrid-27B-v1) @ b811b2c | [runs/NTele-Hybrid-27B-v1-decision-index-results](https://huggingface.co/datasets/ZTE-AIM/NTele-Hybrid-27B-v1-decision-index-results/tree/main/runs/NTele-Hybrid-27B-v1)) (public 0.3: 63.30, complete)| kit 0.3 (f8552a1), `http` engines against `ntele-decide serve` from [NTele-decisions](https://github.com/Jiangxg/NTele-decisions) @ 733529d (`/v1/systemone`), SGLang >=0.5.20 | 8x H800 80 GB, one server per GPU; | BF16; one forward pass per question, option-letter read-out, nothing generated;262,144-token context; 0 errors, 0 unsupported |
