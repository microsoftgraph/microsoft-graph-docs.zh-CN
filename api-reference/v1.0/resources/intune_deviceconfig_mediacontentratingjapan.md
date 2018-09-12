# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="26cf3-101">mediaContentRatingJapan 资源类型</span><span class="sxs-lookup"><span data-stu-id="26cf3-101">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="26cf3-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="26cf3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26cf3-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="26cf3-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="26cf3-104">属性</span><span class="sxs-lookup"><span data-stu-id="26cf3-104">Properties</span></span>
|<span data-ttu-id="26cf3-105">属性</span><span class="sxs-lookup"><span data-stu-id="26cf3-105">Property</span></span>|<span data-ttu-id="26cf3-106">类型</span><span class="sxs-lookup"><span data-stu-id="26cf3-106">Type</span></span>|<span data-ttu-id="26cf3-107">说明</span><span class="sxs-lookup"><span data-stu-id="26cf3-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26cf3-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="26cf3-108">movieRating</span></span>|[<span data-ttu-id="26cf3-109">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="26cf3-109">ratingJapanMoviesType</span></span>](../resources/intune_deviceconfig_ratingjapanmoviestype.md)|<span data-ttu-id="26cf3-110">为日本选定的影片分级。</span><span class="sxs-lookup"><span data-stu-id="26cf3-110">Movies rating selected for Japan Possible values are: , , , , , .</span></span> <span data-ttu-id="26cf3-111">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="26cf3-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="26cf3-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="26cf3-112">tvRating</span></span>|[<span data-ttu-id="26cf3-113">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="26cf3-113">ratingJapanTelevisionType</span></span>](../resources/intune_deviceconfig_ratingjapantelevisiontype.md)|<span data-ttu-id="26cf3-114">为日本选定的电视分级。</span><span class="sxs-lookup"><span data-stu-id="26cf3-114">TV rating selected for Japan Possible values are: , , .</span></span> <span data-ttu-id="26cf3-115">可取值为：`allAllowed`、`allBlocked`、`explicitAllowed`。</span><span class="sxs-lookup"><span data-stu-id="26cf3-115">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26cf3-116">关系</span><span class="sxs-lookup"><span data-stu-id="26cf3-116">Relationships</span></span>
<span data-ttu-id="26cf3-117">无</span><span class="sxs-lookup"><span data-stu-id="26cf3-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="26cf3-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26cf3-118">JSON Representation</span></span>
<span data-ttu-id="26cf3-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26cf3-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```








