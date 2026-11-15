# 約束建議模型（交付版）

給一張 2D 圖的圖元（線、圓、弧、點）和 1～2 對圖元，模型回傳 5 個幾何約束建議；
另附 AutoCAD 2027 操作介面（單對建議、批次找約束、尺寸約束與改值、等比例縮放）。

- **整合方式、輸入輸出格式、注意事項：請看 [整合說明.md](整合說明.md)**
- 模型：`runs_constraint/noise5/best.pt`（需搭配本資料夾的程式碼載入）
- 需要：Python 3.12、torch、numpy；控制 AutoCAD 另需 pywin32 與 AutoCAD 完整版

快速確認：
```
python constraint_suggest.py --ckpt runs_constraint/noise5/best.pt --cpu --input example_input.json
```

開啟 AutoCAD 操作介面（AutoCAD 要先開著圖檔）：
```
python autocad_interface.py
```
