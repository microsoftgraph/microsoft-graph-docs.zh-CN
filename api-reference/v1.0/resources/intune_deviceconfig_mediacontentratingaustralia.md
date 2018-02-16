# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="ffd36-101">mediaContentRatingAustralia 资源类型</span><span class="sxs-lookup"><span data-stu-id="ffd36-101">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="ffd36-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ffd36-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ffd36-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ffd36-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="ffd36-104">属性</span><span class="sxs-lookup"><span data-stu-id="ffd36-104">Properties</span></span>
|<span data-ttu-id="ffd36-105">属性</span><span class="sxs-lookup"><span data-stu-id="ffd36-105">Property</span></span>|<span data-ttu-id="ffd36-106">类型</span><span class="sxs-lookup"><span data-stu-id="ffd36-106">Type</span></span>|<span data-ttu-id="ffd36-107">说明</span><span class="sxs-lookup"><span data-stu-id="ffd36-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffd36-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="ffd36-108">movieRating</span></span>|<span data-ttu-id="ffd36-109">String</span><span class="sxs-lookup"><span data-stu-id="ffd36-109">String</span></span>|<span data-ttu-id="ffd36-110">为澳大利亚选择的电影评级可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove15`、`agesAbove18`。</span><span class="sxs-lookup"><span data-stu-id="ffd36-110">Movies rating selected for Australia Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="ffd36-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="ffd36-111">tvRating</span></span>|<span data-ttu-id="ffd36-112">String</span><span class="sxs-lookup"><span data-stu-id="ffd36-112">String</span></span>|<span data-ttu-id="ffd36-113">为澳大利亚选择的电视评级可取值为：`allAllowed`、`allBlocked`、`preschoolers`、`children`、`general`、`parentalGuidance`、`mature`、`agesAbove15``agesAbove15AdultViolence`。</span><span class="sxs-lookup"><span data-stu-id="ffd36-113">TV rating selected for Australia Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffd36-114">关系</span><span class="sxs-lookup"><span data-stu-id="ffd36-114">Relationships</span></span>
<span data-ttu-id="ffd36-115">无</span><span class="sxs-lookup"><span data-stu-id="ffd36-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ffd36-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ffd36-116">JSON Representation</span></span>
<span data-ttu-id="ffd36-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ffd36-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



