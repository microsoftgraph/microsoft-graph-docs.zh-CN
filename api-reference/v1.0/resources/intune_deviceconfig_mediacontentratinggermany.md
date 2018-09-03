# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="6d839-101">mediaContentRatingGermany 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d839-101">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="6d839-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6d839-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d839-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6d839-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="6d839-104">属性</span><span class="sxs-lookup"><span data-stu-id="6d839-104">Properties</span></span>
|<span data-ttu-id="6d839-105">属性</span><span class="sxs-lookup"><span data-stu-id="6d839-105">Property</span></span>|<span data-ttu-id="6d839-106">类型</span><span class="sxs-lookup"><span data-stu-id="6d839-106">Type</span></span>|<span data-ttu-id="6d839-107">说明</span><span class="sxs-lookup"><span data-stu-id="6d839-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d839-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="6d839-108">movieRating</span></span>|[<span data-ttu-id="6d839-109">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="6d839-109">ratingGermanyMoviesType</span></span>](../resources/intune_deviceconfig_ratinggermanymoviestype.md)|<span data-ttu-id="6d839-110">为德国所选的影片分级。</span><span class="sxs-lookup"><span data-stu-id="6d839-110">Movies rating selected for Germany Possible values are: , , , , , , .</span></span> <span data-ttu-id="6d839-111">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="6d839-111">The possible values are `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`, , , , , or .</span></span>|
|<span data-ttu-id="6d839-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="6d839-112">tvRating</span></span>|[<span data-ttu-id="6d839-113">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="6d839-113">ratingGermanyTelevisionType</span></span>](../resources/intune_deviceconfig_ratinggermanytelevisiontype.md)|<span data-ttu-id="6d839-114">为德国所选的电视分级。</span><span class="sxs-lookup"><span data-stu-id="6d839-114">TV rating selected for Germany Possible values are: , , , , , , .</span></span> <span data-ttu-id="6d839-115">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="6d839-115">The possible values are `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`, , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d839-116">关系</span><span class="sxs-lookup"><span data-stu-id="6d839-116">Relationships</span></span>
<span data-ttu-id="6d839-117">无</span><span class="sxs-lookup"><span data-stu-id="6d839-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6d839-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d839-118">JSON Representation</span></span>
<span data-ttu-id="6d839-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d839-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```



