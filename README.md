# qwenchana






python -c "
import json
path = '~/.cache/huggingface/hub/models--Qwen--Qwen3-0.6B/blobs/f47f71177f32bcd101b7573ec9171e6a57f4f4d31148d38e382306f42996874b'
with open(path, 'rb') as f:
    n = int.from_bytes(f.read(8), 'little')
    print(json.dumps(json.loads(f.read(n)), indent=2))
" > qwen3-0.6B.json
