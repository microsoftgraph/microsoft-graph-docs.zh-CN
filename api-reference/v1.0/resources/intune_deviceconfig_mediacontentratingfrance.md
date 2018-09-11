# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="708f9-101">mediaContentRatingFrance 资源类型</span><span class="sxs-lookup"><span data-stu-id="708f9-101">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="708f9-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="708f9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="708f9-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="708f9-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="708f9-104">属性</span><span class="sxs-lookup"><span data-stu-id="708f9-104">Properties</span></span>
|<span data-ttu-id="708f9-105">属性</span><span class="sxs-lookup"><span data-stu-id="708f9-105">Property</span></span>|<span data-ttu-id="708f9-106">类型</span><span class="sxs-lookup"><span data-stu-id="708f9-106">Type</span></span>|<span data-ttu-id="708f9-107">说明</span><span class="sxs-lookup"><span data-stu-id="708f9-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="708f9-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="708f9-108">movieRating</span></span>|[<span data-ttu-id="708f9-109">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="708f9-109">ratingFranceMoviesType</span></span>](../resources/intune_deviceconfig_ratingfrancemoviestype.md)|<span data-ttu-id="708f9-p101">为法国所选的影片分级。 可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="708f9-p101">Movies rating selected for France Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="708f9-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="708f9-112">tvRating</span></span>|[<span data-ttu-id="708f9-113">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="708f9-113">ratingFranceTelevisionType</span></span>](../resources/intune_deviceconfig_ratingfrancetelevisiontype.md)|<span data-ttu-id="708f9-p102">为法国所选的电视分级。 可取值为：`allAllowed`、`allBlocked`、`agesAbove10`、`agesAbove12`、`agesAbove16`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="708f9-p102">TV rating selected for France Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="708f9-116">关系</span><span class="sxs-lookup"><span data-stu-id="708f9-116">Relationships</span></span>
<span data-ttu-id="708f9-117">无</span><span class="sxs-lookup"><span data-stu-id="708f9-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="708f9-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="708f9-118">JSON Representation</span></span>
<span data-ttu-id="708f9-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="708f9-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```








