# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="b8b53-101">mediaContentRatingCanada 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8b53-101">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="b8b53-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b8b53-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8b53-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b8b53-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="b8b53-104">属性</span><span class="sxs-lookup"><span data-stu-id="b8b53-104">Properties</span></span>
|<span data-ttu-id="b8b53-105">属性</span><span class="sxs-lookup"><span data-stu-id="b8b53-105">Property</span></span>|<span data-ttu-id="b8b53-106">类型</span><span class="sxs-lookup"><span data-stu-id="b8b53-106">Type</span></span>|<span data-ttu-id="b8b53-107">说明</span><span class="sxs-lookup"><span data-stu-id="b8b53-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8b53-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="b8b53-108">movieRating</span></span>|[<span data-ttu-id="b8b53-109">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="b8b53-109">ratingCanadaMoviesType</span></span>](../resources/intune_deviceconfig_ratingcanadamoviestype.md)|<span data-ttu-id="b8b53-p101">为加拿大选择的电影分级。 可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`、`restricted`。</span><span class="sxs-lookup"><span data-stu-id="b8b53-p101">Movies rating selected for Canada Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="b8b53-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="b8b53-112">tvRating</span></span>|[<span data-ttu-id="b8b53-113">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b8b53-113">ratingCanadaTelevisionType</span></span>](../resources/intune_deviceconfig_ratingcanadatelevisiontype.md)|<span data-ttu-id="b8b53-p102">为加拿大选择的电视分级。可取值为：`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="b8b53-p102">TV rating selected for Canada Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8b53-116">关系</span><span class="sxs-lookup"><span data-stu-id="b8b53-116">Relationships</span></span>
<span data-ttu-id="b8b53-117">无</span><span class="sxs-lookup"><span data-stu-id="b8b53-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b8b53-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8b53-118">JSON Representation</span></span>
<span data-ttu-id="b8b53-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8b53-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```








