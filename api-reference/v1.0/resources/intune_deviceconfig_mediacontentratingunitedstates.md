# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="c6646-101">mediaContentRatingUnitedStates 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6646-101">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="c6646-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c6646-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6646-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c6646-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c6646-104">属性</span><span class="sxs-lookup"><span data-stu-id="c6646-104">Properties</span></span>
|<span data-ttu-id="c6646-105">属性</span><span class="sxs-lookup"><span data-stu-id="c6646-105">Property</span></span>|<span data-ttu-id="c6646-106">类型</span><span class="sxs-lookup"><span data-stu-id="c6646-106">Type</span></span>|<span data-ttu-id="c6646-107">说明</span><span class="sxs-lookup"><span data-stu-id="c6646-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6646-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="c6646-108">movieRating</span></span>|[<span data-ttu-id="c6646-109">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="c6646-109">ratingUnitedStatesMoviesType</span></span>](../resources/intune_deviceconfig_ratingunitedstatesmoviestype.md)|<span data-ttu-id="c6646-110">为美国所选的影片分级。</span><span class="sxs-lookup"><span data-stu-id="c6646-110">Movies rating selected for United States Possible values are: , , , , , , .</span></span> <span data-ttu-id="c6646-111">可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="c6646-111">The possible values are `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`, , , , , or .</span></span>|
|<span data-ttu-id="c6646-112">tvRating</span><span class="sxs-lookup"><span data-stu-id="c6646-112">tvRating</span></span>|[<span data-ttu-id="c6646-113">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c6646-113">ratingUnitedStatesTelevisionType</span></span>](../resources/intune_deviceconfig_ratingunitedstatestelevisiontype.md)|<span data-ttu-id="c6646-114">为美国所选的电视分级。</span><span class="sxs-lookup"><span data-stu-id="c6646-114">TV rating selected for United States Possible values are: , , , , , , , .</span></span> <span data-ttu-id="c6646-115">可取值为：`allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`。</span><span class="sxs-lookup"><span data-stu-id="c6646-115">The possible values are `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`, , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6646-116">关系</span><span class="sxs-lookup"><span data-stu-id="c6646-116">Relationships</span></span>
<span data-ttu-id="c6646-117">无</span><span class="sxs-lookup"><span data-stu-id="c6646-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c6646-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6646-118">JSON Representation</span></span>
<span data-ttu-id="c6646-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6646-119">Here is a JSON representation of the resource.</span></span>
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



