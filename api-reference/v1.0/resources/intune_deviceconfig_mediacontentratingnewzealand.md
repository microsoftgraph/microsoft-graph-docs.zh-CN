# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="14cc6-101">mediaContentRatingNewZealand 资源类型</span><span class="sxs-lookup"><span data-stu-id="14cc6-101">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="14cc6-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="14cc6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14cc6-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="14cc6-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="14cc6-104">属性</span><span class="sxs-lookup"><span data-stu-id="14cc6-104">Properties</span></span>
|<span data-ttu-id="14cc6-105">属性</span><span class="sxs-lookup"><span data-stu-id="14cc6-105">Property</span></span>|<span data-ttu-id="14cc6-106">类型</span><span class="sxs-lookup"><span data-stu-id="14cc6-106">Type</span></span>|<span data-ttu-id="14cc6-107">说明</span><span class="sxs-lookup"><span data-stu-id="14cc6-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14cc6-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="14cc6-108">movieRating</span></span>|[<span data-ttu-id="14cc6-109">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="14cc6-109">ratingNewZealandMoviesType</span></span>](../resources/intune_deviceconfig_ratingnewzealandmoviestype.md)|<span data-ttu-id="14cc6-110">分级新西兰所选的影片。</span><span class="sxs-lookup"><span data-stu-id="14cc6-110">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="14cc6-111">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted`。</span><span class="sxs-lookup"><span data-stu-id="14cc6-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="14cc6-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="14cc6-112">tvRating</span></span>|[<span data-ttu-id="14cc6-113">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="14cc6-113">ratingNewZealandTelevisionType</span></span>](../resources/intune_deviceconfig_ratingnewzealandtelevisiontype.md)|<span data-ttu-id="14cc6-114">选择新西兰 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="14cc6-114">TV rating selected for New Zealand.</span></span> <span data-ttu-id="14cc6-115">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="14cc6-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14cc6-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="14cc6-116">Relationships</span></span>
<span data-ttu-id="14cc6-117">无</span><span class="sxs-lookup"><span data-stu-id="14cc6-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="14cc6-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14cc6-118">JSON Representation</span></span>
<span data-ttu-id="14cc6-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14cc6-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```



