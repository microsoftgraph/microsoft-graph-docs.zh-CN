# <a name="mediacontentratingunitedstates-resource-type"></a>mediaContentRatingUnitedStates 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

尚未记录
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|movieRating|[ratingUnitedStatesMoviesType](../resources/intune_deviceconfig_ratingunitedstatesmoviestype.md)|分级美国的所选的影片。 可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults`。|
|tvRating|[ratingUnitedStatesTelevisionType](../resources/intune_deviceconfig_ratingunitedstatestelevisiontype.md)|美国的所选 TV 分级。 可取值为：`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults`。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```



