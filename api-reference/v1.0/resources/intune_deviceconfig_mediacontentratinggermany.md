# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="2a19a-101">mediaContentRatingGermany 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a19a-101">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="2a19a-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2a19a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a19a-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2a19a-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="2a19a-104">属性</span><span class="sxs-lookup"><span data-stu-id="2a19a-104">Properties</span></span>
|<span data-ttu-id="2a19a-105">属性</span><span class="sxs-lookup"><span data-stu-id="2a19a-105">Property</span></span>|<span data-ttu-id="2a19a-106">类型</span><span class="sxs-lookup"><span data-stu-id="2a19a-106">Type</span></span>|<span data-ttu-id="2a19a-107">说明</span><span class="sxs-lookup"><span data-stu-id="2a19a-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a19a-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="2a19a-108">movieRating</span></span>|[<span data-ttu-id="2a19a-109">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="2a19a-109">ratingGermanyMoviesType</span></span>](../resources/intune_deviceconfig_ratinggermanymoviestype.md)|<span data-ttu-id="2a19a-110">分级德国所选的影片。</span><span class="sxs-lookup"><span data-stu-id="2a19a-110">Movies rating selected for Germany.</span></span> <span data-ttu-id="2a19a-111">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="2a19a-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="2a19a-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="2a19a-112">tvRating</span></span>|[<span data-ttu-id="2a19a-113">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="2a19a-113">ratingGermanyTelevisionType</span></span>](../resources/intune_deviceconfig_ratinggermanytelevisiontype.md)|<span data-ttu-id="2a19a-114">德国选择 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="2a19a-114">TV rating selected for Germany.</span></span> <span data-ttu-id="2a19a-115">可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="2a19a-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a19a-116">关系</span><span class="sxs-lookup"><span data-stu-id="2a19a-116">Relationships</span></span>
<span data-ttu-id="2a19a-117">无</span><span class="sxs-lookup"><span data-stu-id="2a19a-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2a19a-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a19a-118">JSON Representation</span></span>
<span data-ttu-id="2a19a-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a19a-119">Here is a JSON representation of the resource.</span></span>
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



