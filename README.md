# unity-LiquidChain
# 糸を引く液体のスクリプト
![liquidChainSampleImage](https://user-images.githubusercontent.com/39085780/105623709-17da0400-5e5f-11eb-9d0f-7fa4aebd428e.jpg)

糸を引く液体を再現するためのスクリプトです

## 使い方
LineRendererを持つGameObjectに割り当てます

## パラメータ

### Solver.IterationCount
演算回数です。数を増やすほど糸が垂れにくくなります。

### Solver.NumOfPoints
頂点数です。頂点数が多いほど滑らかになりますが、糸が垂れやすくなります。

### Solver.BreakThreshold
糸の切れるしきい値です。小さければ小さいほど切れにくくなります。

### Solver.StraightRange
糸がまっすぐになる範囲です。

### Solver.GravityMultiplier
重力係数(-9.8)に乗算されます。
1だと落ちるのが早すぎるので、0.2くらいが良いかもしれません。

### Solver.LiquidQuantity
両端の液体の量です。ラインの太さに影響します。

### Solver.LifeTimeFramesOfBrokenChain
糸が切れてからの生存フレーム数です。

### LineRenderSetting.Width
糸の基準太さです。

### LineRenderSetting.MinWidth
糸の最小の太さです。

### LineRenderSetting.BaseLength
糸が伸びるほど細くなるときの、基準の長さです。

### TargetSettings.TouchDistance
対象が触れたと判定される距離です。

### TargetSettings.TargetTag
対象を検索する際のTag名です。
デフォルトはLiquidChainTargetなので、このタグが存在しない場合は作成する必要があります。
