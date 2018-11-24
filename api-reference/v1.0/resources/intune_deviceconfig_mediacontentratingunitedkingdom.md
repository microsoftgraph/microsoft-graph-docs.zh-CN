# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="c26cd-101">mediaContentRatingUnitedKingdom 资源类型</span><span class="sxs-lookup"><span data-stu-id="c26cd-101">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="c26cd-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c26cd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c26cd-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c26cd-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c26cd-104">属性</span><span class="sxs-lookup"><span data-stu-id="c26cd-104">Properties</span></span>
|<span data-ttu-id="c26cd-105">属性</span><span class="sxs-lookup"><span data-stu-id="c26cd-105">Property</span></span>|<span data-ttu-id="c26cd-106">类型</span><span class="sxs-lookup"><span data-stu-id="c26cd-106">Type</span></span>|<span data-ttu-id="c26cd-107">说明</span><span class="sxs-lookup"><span data-stu-id="c26cd-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c26cd-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="c26cd-108">movieRating</span></span>|[<span data-ttu-id="c26cd-109">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="c26cd-109">ratingUnitedKingdomMoviesType</span></span>](../resources/intune_deviceconfig_ratingunitedkingdommoviestype.md)|<span data-ttu-id="c26cd-110">分级英国的所选的影片。</span><span class="sxs-lookup"><span data-stu-id="c26cd-110">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="c26cd-111">可取值为：`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="c26cd-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="c26cd-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="c26cd-112">tvRating</span></span>|[<span data-ttu-id="c26cd-113">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c26cd-113">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune_deviceconfig_ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="c26cd-114">选定用于英国 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="c26cd-114">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="c26cd-115">可取值为：`allAllowed`、`allBlocked`、`caution`。</span><span class="sxs-lookup"><span data-stu-id="c26cd-115">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c26cd-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="c26cd-116">Relationships</span></span>
<span data-ttu-id="c26cd-117">无</span><span class="sxs-lookup"><span data-stu-id="c26cd-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c26cd-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c26cd-118">JSON Representation</span></span>
<span data-ttu-id="c26cd-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c26cd-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```



