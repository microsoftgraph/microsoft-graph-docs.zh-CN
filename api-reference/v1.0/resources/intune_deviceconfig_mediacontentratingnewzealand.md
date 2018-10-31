# <a name="mediacontentratingnewzealand-resource-type"></a>mediaContentRatingNewZealand 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

尚未记录
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|movieRating|[ratingNewZealandMoviesType](../resources/intune_deviceconfig_ratingnewzealandmoviestype.md)|为新西兰选择的影片分级。 可取值为：`allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`。|
|tvRating|[ratingNewZealandTelevisionType](../resources/intune_deviceconfig_ratingnewzealandtelevisiontype.md)|为新西兰选择的电视分级。 可取值为：`allAllowed`  `allBlocked`, `general`, `parentalGuidance`, `adults`.|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```



