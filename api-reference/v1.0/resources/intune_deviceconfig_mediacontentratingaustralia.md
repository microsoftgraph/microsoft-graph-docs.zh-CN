# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="cf23e-101">mediaContentRatingAustralia 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf23e-101">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="cf23e-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cf23e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf23e-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cf23e-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="cf23e-104">属性</span><span class="sxs-lookup"><span data-stu-id="cf23e-104">Properties</span></span>
|<span data-ttu-id="cf23e-105">属性</span><span class="sxs-lookup"><span data-stu-id="cf23e-105">Property</span></span>|<span data-ttu-id="cf23e-106">类型</span><span class="sxs-lookup"><span data-stu-id="cf23e-106">Type</span></span>|<span data-ttu-id="cf23e-107">说明</span><span class="sxs-lookup"><span data-stu-id="cf23e-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf23e-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="cf23e-108">movieRating</span></span>|[<span data-ttu-id="cf23e-109">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="cf23e-109">ratingAustraliaMoviesType</span></span>](../resources/intune_deviceconfig_ratingaustraliamoviestype.md)|<span data-ttu-id="cf23e-110">为澳大利亚所选的影片分级。</span><span class="sxs-lookup"><span data-stu-id="cf23e-110">Movies rating selected for Australia Possible values are: , , , , , , .</span></span> <span data-ttu-id="cf23e-111">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="cf23e-111">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`, , , , , or .</span></span>|
|<span data-ttu-id="cf23e-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="cf23e-112">tvRating</span></span>|[<span data-ttu-id="cf23e-113">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="cf23e-113">ratingAustraliaTelevisionType</span></span>](../resources/intune_deviceconfig_ratingaustraliatelevisiontype.md)|<span data-ttu-id="cf23e-114">为澳大利亚所选的电视分级。</span><span class="sxs-lookup"><span data-stu-id="cf23e-114">TV rating selected for Australia Possible values are: , , , , , , , , .</span></span> <span data-ttu-id="cf23e-115">可取值为：`allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`。</span><span class="sxs-lookup"><span data-stu-id="cf23e-115">The possible values are `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`, , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf23e-116">关系</span><span class="sxs-lookup"><span data-stu-id="cf23e-116">Relationships</span></span>
<span data-ttu-id="cf23e-117">无</span><span class="sxs-lookup"><span data-stu-id="cf23e-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cf23e-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf23e-118">JSON Representation</span></span>
<span data-ttu-id="cf23e-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf23e-119">Here is a JSON representation of the resource.</span></span>
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



