# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="7c391-101">mediaContentRatingCanada 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c391-101">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="7c391-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7c391-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7c391-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7c391-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="7c391-104">属性</span><span class="sxs-lookup"><span data-stu-id="7c391-104">Properties</span></span>
|<span data-ttu-id="7c391-105">属性</span><span class="sxs-lookup"><span data-stu-id="7c391-105">Property</span></span>|<span data-ttu-id="7c391-106">类型</span><span class="sxs-lookup"><span data-stu-id="7c391-106">Type</span></span>|<span data-ttu-id="7c391-107">说明</span><span class="sxs-lookup"><span data-stu-id="7c391-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c391-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="7c391-108">movieRating</span></span>|[<span data-ttu-id="7c391-109">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="7c391-109">ratingCanadaMoviesType</span></span>](../resources/intune_deviceconfig_ratingcanadamoviestype.md)|<span data-ttu-id="7c391-110">分级加拿大所选的影片。</span><span class="sxs-lookup"><span data-stu-id="7c391-110">Movies rating selected for Canada.</span></span> <span data-ttu-id="7c391-111">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`、`restricted`。</span><span class="sxs-lookup"><span data-stu-id="7c391-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="7c391-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="7c391-112">tvRating</span></span>|[<span data-ttu-id="7c391-113">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="7c391-113">ratingCanadaTelevisionType</span></span>](../resources/intune_deviceconfig_ratingcanadatelevisiontype.md)|<span data-ttu-id="7c391-114">选定用于加拿大 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="7c391-114">TV rating selected for Canada.</span></span> <span data-ttu-id="7c391-115">可取值为：`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="7c391-115">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c391-116">关系</span><span class="sxs-lookup"><span data-stu-id="7c391-116">Relationships</span></span>
<span data-ttu-id="7c391-117">无</span><span class="sxs-lookup"><span data-stu-id="7c391-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7c391-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c391-118">JSON Representation</span></span>
<span data-ttu-id="7c391-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c391-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```



