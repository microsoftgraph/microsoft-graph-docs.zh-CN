# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="2e095-101">mediaContentRatingUnitedStates 资源类型</span><span class="sxs-lookup"><span data-stu-id="2e095-101">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="2e095-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2e095-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e095-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2e095-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="2e095-104">属性</span><span class="sxs-lookup"><span data-stu-id="2e095-104">Properties</span></span>
|<span data-ttu-id="2e095-105">属性</span><span class="sxs-lookup"><span data-stu-id="2e095-105">Property</span></span>|<span data-ttu-id="2e095-106">类型</span><span class="sxs-lookup"><span data-stu-id="2e095-106">Type</span></span>|<span data-ttu-id="2e095-107">说明</span><span class="sxs-lookup"><span data-stu-id="2e095-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e095-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="2e095-108">movieRating</span></span>|[<span data-ttu-id="2e095-109">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="2e095-109">ratingUnitedStatesMoviesType</span></span>](../resources/intune_deviceconfig_ratingunitedstatesmoviestype.md)|<span data-ttu-id="2e095-110">分级美国的所选的影片。</span><span class="sxs-lookup"><span data-stu-id="2e095-110">Movies rating selected for United States.</span></span> <span data-ttu-id="2e095-111">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="2e095-111">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="2e095-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="2e095-112">tvRating</span></span>|[<span data-ttu-id="2e095-113">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="2e095-113">ratingUnitedStatesTelevisionType</span></span>](../resources/intune_deviceconfig_ratingunitedstatestelevisiontype.md)|<span data-ttu-id="2e095-114">美国的所选 TV 分级。</span><span class="sxs-lookup"><span data-stu-id="2e095-114">TV rating selected for United States.</span></span> <span data-ttu-id="2e095-115">可取值为：`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="2e095-115">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e095-116">关系</span><span class="sxs-lookup"><span data-stu-id="2e095-116">Relationships</span></span>
<span data-ttu-id="2e095-117">无</span><span class="sxs-lookup"><span data-stu-id="2e095-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2e095-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2e095-118">JSON Representation</span></span>
<span data-ttu-id="2e095-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e095-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```



