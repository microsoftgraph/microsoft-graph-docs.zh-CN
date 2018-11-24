# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="5c931-101">mediaContentRatingJapan 资源类型</span><span class="sxs-lookup"><span data-stu-id="5c931-101">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="5c931-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5c931-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c931-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5c931-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="5c931-104">属性</span><span class="sxs-lookup"><span data-stu-id="5c931-104">Properties</span></span>
|<span data-ttu-id="5c931-105">属性</span><span class="sxs-lookup"><span data-stu-id="5c931-105">Property</span></span>|<span data-ttu-id="5c931-106">类型</span><span class="sxs-lookup"><span data-stu-id="5c931-106">Type</span></span>|<span data-ttu-id="5c931-107">说明</span><span class="sxs-lookup"><span data-stu-id="5c931-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c931-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="5c931-108">movieRating</span></span>|[<span data-ttu-id="5c931-109">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="5c931-109">ratingJapanMoviesType</span></span>](../resources/intune_deviceconfig_ratingjapanmoviestype.md)|<span data-ttu-id="5c931-110">分级日本所选的影片。</span><span class="sxs-lookup"><span data-stu-id="5c931-110">Movies rating selected for Japan.</span></span> <span data-ttu-id="5c931-111">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="5c931-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="5c931-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="5c931-112">tvRating</span></span>|[<span data-ttu-id="5c931-113">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="5c931-113">ratingJapanTelevisionType</span></span>](../resources/intune_deviceconfig_ratingjapantelevisiontype.md)|<span data-ttu-id="5c931-114">日本选择 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="5c931-114">TV rating selected for Japan.</span></span> <span data-ttu-id="5c931-115">可取值为：`allAllowed`、`allBlocked`、`explicitAllowed`。</span><span class="sxs-lookup"><span data-stu-id="5c931-115">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c931-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="5c931-116">Relationships</span></span>
<span data-ttu-id="5c931-117">无</span><span class="sxs-lookup"><span data-stu-id="5c931-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5c931-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c931-118">JSON Representation</span></span>
<span data-ttu-id="5c931-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c931-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```



