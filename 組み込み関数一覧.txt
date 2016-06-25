■BlockLauncherに組み込まれている関数の一覧です。
  // 参考ver.1.12.4
  

addItemInventory(ID,個数,ダメージ値);  //インベントリにアイテム追加

clientMessage("文字列");  //チャット欄にメッセージ表示

explode(x,y,z,爆発半径,true又はfalse);  //指定座標を爆発

getCarriedItem();  //手持ちアイテムID取得

getLevel();  //難易度取得

getPitch(円角度);  //縦回転軸を取得

getPlayerEnt();  //プレイヤー情報取得

getPlayerX();  //プレイヤーのx値取得
getPlayerY();  //プレイヤーのy値取得
getPlayerZ();  //プレイヤーのz値取得

getTile(x,y,z);  //ブロック情報取得

getYaw(視覚方向);  //横回転軸を取得

preventDefault();  //通常の動作を防ぐ

print("文字列");  //一定時間メッセージ表示

rideAnimal(対象エンティティ,騎乗エンティティ);  //エンティティに乗る

setNightMode(true又はfalse);  //ナイトモードへの変更。trueで常夜に移行。

setPosition(エンティティ,x,y,z);  //指定座標にエンティティをセット

setPositionRelative(エンティティ,x,y,z);  //エンティティを指定座標方向に動かす

setRot(エンティティ, 横回転軸, 縦回転軸);  //指定エンティティの視覚を指定

setTile(x,y,z,ID,ダメージ値);  //指定座標にブロックを設置

setVelX(エンティティ, 速度);  //0.3で1ブロックの単位で対象をx方向に速度を加える
setVelY(エンティティ, 速度);  //0.3で1ブロックの単位で対象をy方向に速度を加える
setVelZ(エンティティ, 速度);  //0.3で1ブロックの単位で対象をz方向に速度を加える

spawnChicken(x,y,z,"スキンURL");  //鶏をスポーン

spawnCow(x,y,z,"スキンURL");  //牛をスポーン

spawnPigZombie(x,y,z,ID,"スキンURL");  //ゾンビピッグマンを指定アイテムを持たせてスポーン





ModPE.dumpVtable("par1文字列", par2整数);  //？？？

ModPE.getBytesFromTexturePack("アドレス");  //？？？

ModPE.getI18n("par1文字列");  //詳細不明。多言語化ファイルを読み込む？

ModPE.getLanguage();  //現在使用されている言語を取得

ModPE.getMinecraftVersion();  //MCPEのバージョン情報を取得

ModPE.langEdit("元の文字列","編集文字列");  //en_US.langの文字列を元に表示されるアイテム名を編集

ModPE.leaveGame();  //ワールドを閉じる時に実行

ModPE.log("文字列");  //システムコンソールに指定メッセージを出力

ModPE.openInputStreamFromTexturePack("アドレス");  //？？？

ModPE.overrideTexture(対象, "URL");  //指定対象のテクスチャにURLのテクスチャをオーバーライドさせる

ModPE.readData("保存した変数名");  //保存したデータの読み込み
ModPE.removeData("保存した変数名");  //保存したデータの削除
ModPE.saveData("保存する変数名", 保存内容);  //残したいデータを保存

ModPE.resetFov();  //変更した視野を初期値にリセット
ModPE.resetImages();  //変更したテクスチャをリセット

ModPE.selectLevel("ワールド名", "ワールドのディレクトリ");  //ワールド間を移動。第1引数のみでも可。

ModPE.setCamera(エンティティ);  //指定エンティティの視覚に切り替える

ModPE.setFoodItem(ID,"テクスチャネーム",グループ指定,満腹量,"アイテムネーム",ストック制限);  //食べ物を追加

ModPE.setFov(視野値);  //指定数値の視野に変更

ModPE.setGameSpeed(毎秒チック数);  //1秒を指定チック(標準秒間20チック)に変更

ModPE.setItem(ID,"テクスチャネーム",グループ番号,"アイテムネーム",ストック制限);  //アイテムを追加

ModPE.setGuiBlocks("アドレス");  //GUIのブロックテクスチャを任意のファイルに変更
ModPE.setItems("アドレス");  //アイテムテクスチャを任意のファイルに変更
ModPE.setTerrain("アドレス");  //Terrainのブロックテクスチャを任意のファイルに変更

ModPE.setUiRenderDebug(true又はfalse);  //画面にデバッグ表示をさせる。UseDesktop GUIがONの場合はタイトル以外にもGUI 等にデバッグ表示されるようになる

ModPE.showTipMessage("文字列");  //即時上書き可能のメッセージを表示

ModPE.takeScreenshot("文字列");  //指定文字列でスクショを保存





Level.addParticle(パーティクルタイプ,始点x,始点y,始点z,方向x,方向y,方向z,サイズ);  //指定のパーティクルを生成

Level.biomeIdToName(バイオームID);  //指定したバイオーム番号のバイオーム名を返す

Level.canSeeSky(x,y,z);  //座標の真上に空があるかどうかをtrue(有)かfalse(無)で返す

Level.destroyBlock(x,y,z,ドロップ指定);  //指定座標ブロックの破壊。true(そのままドロップ)又はfalse(消滅)を指定

Level.dropItem(x,y,z,跳ねる高さ,ID,個数,ダメージ値);  //指定アイテムのドロップ

Level.explode(x,y,z,爆発半径,true又はfalse);  //指定座標を爆発

Level.getAddress();  //？？？

Level.getBiome(x,z);  //指定座標のバイオームIDを取得
Level.getBiomeName(x,z);  //指定座標のバイオーム名を取得

Level.getBrightness(x,y,z);  //指定座標の光度を取得

Level.getChestSlot(x,y,z,スロット番号);  //指定座標のチェストのスロットからIDを取得
Level.getChestSlotCount(x,y,z,スロット番号);  //指定座標のチェストのスロットから所持数を取得
Level.getChestSlotCustomName(x,y,z,スロット番号);  //指定座標のチェストのスロットから表示ネームを取得
Level.getChestSlotData(x,y,z,スロット番号);  //指定座標のチェストのスロットからダメージ値を取得

Level.getData(x,y,z);  //指定座標ブロックのダメージ値を取得

Level.getDifficulty();  //現在の難易度を取得。0がピースフル

Level.getFurnaceSlot(x,y,z,スロット);  //石窯のスロットのIDデータを取得。0が原料、1が燃料、2が完成品
Level.getFurnaceSlotCount(x,y,z,スロット);  //石窯のスロットの個数データを取得。
Level.getFurnaceSlotData(x,y,z,スロット);  //石窯のスロットのダメージ値データを取得。

Level.getGameMode();  //現在のゲームモードを取得

Level.getGrassColor(x, z);  //指定座標の草ブロックのカラー情報を取得

Level.getLightningLevel();  //雷の有無の状態を0～1の数値で返す

Level.getRainLevel();  //雨の有無の状態を0～1の数値で返す

Level.getSignText(x,y,z,行数);  //指定座標の指定行の内容を取得

Level.getSpawnerEntityType(x,y,z);  //指定座標のスポナーにセットされてるエンティティIDを取得

Level.getTile(x,y,z);  //ブロック情報の取得

Level.getTime();  //ゲーム内時間を取得

Level.getWorldDir();  //ワールドのフォルダ名を取得

Level.getWorldName();  //ワールド名を取得

Level.playSound(x,y,z,"サウンド名",音量,ピッチ);  //指定座標からゲームサウンドを再生

Level.playSoundEnt(エンティティ,"サウンド名",音量,ピッチ);  //指定したエンティティからゲームサウンドを再生

Level.setChestSlot(x,y,z,スロット,ID,ダメージ値,数量);  //指定座標のチェストの指定スロットにアイテムをセット
Level.setChestSlotCustomName(x,y,z,スロット,ネーム);  //指定座標のチェストの指定スロットに表示ネームをセット

Level.setDifficulty(難易度);  //指定の難易度に変更する

Level.setFurnaceSlot(x,y,z,スロット,ID,ダメージ値,数量);  //指定座標の石窯のスロットにアイテムをセット

Level.setGameMode(ゲームモードID);  //指定のゲームモードに変更

Level.setGrassColor(x,z,カラーコード);  //指定座標の草ブロックの色を変更

Level.setLightningLevel(0又は1);  //雷の有無を切り替え。或いはtrue又はfalse。

Level.setNightMode(true又はfalse);  //ナイトモードへの変更。trueで常夜に移行。

Level.setRainLevel(0又は1);  //雨の有無を切り替え。或いはtrue又はfalse。

Level.setSignText(x,y,z,行数,"文字列");  //指定座標の指定行に文字を記入

Level.setSpawn(x,y,z);  //指定座標にプレイヤーのスポーン地点をセット

Level.setSpawnerEntityType(x, y, z, エンティティID);  //指定座標のスポナーにエンティティをセット

Level.setTile(x,y,z,ID,ダメージ値);  //指定座標にブロックを設置

Level.setTime(時間);  //指定した時間に変更。マイクラ内の1日は24000チックで、12540チックからベッドで寝れるようになる

Level.spawnChicken(x,y,z,"スキンURL");  //指定座標に鶏をスポーン

Level.spawnCow(x,y,z,"スキンURL");  //指定座標に牛をスポーン

Level.spawnMob(x,y,z,エンティティタイプID,"スキンURL");  //指定座標に指定のMOBをスポーン





/*プレイヤーを対象とした関数*/

Player.addExp(経験値);  //指定した分の経験値を追加する

Player.addItemCreativeInv(ID,数量,ダメージ値);  //クリエイティブにアイテムを追加

Player.addItemInventory(ID,数量,ダメージ値);  //インベントリにアイテムを追加

Player.canFly();  //飛行可能状態(true)か不可能状態(false)を取得

Player.clearInventorySlot(スロット);  //インベントリから指定スロットのアイテムを消去

Player.enchant(スロット,エンチャント,レベル);  //指定スロットにエンチャントを付与する

Player.getArmorSlot(スロット);  //指定スロットの防具のIDを取得
Player.getArmorSlotDamage(スロット);  //指定スロットの防具のダメージ値を取得

Player.getCarriedItem();  //手持ちのIDを取得
Player.getCarriedItemCount();  //手持ちの数量を取得
Player.getCarriedItemData();  //手持ちのダメージ値を取得

Player.getDimension();  //現在地のディメンションを取得。0が通常で1がネザー

Player.getEnchantments(スロット);  //指定スロットのエンチャントを取得

Player.getEntity();  //プレイヤーのエンティティ情報を取得

Player.getExhaustion();  //スタミナの消耗値を取得。0～4迄の間を返し、4になると隠し満腹度を1消費し0にリセットされる。隠し満腹度が0の場合は満腹度から1引かれてリセットされる

Player.getExp();  //現在の経験値を取得。0～1の数値を返し、1になるとレベルが1上がりリセットされる

Player.getHunger();  //満腹度を取得

Player.getInventorySlot(スロット);  //指定スロットのIDを取得
Player.getInventorySlotCount(スロット);  //指定スロットの数量を取得
Player.getInventorySlotData(スロット);  //指定スロットのダメージ値を取得

Player.getItemCustomName(スロット);  //指定スロットの表示ネームを取得

Player.getLevel();  //現在のレベルを取得

Player.getName(プレイヤー);  //プレイヤーリストからプレイヤーの名前を取得

Player.getPointedBlockData();  //ポイントしたブロックのダメージ値を取得
Player.getPointedBlockId();  //ポイントしたブロックのIDを取得
Player.getPointedBlockSide();  //ポイントしたブロックの面方向を取得

Player.getPointedBlockX();  //ポイントしたブロックのx値を取得
Player.getPointedBlockY();  //ポイントしたブロックのy値を取得
Player.getPointedBlockZ();  //ポイントしたブロックのz値を取得

Player.getPointedEntity();  //ポイントしたエンティティの情報を取得

Player.getPointedVecX();  //ポイントしたブロック面の座標を取得。平面的に見て変動が無い軸では整数のみ返す
Player.getPointedVecY();  //ポイントしたブロック面の座標を取得。平面的に見て変動が無い軸では整数のみ返す
Player.getPointedVecZ();  //ポイントしたブロック面の座標を取得。平面的に見て変動が無い軸では整数のみ返す

Player.getSaturation();  //隠し満腹度を取得

Player.getScore();  //プレイヤーのスコアを取得。プレイヤーの行動によって加算され、死ぬと0にリセットされる

Player.getSelectedSlotId();  //ホットバーで選択されているスロット番号を取得

Player.getX();  //プレイヤーのx値取得
Player.getY();  //プレイヤーのy値取得
Player.getZ();  //プレイヤーのz値取得

Player.isFlying();  //飛行状態かどうかを取得

Player.isPlayer(プレイヤー);  //指定したプレイヤーをチェック

Player.setArmorSlot(スロット,ID,ダメージ値);  //指定したスロットに防具をセット

Player.setCanFly(0又は1);  //0(無飛行)又は1(飛行)で飛行出来るようにするかを変更。又はfalseかtrue

Player.setExhaustion(疲労値);  //指定数値のスタミナを消費させる。4毎に隠し満腹度、又は満腹度を1消費する

Player.setExp(経験値);  //経験値を指定した数値に変更する。1以上にしても経験値が追加されないとレベルが上がらず、また1度に1レベル以上は上がらない

Player.setFlying(true又はfalse);  //trueで飛行状態、falseで無飛行状態にする

Player.setHealth(体力);  //指定した体力値に変更する

Player.setHunger(空腹度);  //指定の空腹度に変更する。20でフルゲージ

Player.setInventorySlot(スロット,ID,数量,ダメージ値);  //指定スロットの情報を変更する

Player.setItemCustomName(スロット,"変更ネーム");  //指定スロットの表示ネームを変更する

Player.setLevel(レベル);  //指定したレベルに変更する

Player.setSaturation(隠し満腹値);  //隠し満腹度を指定の数値に変更する。上限は20で、それ以上の数値は変化時に20に変えられる

Player.setSelectedSlotId(番号);  //手持ちアイテムを指定スロットに変更





/*エンティティ全般*/

Entity.addEffect(エンティティ, エフェクトID, 効果時間, レベル, 範囲?(ambient), パーティクル表現の有無?(showParticles));  //指定エンティティにエフェクトを追加する

Entity.getAll();  //全てのエンティティ情報を取得

Entity.getAnimalAge(エンティティ);  //指定エンティティの年齢を取得

Entity.getArmor(エンティティ,スロット);  //指定エンティティのスロットの防具のIDを取得
Entity.getArmorCustomName(エンティティ,スロット);  //指定エンティティのスロットの防具の表示ネームを取得
Entity.getArmorDamage(エンティティ,スロット);  //指定エンティティのスロットの防具のダメージ値を取得

Entity.getEntityTypeId(エンティティ);  //指定エンティティのエンティティIDを取得

Entity.getExtraData(エンティティ,"ネーム.MOD名.データ");  //保存されたデータを読み込む

Entity.getHealth(エンティティ);  //指定エンティティの体力を取得

Entity.getItemEntityCount(エンティティ);  //ドロップアイテムの数を取得
Entity.getItemEntityData(エンティティ);  //ドロップアイテムのダメージ値を取得
Entity.getItemEntityId(エンティティ);  //ドロップアイテムのIDを取得

Entity.getMaxHealth(エンティティ);  //指定エンティティの最大HPを取得

Entity.getMobSkin(エンティティ);  //指定エンティティのスキン情報を取得

Entity.getNameTag(エンティティ);  //指定エンティティのタグネームを取得

Entity.getPitch(エンティティ);  //指定エンティティの視覚情報を取得

Entity.getRenderType(エンティティ);  //指定エンティティのレンダリングIDを取得

Entity.getRider(エンティティ);  //指定エンティティに乗っているエンティティ情報を取得

Entity.getRiding(エンティティ);  //指定エンティティに乗られているエンティティ情報を取得

Entity.getTarget(エンティティ);  //指定エンティティが敵対するMOBを取得

Entity.getUniqueId(エンティティ);  //指定エンティティのUUIDを取得

Entity.getVelX(エンティティ);  //指定エンティティのx値の速度を取得
Entity.getVelY(エンティティ);  //指定エンティティのy値の速度を取得
Entity.getVelZ(エンティティ);  //指定エンティティのz値の速度を取得

Entity.getX(エンティティ);  //指定エンティティのx値を取得
Entity.getY(エンティティ);  //指定エンティティのy値を取得
Entity.getZ(エンティティ);  //指定エンティティのz値を取得

Entity.getYaw(エンティティ);  //指定エンティティの視覚方向を取得

Entity.isSneaking(エンティティ);  //エンティティのスニーク判定を取得

Entity.remove(エンティティ);  //指定エンティティを消去します。

Entity.removeAllEffects(エンティティ);  //指定エンティティのエフェクトを全て無効化する
Entity.removeEffect(エンティティ, エフェクトID);  //指定エンティティの指定エフェクトを無効化する

Entity.rideAnimal(騎乗エンティティ,対象エンティティ);  //指定エンティティを指定エンティティに騎乗させる

Entity.setAnimalAge(エンティティ,年齢);  //指定エンティティを指定の年齢にする。

Entity.setArmor(エンティティ,スロット,ID, ダメージ値);  //指定エンティティの指定部位に指定防具アイテムをセット
Entity.setArmorCustomName(エンティティ,スロット,"表示ネーム");  //指定エンティティの指定部位に表示ネームをセット

Entity.setCape(エンティティID, "アドレス");  //指定エンティティにマントを付与

Entity.setCarriedItem(エンティティ,ID,数量,ダメージ値);  //指定エンティティの持ち物を変更

Entity.setCollisionSize(エンティティ, サイズxとz, サイズy);  //エンティティのヒットボックスを設定？(フォーラム情報。未確認)

Entity.setExtraData(エンティティ,"ネーム.MOD名.データ","保存ファイル名");  //エンティティデータを保存

Entity.setFireTicks(エンティティ, 時間);  //指定エンティティを指定時間燃やす

Entity.setHealth(エンティティ, 体力);  //指定エンティティを指定体力に変更

Entity.setImmobile(エンティティ,true又はfalse);  //指定エンティティの動きをtrueで止め、falseで解除する

Entity.setMaxHealth(エンティティ,体力);  //指定エンティティの最大体力値をセット

Entity.setMobSkin(エンティティ,"スキンURL");  //指定エンティティのスキンをMCPE内にあるスキンに変更

Entity.setNameTag(エンティティ,"ネーム");  //指定エンティティに指定ネームを付ける

Entity.setPosition(エンティティ,x,y,z);  //指定エンティティを指定座標に変更

Entity.setPositionRelative(エンティティ,x方向,y方向,z方向);  //指定エンティティを指定方向に飛ばす

Entity.setRenderType(エンティティ,レンダータイプ);  //指定エンティティに指定のレンダリングをする

Entity.setRot(エンティティ,横回転軸,縦回転軸);  //指定エンティティの視覚を指定

Entity.setSneaking(エンティティ,true又はfalse);  //指定エンティティのスニーキング設定

Entity.setTarget(エンティティ,ターゲット);  //指定エンティティをターゲットに敵対させる

Entity.setVelX(エンティティ,速度);  //0.3で1ブロックの単位で対象をx方向に速度を加える
Entity.setVelY(エンティティ,速度);  //0.3で1ブロックの単位で対象をy方向に速度を加える
Entity.setVelZ(エンティティ,速度);  //0.3で1ブロックの単位で対象をz方向に速度を加える

Entity.spawnMob(x,y,z,エンティティID,"スキンURL");  //MOBのスポーン





/*アイテム関連*/

Item.addCraftRecipe(ID,個数,ダメージ値,[ID,個数,ダメージ値]);  //クラフトレシピの追加

Item.addFurnaceRecipe(素材ID,完成ID,ダメージ値);  //石窯レシピの追加

Item.addShapedRecipe(ID,個数,ダメージ値,["ABC","DEF","GHI"],["変数",ID,ダメージ値]);  //クラフトレシピの追加

Item.defineArmor(ID,"表示テクスチャネーム",順番指定,"アイテムネーム","装着時のテクスチャアドレス",防御力,耐久力,アーマータイプID);  //防具アイテムの追加

Item.getMaxDamage(ID);  //指定IDの最大耐久値を取得

Item.getMaxStackSize(ID);  //指定IDの最大ストック数を取得

Item.getName(ID,ダメージ値,true又はfalse);  //指定アイテムのシステムアイテム名を取得。trueで取得、falseで取得しない

Item.getTextureCoords(ID, ダメージ値);  //指定アイテムのテクスチャ位置を取得

Item.getUseAnimation(ID);  //指定IDのアニメーションタイプを取得

Item.internalNameToId("アイテム名");  //英語の指定アイテム名のIDを取得

Item.isValidItem(ID);  //指定IDが有効であればtrueを返す(？)

Item.setCategory(ID,カテゴリー);  //アイテムカテゴリーの設定

Item.setEnchantType(ID,ツールタイプ,0又は1);  //追加アイテムに指定ツールタイプのエンチャント付与が出来るようにする。1で有効化、0で無効化。或いはtrue又はfalse

Item.setHandEquipped(ID,true又はfalse);  //剣などのようにアイテムを持つ時に握った状態で持たせる。trueで握った状態

Item.setMaxDamage(ID,耐久力);  //指定アイテムに耐久値を設定

Item.setProperties(ID,{プロパティ});  //json形式のアイテムを設定

Item.setStackedByData(ID,true又はfalse);  //

Item.setUseAnimation(ID,アニメーションタイプ);  //指定IDのアニメーションタイプを設定。通常は0、ドリンクが2、弓が4。

Item.translatedNameToId("アイテム名");  //指定アイテム名と同じ言語を選択していた場合にIDを取得





/*ブロック関連*/

Block.defineBlock(ID,"表示ネーム",[["テクスチャネーム(底面)",順番指定],["テクスチャネーム(上面)",順番指定],["テクスチャネーム(北面)",順番指定],["テクスチャネーム(南面)",順番指定],["テクスチャネーム(西面)",順番指定],["テクスチャネーム(東面)",順番指定]],適性ツール設定,光透過設定,ブロック形状設定);  //ブロックを追加

Block.defineLiquidBlock(ID,"表示ネーム",[["テクスチャネーム(溜まり用)",順番指定],["テクスチャネーム(流れ用)",順番指定]],液状タイプ);  //液体ブロックを追加。8で水タイプ、10で溶岩タイプ。

Block.getAllBlockIds();  //ブロックのx,y,zとvelX,velY,velZを取得？

Block.getDestroyTime(ID,par2整数);  //指定したブロックIDの破壊時間を取得。par2は不明だが無くても機能するのは確認済み

Block.getFriction(ID,par2整数);  //指定したブロックIDの上を歩いた時の摩擦度(滑りやすさ)を取得。par2は不明だが無くても機能するのは確認済み

Block.getRenderType(ID);  //対象ブロックのブロック形状を取得

Block.getTextureCoords(ID, サイド,ダメージ値);  //指定ブロックの指定面のテクスチャ位置を取得

Block.setColor(ID,[0x(Hexカラーコード)]);  //指定ブロックのカラーを変更

Block.setDestroyTime(ID,秒数);  //指定ブロックの破壊時間の設定

Block.setExplosionResistance(ID,耐性値);  //指定ブロックの爆発耐性を設定

Block.setFriction(ID,摩擦度);  //指定したブロックIDの摩擦度をセット。通常は0.6、氷では0.9。数値が低いと滑りにくくなりグリップが上がるのか移動速度が上がり、高いと移動し辛く滑りやすくなって制御が効かなくなってくる

Block.setLightLevel(ID,光度);  //指定ブロックの光度を設定

Block.setLightOpacity(ID,不透明度);  //指定ブロックの光を通す度合いを設定

Block.setRedstoneConsumer(ID,true又はfalse);  //指定したブロックIDにレッドストーンパワーの有無をセット？

Block.setRenderLayer(ID,レイヤー番号);  //指定ブロックのレイヤー設定。

Block.setRenderType(ID,形状タイプID);  //指定ブロックを指定ブロック形状にレンダリングする設定

Block.setShape(ID,始点x,始点y,始点z,終点x,終点y,終点z,ダメージ値);  //指定ブロックの形状を変化させる





Server.getAddress();  //プレイヤーの入っているサーバーのIPアドレスを取得

Server.getAllPlayerNames();  //入っているサーバーに居るプレイヤー名を取得

Server.getAllPlayers();  //入っているサーバーのプレイヤー情報を取得

Server.getPort();  //プレイヤーの入っているサーバーのポート番号を取得

Server.joinServer(IP,ポート);  //指定のサーバーに入る

Server.sendChat("文字列");  //プレイヤーの名前でチャットメッセージを送信






// can use preventDefault()
function attackHook(attacker, victim)
// can use preventDefault()
function chatHook(str)
// can use preventDefault()
function continueDestroyBlock(x, y, z, side, progress)
// can use preventDefault()
function destroyBlock(x, y, z, side)
function projectileHitEntityHook(projectile, targetEntity)
function eatHook(hearts, saturationRatio)
function entityAddedHook(entity)
// can use preventDefault()
function entityHurtHook(attacker, victim, halfhearts)
function entityRemovedHook(entity)
// can use preventDefault()
function explodeHook(entity, x, y, z, power, onFire)
// can use preventDefault()
function serverMessageReceiveHook(str)
// can use preventDefault()
function deathHook(attacker, victim)
// can use preventDefault()
function playerAddExpHook(player, experienceAdded)
// can use preventDefault()
function playerExpLevelChangeHook(player, levelsAdded)
function redstoneUpdateHook(x, y, z, newCurrent, someBooleanIDontKnow, blockId, blockData)
function newLevel()
// can use preventDefault()
function startDestroyBlock(x, y, z, side)
function projectileHitBlockHook(projectile, blockX, blockY, blockZ, side)
function modTick()
// can use preventDefault()
function useItem(x, y, z, itemid, blockid, side, itemDamage, blockDamage)

ChatColor.AQUA;
ChatColor.BEGIN;
ChatColor.BLACK;
ChatColor.BLUE;
ChatColor.BOLD;
ChatColor.DARK_AQUA;
ChatColor.DARK_BLUE;
ChatColor.DARK_GRAY;
ChatColor.DARK_GREEN;
ChatColor.DARK_PURPLE;
ChatColor.DARK_RED;
ChatColor.GOLD;
ChatColor.GRAY;
ChatColor.GREEN;
ChatColor.LIGHT_PURPLE;
ChatColor.RED;
ChatColor.RESET;
ChatColor.WHITE;
ChatColor.YELLOW;

ItemCategory.DECORATION;
ItemCategory.FOOD;
ItemCategory.INTERNAL;
ItemCategory.MATERIAL;
ItemCategory.TOOL;

ParticleType.angryVillager;
ParticleType.bubble;
ParticleType.cloud;
ParticleType.crit;
ParticleType.dripLava;
ParticleType.dripWater;
ParticleType.enchantmenttable;
ParticleType.fallingDust;
ParticleType.flame;
ParticleType.happyVillager;
ParticleType.heart;
ParticleType.hugeexplosion;
ParticleType.hugeexplosionSeed;
ParticleType.ink;
ParticleType.itemBreak;
ParticleType.largeexplode;
ParticleType.lava;
ParticleType.mobFlame;
ParticleType.note;
ParticleType.portal;
ParticleType.rainSplash;
ParticleType.redstone;
ParticleType.slime;
ParticleType.smoke;
ParticleType.smoke2;
ParticleType.snowballpoof;
ParticleType.spell;
ParticleType.spell2;
ParticleType.spell3;
ParticleType.splash;
ParticleType.suspendedTown;
ParticleType.terrain;
ParticleType.waterWake;

EntityType.ARROW;
EntityType.BAT;
EntityType.BLAZE;
EntityType.BOAT;
EntityType.CAVE_SPIDER;
EntityType.CHICKEN;
EntityType.COW;
EntityType.CREEPER;
EntityType.EGG;
EntityType.ENDERMAN;
EntityType.EXPERIENCE_ORB;
EntityType.EXPERIENCE_POTION;
EntityType.FALLING_BLOCK;
EntityType.FIREBALL;
EntityType.FISHING_HOOK;
EntityType.GHAST;
EntityType.IRON_GOLEM;
EntityType.ITEM;
EntityType.LAVA_SLIME;
EntityType.LIGHTNING_BOLT;
EntityType.MINECART;
EntityType.MUSHROOM_COW;
EntityType.OCELOT;
EntityType.PAINTING;
EntityType.PIG;
EntityType.PIG_ZOMBIE;
EntityType.PLAYER;
EntityType.PRIMED_TNT;
EntityType.RABBIT;
EntityType.SHEEP;
EntityType.SILVERFISH;
EntityType.SKELETON;
EntityType.SLIME;
EntityType.SMALL_FIREBALL;
EntityType.SNOWBALL;
EntityType.SNOW_GOLEM;
EntityType.SPIDER;
EntityType.SQUID;
EntityType.THROWN_POTION;
EntityType.VILLAGER;
EntityType.WOLF;
EntityType.ZOMBIE;
EntityType.ZOMBIE_VILLAGER;

EntityRenderType.arrow;
EntityRenderType.bat;
EntityRenderType.blaze;
EntityRenderType.boat;
EntityRenderType.camera;
EntityRenderType.chicken;
EntityRenderType.cow;
EntityRenderType.creeper;
EntityRenderType.egg;
EntityRenderType.enderman;
EntityRenderType.expPotion;
EntityRenderType.experienceOrb;
EntityRenderType.fallingTile;
EntityRenderType.fireball;
EntityRenderType.fishHook;
EntityRenderType.ghast;
EntityRenderType.human;
EntityRenderType.ironGolem;
EntityRenderType.item;
EntityRenderType.lavaSlime;
EntityRenderType.lightningBolt;
EntityRenderType.map;
EntityRenderType.minecart;
EntityRenderType.mushroomCow;
EntityRenderType.ocelot;
EntityRenderType.painting;
EntityRenderType.pig;
EntityRenderType.player;
EntityRenderType.rabbit;
EntityRenderType.sheep;
EntityRenderType.silverfish;
EntityRenderType.skeleton;
EntityRenderType.slime;
EntityRenderType.smallFireball;
EntityRenderType.snowGolem;
EntityRenderType.snowball;
EntityRenderType.spider;
EntityRenderType.squid;
EntityRenderType.thrownPotion;
EntityRenderType.tnt;
EntityRenderType.unknownItem;
EntityRenderType.villager;
EntityRenderType.villagerZombie;
EntityRenderType.witch;
EntityRenderType.wolf;
EntityRenderType.zombie;
EntityRenderType.zombiePigman;

ArmorType.boots;
ArmorType.chestplate;
ArmorType.helmet;
ArmorType.leggings;

MobEffect.effectIds;
MobEffect.absorption;
MobEffect.blindness;
MobEffect.confusion;
MobEffect.damageBoost;
MobEffect.damageResistance;
MobEffect.digSlowdown;
MobEffect.digSpeed;
MobEffect.fireResistance;
MobEffect.harm;
MobEffect.heal;
MobEffect.healthBoost;
MobEffect.hunger;
MobEffect.invisibility;
MobEffect.jump;
MobEffect.movementSlowdown;
MobEffect.movementSpeed;
MobEffect.nightVision;
MobEffect.poison;
MobEffect.regeneration;
MobEffect.saturation;
MobEffect.waterBreathing;
MobEffect.weakness;
MobEffect.wither;

DimensionId.NETHER;
DimensionId.NORMAL;

BlockFace.DOWN;
BlockFace.EAST;
BlockFace.NORTH;
BlockFace.SOUTH;
BlockFace.UP;
BlockFace.WEST;

UseAnimation.bow;
UseAnimation.normal;

Enchantment.AQUA_AFFINITY;
Enchantment.BANE_OF_ARTHROPODS;
Enchantment.BLAST_PROTECTION;
Enchantment.DEPTH_STRIDER;
Enchantment.EFFICIENCY;
Enchantment.FEATHER_FALLING;
Enchantment.FIRE_ASPECT;
Enchantment.FIRE_PROTECTION;
Enchantment.FLAME;
Enchantment.FORTUNE;
Enchantment.INFINITY;
Enchantment.KNOCKBACK;
Enchantment.LOOTING;
Enchantment.LUCK_OF_THE_SEA;
Enchantment.LURE;
Enchantment.POWER;
Enchantment.PROJECTILE_PROTECTION;
Enchantment.PROTECTION;
Enchantment.PUNCH;
Enchantment.RESPIRATION;
Enchantment.SHARPNESS;
Enchantment.SILK_TOUCH;
Enchantment.SMITE;
Enchantment.THORNS;
Enchantment.UNBREAKING;

EnchantType.all;
EnchantType.axe;
EnchantType.book;
EnchantType.bow;
EnchantType.fishingRod;
EnchantType.flintAndSteel;
EnchantType.hoe;
EnchantType.pickaxe;
EnchantType.shears;
EnchantType.shovel;
EnchantType.weapon;

BlockRenderLayer.alpha;
BlockRenderLayer.alpha_seasons;
BlockRenderLayer.alpha_single_side;
BlockRenderLayer.blend;
BlockRenderLayer.doubleside;
BlockRenderLayer.far;
BlockRenderLayer.opaque;
BlockRenderLayer.opaque_seasons;
BlockRenderLayer.seasons_far;
BlockRenderLayer.seasons_far_alpha;
BlockRenderLayer.water;
