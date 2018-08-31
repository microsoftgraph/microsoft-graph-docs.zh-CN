# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="c9452-101">mediaContentRatingNewZealand 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9452-101">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="c9452-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c9452-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9452-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c9452-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c9452-104">属性</span><span class="sxs-lookup"><span data-stu-id="c9452-104">Properties</span></span>
|<span data-ttu-id="c9452-105">属性</span><span class="sxs-lookup"><span data-stu-id="c9452-105">Property</span></span>|<span data-ttu-id="c9452-106">类型</span><span class="sxs-lookup"><span data-stu-id="c9452-106">Type</span></span>|<span data-ttu-id="c9452-107">说明</span><span class="sxs-lookup"><span data-stu-id="c9452-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9452-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="c9452-108">movieRating</span></span>|[<span data-ttu-id="c9452-109">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="c9452-109">ratingNewZealandMoviesType</span></span>](../resources/intune_deviceconfig_ratingnewzealandmoviestype.md)|<span data-ttu-id="c9452-110">为新西兰选择的影片分级。</span><span class="sxs-lookup"><span data-stu-id="c9452-110">Movies rating selected for New Zealand Possible values are: , , , , , , , , , , .</span></span> <span data-ttu-id="c9452-111">可取值为：`allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`。</span><span class="sxs-lookup"><span data-stu-id="c9452-111">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`, or .</span></span>|
|<span data-ttu-id="c9452-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="c9452-112">tvRating</span></span>|[<span data-ttu-id="c9452-113">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c9452-113">ratingNewZealandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingnewzealandtelevisiontype.md)|<span data-ttu-id="c9452-114">为新西兰选择的电视分级。</span><span class="sxs-lookup"><span data-stu-id="c9452-114">TV rating selected for New Zealand Possible values are: , , , , .</span></span> <span data-ttu-id="c9452-115">|||UNTRANSLATED_CONTENT_START|||The possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.|||UNTRANSLATED_CONTENT_END|||</span><span class="sxs-lookup"><span data-stu-id="c9452-115">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`, , , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9452-116">关系</span><span class="sxs-lookup"><span data-stu-id="c9452-116">Relationships</span></span>
<span data-ttu-id="c9452-117">无</span><span class="sxs-lookup"><span data-stu-id="c9452-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c9452-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9452-118">JSON Representation</span></span>
<span data-ttu-id="c9452-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9452-119">Here is a JSON representation of the resource.</span></span>
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



