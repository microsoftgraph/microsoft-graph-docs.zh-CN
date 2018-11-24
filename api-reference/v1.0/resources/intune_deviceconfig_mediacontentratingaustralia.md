# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="13b4b-101">mediaContentRatingAustralia 资源类型</span><span class="sxs-lookup"><span data-stu-id="13b4b-101">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="13b4b-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="13b4b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13b4b-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="13b4b-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="13b4b-104">属性</span><span class="sxs-lookup"><span data-stu-id="13b4b-104">Properties</span></span>
|<span data-ttu-id="13b4b-105">属性</span><span class="sxs-lookup"><span data-stu-id="13b4b-105">Property</span></span>|<span data-ttu-id="13b4b-106">类型</span><span class="sxs-lookup"><span data-stu-id="13b4b-106">Type</span></span>|<span data-ttu-id="13b4b-107">说明</span><span class="sxs-lookup"><span data-stu-id="13b4b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13b4b-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="13b4b-108">movieRating</span></span>|[<span data-ttu-id="13b4b-109">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="13b4b-109">ratingAustraliaMoviesType</span></span>](../resources/intune_deviceconfig_ratingaustraliamoviestype.md)|<span data-ttu-id="13b4b-110">分级澳大利亚的所选的影片。</span><span class="sxs-lookup"><span data-stu-id="13b4b-110">Movies rating selected for Australia.</span></span> <span data-ttu-id="13b4b-111">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="13b4b-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="13b4b-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="13b4b-112">tvRating</span></span>|[<span data-ttu-id="13b4b-113">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="13b4b-113">ratingAustraliaTelevisionType</span></span>](../resources/intune_deviceconfig_ratingaustraliatelevisiontype.md)|<span data-ttu-id="13b4b-114">澳大利亚选择 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="13b4b-114">TV rating selected for Australia.</span></span> <span data-ttu-id="13b4b-115">可取值为：`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence`。</span><span class="sxs-lookup"><span data-stu-id="13b4b-115">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13b4b-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="13b4b-116">Relationships</span></span>
<span data-ttu-id="13b4b-117">无</span><span class="sxs-lookup"><span data-stu-id="13b4b-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="13b4b-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13b4b-118">JSON Representation</span></span>
<span data-ttu-id="13b4b-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13b4b-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```



