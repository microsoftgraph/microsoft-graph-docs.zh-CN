# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="4cf93-101">mediaContentRatingFrance 资源类型</span><span class="sxs-lookup"><span data-stu-id="4cf93-101">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="4cf93-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4cf93-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4cf93-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4cf93-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="4cf93-104">属性</span><span class="sxs-lookup"><span data-stu-id="4cf93-104">Properties</span></span>
|<span data-ttu-id="4cf93-105">属性</span><span class="sxs-lookup"><span data-stu-id="4cf93-105">Property</span></span>|<span data-ttu-id="4cf93-106">类型</span><span class="sxs-lookup"><span data-stu-id="4cf93-106">Type</span></span>|<span data-ttu-id="4cf93-107">说明</span><span class="sxs-lookup"><span data-stu-id="4cf93-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cf93-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="4cf93-108">movieRating</span></span>|[<span data-ttu-id="4cf93-109">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="4cf93-109">ratingFranceMoviesType</span></span>](../resources/intune_deviceconfig_ratingfrancemoviestype.md)|<span data-ttu-id="4cf93-110">为法国所选的影片分级。</span><span class="sxs-lookup"><span data-stu-id="4cf93-110">Movies rating selected for France Possible values are: , , , , , .</span></span> <span data-ttu-id="4cf93-111">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="4cf93-111">The possible values are `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`, , , , , , or .</span></span>|
|<span data-ttu-id="4cf93-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="4cf93-112">tvRating</span></span>|[<span data-ttu-id="4cf93-113">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="4cf93-113">ratingFranceTelevisionType</span></span>](../resources/intune_deviceconfig_ratingfrancetelevisiontype.md)|<span data-ttu-id="4cf93-114">为法国所选的电视分级。</span><span class="sxs-lookup"><span data-stu-id="4cf93-114">TV rating selected for France Possible values are: , , , , , .</span></span> <span data-ttu-id="4cf93-115">可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="4cf93-115">The possible values are `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`, , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="4cf93-116">关系</span><span class="sxs-lookup"><span data-stu-id="4cf93-116">Relationships</span></span>
<span data-ttu-id="4cf93-117">无</span><span class="sxs-lookup"><span data-stu-id="4cf93-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4cf93-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4cf93-118">JSON Representation</span></span>
<span data-ttu-id="4cf93-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4cf93-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```



