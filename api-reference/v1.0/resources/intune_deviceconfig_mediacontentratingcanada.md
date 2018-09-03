# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="27d52-101">mediaContentRatingCanada 资源类型</span><span class="sxs-lookup"><span data-stu-id="27d52-101">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="27d52-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="27d52-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27d52-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="27d52-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="27d52-104">属性</span><span class="sxs-lookup"><span data-stu-id="27d52-104">Properties</span></span>
|<span data-ttu-id="27d52-105">属性</span><span class="sxs-lookup"><span data-stu-id="27d52-105">Property</span></span>|<span data-ttu-id="27d52-106">类型</span><span class="sxs-lookup"><span data-stu-id="27d52-106">Type</span></span>|<span data-ttu-id="27d52-107">说明</span><span class="sxs-lookup"><span data-stu-id="27d52-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27d52-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="27d52-108">movieRating</span></span>|[<span data-ttu-id="27d52-109">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="27d52-109">ratingCanadaMoviesType</span></span>](../resources/intune_deviceconfig_ratingcanadamoviestype.md)|<span data-ttu-id="27d52-110">选定加拿大电影分级。</span><span class="sxs-lookup"><span data-stu-id="27d52-110">Movies rating selected for Canada Possible values are: , , , , , , .</span></span> <span data-ttu-id="27d52-111">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`、`restricted`。</span><span class="sxs-lookup"><span data-stu-id="27d52-111">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`, , , , , or .</span></span>|
|<span data-ttu-id="27d52-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="27d52-112">tvRating</span></span>|[<span data-ttu-id="27d52-113">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="27d52-113">ratingCanadaTelevisionType</span></span>](../resources/intune_deviceconfig_ratingcanadatelevisiontype.md)|<span data-ttu-id="27d52-114">选定加拿大电视分级。</span><span class="sxs-lookup"><span data-stu-id="27d52-114">TV rating selected for Canada Possible values are: , , , , , , , .</span></span> <span data-ttu-id="27d52-115">可取值为：`allAllowed`、`allBlocked`、`children`、`childrenAbove8`、`general`、`parentalGuidance`、`agesAbove14`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="27d52-115">The possible values are `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="27d52-116">关系</span><span class="sxs-lookup"><span data-stu-id="27d52-116">Relationships</span></span>
<span data-ttu-id="27d52-117">无</span><span class="sxs-lookup"><span data-stu-id="27d52-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="27d52-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="27d52-118">JSON Representation</span></span>
<span data-ttu-id="27d52-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27d52-119">Here is a JSON representation of the resource.</span></span>
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



