# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="c7e53-101">mediaContentRatingIreland 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7e53-101">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="c7e53-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c7e53-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7e53-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c7e53-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c7e53-104">属性</span><span class="sxs-lookup"><span data-stu-id="c7e53-104">Properties</span></span>
|<span data-ttu-id="c7e53-105">属性</span><span class="sxs-lookup"><span data-stu-id="c7e53-105">Property</span></span>|<span data-ttu-id="c7e53-106">类型</span><span class="sxs-lookup"><span data-stu-id="c7e53-106">Type</span></span>|<span data-ttu-id="c7e53-107">说明</span><span class="sxs-lookup"><span data-stu-id="c7e53-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7e53-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="c7e53-108">movieRating</span></span>|[<span data-ttu-id="c7e53-109">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="c7e53-109">ratingIrelandMoviesType</span></span>](../resources/intune_deviceconfig_ratingirelandmoviestype.md)|<span data-ttu-id="c7e53-110">为爱尔兰选择的电影评级。</span><span class="sxs-lookup"><span data-stu-id="c7e53-110">Movies rating selected for Ireland Possible values are: , , , , , , , .</span></span> <span data-ttu-id="c7e53-111">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove12`、`agesAbove15`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="c7e53-111">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`, , , , or .</span></span>|
|<span data-ttu-id="c7e53-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="c7e53-112">tvRating</span></span>|[<span data-ttu-id="c7e53-113">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c7e53-113">ratingIrelandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingirelandtelevisiontype.md)|<span data-ttu-id="c7e53-114">为爱尔兰选择的 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="c7e53-114">TV rating selected for Ireland Possible values are: , , , , , , .</span></span> <span data-ttu-id="c7e53-115">可取值为：`allAllowed`、`allBlocked`、`general`、`children`、`youngAdults`、`parentalSupervision`、`mature`。</span><span class="sxs-lookup"><span data-stu-id="c7e53-115">The possible values are `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`, , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7e53-116">关系</span><span class="sxs-lookup"><span data-stu-id="c7e53-116">Relationships</span></span>
<span data-ttu-id="c7e53-117">无</span><span class="sxs-lookup"><span data-stu-id="c7e53-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c7e53-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7e53-118">JSON Representation</span></span>
<span data-ttu-id="c7e53-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7e53-119">Here is a JSON representation of the resource.</span></span>
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



