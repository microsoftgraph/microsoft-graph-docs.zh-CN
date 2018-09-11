# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="7367d-101">mediaContentRatingAustralia 资源类型</span><span class="sxs-lookup"><span data-stu-id="7367d-101">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="7367d-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7367d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7367d-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7367d-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="7367d-104">属性</span><span class="sxs-lookup"><span data-stu-id="7367d-104">Properties</span></span>
|<span data-ttu-id="7367d-105">属性</span><span class="sxs-lookup"><span data-stu-id="7367d-105">Property</span></span>|<span data-ttu-id="7367d-106">类型</span><span class="sxs-lookup"><span data-stu-id="7367d-106">Type</span></span>|<span data-ttu-id="7367d-107">说明</span><span class="sxs-lookup"><span data-stu-id="7367d-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7367d-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="7367d-108">movieRating</span></span>|[<span data-ttu-id="7367d-109">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="7367d-109">ratingAustraliaMoviesType</span></span>](../resources/intune_deviceconfig_ratingaustraliamoviestype.md)|<span data-ttu-id="7367d-p101">为澳大利亚所选的影片分级。 可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="7367d-p101">Movies rating selected for Australia Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="7367d-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="7367d-112">tvRating</span></span>|[<span data-ttu-id="7367d-113">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="7367d-113">ratingAustraliaTelevisionType</span></span>](../resources/intune_deviceconfig_ratingaustraliatelevisiontype.md)|<span data-ttu-id="7367d-p102">为澳大利亚所选的电视分级。 可取值为：`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove15AdultViolence`。</span><span class="sxs-lookup"><span data-stu-id="7367d-p102">TV rating selected for Australia Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7367d-116">关系</span><span class="sxs-lookup"><span data-stu-id="7367d-116">Relationships</span></span>
<span data-ttu-id="7367d-117">无</span><span class="sxs-lookup"><span data-stu-id="7367d-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7367d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7367d-118">JSON Representation</span></span>
<span data-ttu-id="7367d-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7367d-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```








