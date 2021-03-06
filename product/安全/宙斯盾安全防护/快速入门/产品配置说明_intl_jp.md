
DDoS高保護IPおよびDDoS高保護パケットを購入する前に、次の点を確認する必要があります。

##準備と選択
-DDoS高保護IP
DDoS高保護IPは、プロキシ転送モードによって、サービストラフィックを高保護IPにリダイレクトし、フィルタリング後にそれを実サーバに転送してDDoS攻撃保護を提供します。現在、Tencent Cloud DDoS高保護IPは、トラフィックの多いDDoS攻撃の下で、インターネットサーバー（非Tencent Cloud Serverを含む）に安定した保護を提供します。
-DDoS高保護パケット
DDoS高保護パケットは、Tencent Cloud Serverなどの一連のクラウド製品に対して保護機能を直接提供するセキュリティ製品です。DDoS高保護IPと比較すると、DDoS高保護パケットは、クラウド保護をクラウド製品に直接バインドし、IPアドレス転送やポート間転送ルールの設定は不要です。

##DDoS高保護IP
###高保護IPエリアとネットワークの決定
 -エリア選択原則
DDoS高保護IPはプロキシ転送モードを提供しています。できるだけ実サーバの地理的な位置の近くにあるエリアを選択してください。高保護IPエリアが実サーバーに近づくほど、アクセスレイテンシは小さくなり、アクセススピードは速くなります。
 -ネットワーク選択原則
統合エリアと保護ピークのニーズに基づいてネットワークを選択します。BGPネットワークは高いネットワークエクスペリエンスを提供しますが、提供された最高の保護ピークは非BGP高保護IPよりも低くなります。CHINA TELECOM、China Unicom、CHINA MOBILEの非BGP高保護IPの最大保護ピークは順番に減少するので、ユーザ分布に応じて対応するキャリアを選択し、クロスネットワークアクセスを避けるようにしてください。

###高保護IP設定方案の決定
 -最低保証保護帯域幅ピーク
 年払いと月払いで先払いです最低保証保護帯域幅ピークがほとんどの攻撃に防御できるように、過去の攻撃トラフィックの平均を参照として、平均値よりも高い最低保証保護帯域幅ピークを設定することをお勧めします。
 -フレキシブル保護帯域幅ピーク
 従量課金し、毎日決済されます。大規模なトラフィック攻撃の場合、防御するのに十分な容量があり、保護帯域幅ピークIPを超えてブロックされないように、過去の攻撃トラフィックの最高値を参照として、過去の最高ピークよりもやや高いフレキシブル保護帯域幅ピークを設定することをお勧めします。同時に、毎月フレキシブルに従量課金され、使用しない場合は料金がかからず、費用を大幅に削減できます。
 -転送サービストラフィック
 非攻撃状態の通常のサービスの実サーバーに転送されるトラフィックです。帯域幅またはトラフィックによって課金することができます。通常のサービストラフィックの特性に従って選択することをお勧めします。

##DDoS高保護パケット
###高保護パケットエリアの決定原則
 -エリア選択原則
	DDoS高保護パケットは、現在、同じエリアのTencent CloudパブリックネットワークIPのみに高保護サービスを提供でき、Tencent Cloud実サーバと同じエリアの高保護パケットを選択してください。
	
###高保護パケット設定方案の決定
-保護範囲
単一のIPまたは複数のIPを選択できます。単一IPモード高保護パケットは、排他的な保護ピークを持つ1つのTencent CloudパブリックネットワークIPアドレスにバインドすることができます。複数IPモード高保護パケットは、保護ピークを共有する複数のTencent CloudパブリックネットワークIPアドレスにバインドすることができます。複数のIPが同時にDDoS攻撃を受ける場合、重畳ピークが保護ピークを超えると、攻撃トラフィックが最も高いIPアドレスからブロックされます。
-最低保証保護帯域幅ピーク
 年払いと月払いで先払いです最低保証保護帯域幅ピークがほとんどの攻撃に防御できるように、過去の攻撃トラフィックの平均を参照として、平均値よりも高い最低保証保護帯域幅ピークを設定することをお勧めします。
-フレキシブル保護帯域幅ピーク
従量課金し、毎日決済されます。大規模なトラフィック攻撃の場合、防御するのに十分な容量があり、保護帯域幅ピークIPを超えてブロックされないように、過去の攻撃トラフィックの最高値を参照として、過去の最高ピークよりもやや高いフレキシブル保護帯域幅ピークを設定することをお勧めします。同時に、毎月フレキシブルに従量課金され、使用しない場合は料金がかからず、費用を大幅に削減できます。
-フレキシブル課金モード
フレキシブル保護は、フレキシブルトラフィックパケットとフレキシブル帯域幅ピークの2つの課金モードをサポートします。フレキシブルトラフィックパケットは前払いで購入する必要があります。攻撃が最低保証保護帯域幅ピークを超えてフレキシブル保護使用量が生じる場合は、フレキシブルトラフィックの使用量に従ってトラフィックパケットから差し引かれます。フレキシブル帯域幅モードと比較すると、攻撃頻度が低く、攻撃帯域幅ピークが高く、持続時間が短いシナリオに対して、ユーザーのフレキシブル保護料金を著しく削減できます。サービスが頻繁に攻撃され、攻撃が長時間続く場合は、フレキシブル帯域幅ピークにより課金するモードを使用でき、フレキシブル帯域幅は日単位で課金されます。
-フレキシブルトラフィックパケット
フレキシブル保護課金モードが「フレキシブルトラフィックパケット」を選択した場合、フレキシブル保護が発生すると、、同じエリア内の購入されたフレキシブルトラフィックパケットからフレキシブルに生成されたトラフィックを差し引きます。フレキシブルトラフィックパケットが購入されていない場合、またはフレキシブルトラフィックパケットが使い尽くされた場合、フレキシブル保護機能は一時停止されます。
-フレキシブル帯域幅ピーク
フレキシブル保護課金モードが「フレキシブル帯域幅ピーク」を選択した場合、フレキシブル保護が発生すると、フレキシブル帯域幅ピークに従って日単位でユーザ課金が行われます。

