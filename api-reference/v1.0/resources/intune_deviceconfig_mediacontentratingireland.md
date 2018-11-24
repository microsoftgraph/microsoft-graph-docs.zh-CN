# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="e39b8-101">mediaContentRatingIreland 资源类型</span><span class="sxs-lookup"><span data-stu-id="e39b8-101">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="e39b8-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e39b8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e39b8-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e39b8-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="e39b8-104">属性</span><span class="sxs-lookup"><span data-stu-id="e39b8-104">Properties</span></span>
|<span data-ttu-id="e39b8-105">属性</span><span class="sxs-lookup"><span data-stu-id="e39b8-105">Property</span></span>|<span data-ttu-id="e39b8-106">类型</span><span class="sxs-lookup"><span data-stu-id="e39b8-106">Type</span></span>|<span data-ttu-id="e39b8-107">说明</span><span class="sxs-lookup"><span data-stu-id="e39b8-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e39b8-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="e39b8-108">movieRating</span></span>|[<span data-ttu-id="e39b8-109">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="e39b8-109">ratingIrelandMoviesType</span></span>](../resources/intune_deviceconfig_ratingirelandmoviestype.md)|<span data-ttu-id="e39b8-110">分级爱尔兰的所选的影片。</span><span class="sxs-lookup"><span data-stu-id="e39b8-110">Movies rating selected for Ireland.</span></span> <span data-ttu-id="e39b8-111">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="e39b8-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="e39b8-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="e39b8-112">tvRating</span></span>|[<span data-ttu-id="e39b8-113">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e39b8-113">ratingIrelandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingirelandtelevisiontype.md)|<span data-ttu-id="e39b8-114">选择爱尔兰 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="e39b8-114">TV rating selected for Ireland.</span></span> <span data-ttu-id="e39b8-115">可取值为：`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature`。</span><span class="sxs-lookup"><span data-stu-id="e39b8-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e39b8-116">关系</span><span class="sxs-lookup"><span data-stu-id="e39b8-116">Relationships</span></span>
<span data-ttu-id="e39b8-117">无</span><span class="sxs-lookup"><span data-stu-id="e39b8-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e39b8-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e39b8-118">JSON Representation</span></span>
<span data-ttu-id="e39b8-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e39b8-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```



