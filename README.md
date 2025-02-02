# Eval_GenerateImg
画像生成(超解像)の評価法

SSIM (Structural Similarity Index Measure)
画像の類似度を測る指標。
人間の視覚に基づき、輝度・コントラスト・構造の違いを考慮。
範囲: 0 ～ 1（1に近いほど類似している）。

MSE (Mean Squared Error, 平均二乗誤差)
2つの画像間のピクセルごとの差の二乗平均。
値が小さいほど類似度が高い（0なら完全一致）。

PSNR (Peak Signal-to-Noise Ratio, ピーク信号対雑音比)
画像の品質を測る指標（主に圧縮後の画像品質評価で使用）。
単位: dB（デシベル）。値が大きいほど元画像に近い。

NRMSE (Normalized Root Mean Squared Error, 正規化ルート平均二乗誤差)
MSE を正規化してスケールに依存しない形にした指標。
値が小さいほど画像が似ている。

HD (Hausdorff Distance, ハウスドルフ距離)
2つの画像（輪郭やバイナリ画像）の形状の違いを測る指標。
輪郭の最も遠い点の距離を計算。値が小さいほど類似度が高い。
