## ❓ Info

A implementation that modify the script.py to scripto.py.

Forked from roboflow/supervision.

This modified script can count, track, annotate, classify, and distinguish different classes of vehicles.


[https://github.com/hugoles/supervision/edit/develop/examples/traffic_analysis/output_result_multiples_vehicles.mov](https://github.com/hugoles/supervision/assets/67278688/3eb27b9d-7bc3-4477-9da9-2926fcd37c78)

## 💻 install





- clone repository and navigate to example directory

    ```bash
    git clone https://github.com/hugoles/supervision.git
    cd supervision/examples/traffic_analysis
    ```

- setup python environment and activate it [optional]

    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```

- install required dependencies

    ```bash
    pip install -r requirements.txt
    ```

- download `model4.pt` and `output.mov` files

    ```bash
    ./setup.sh
    ```

## ⚙️ run

```bash
python scripto.py \
--source_weights_path data/model4.pt \
--source_video_path data/output.mov \
--confidence_threshold 0.3 \
--iou_threshold 0.5 \
--target_video_path data/output_result.mov
```
