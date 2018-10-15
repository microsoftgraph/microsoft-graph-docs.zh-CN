# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="b3890-101">mediaContentRatingNewZealand 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3890-101">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="b3890-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b3890-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3890-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b3890-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="b3890-104">属性</span><span class="sxs-lookup"><span data-stu-id="b3890-104">Properties</span></span>
|<span data-ttu-id="b3890-105">属性</span><span class="sxs-lookup"><span data-stu-id="b3890-105">Property</span></span>|<span data-ttu-id="b3890-106">类型</span><span class="sxs-lookup"><span data-stu-id="b3890-106">Type</span></span>|<span data-ttu-id="b3890-107">说明</span><span class="sxs-lookup"><span data-stu-id="b3890-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3890-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="b3890-108">movieRating</span></span>|[<span data-ttu-id="b3890-109">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="b3890-109">ratingNewZealandMoviesType</span></span>](../resources/intune_deviceconfig_ratingnewzealandmoviestype.md)|<span data-ttu-id="b3890-p101">为新西兰选择的影片分级。可取值为： `allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted`。</span><span class="sxs-lookup"><span data-stu-id="b3890-p101">Movies rating selected for New Zealand Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="b3890-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="b3890-112">tvRating</span></span>|[<span data-ttu-id="b3890-113">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b3890-113">ratingNewZealandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingnewzealandtelevisiontype.md)|<span data-ttu-id="b3890-p102">为新西兰选择的电视评级。可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="b3890-p102">TV rating selected for New Zealand Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3890-116">关系</span><span class="sxs-lookup"><span data-stu-id="b3890-116">Relationships</span></span>
<span data-ttu-id="b3890-117">无</span><span class="sxs-lookup"><span data-stu-id="b3890-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b3890-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3890-118">JSON Representation</span></span>
<span data-ttu-id="b3890-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3890-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```








