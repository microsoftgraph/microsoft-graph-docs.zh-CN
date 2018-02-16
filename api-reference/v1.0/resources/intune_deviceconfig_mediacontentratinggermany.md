# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="6d4a2-101">mediaContentRatingGermany 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d4a2-101">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="6d4a2-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6d4a2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d4a2-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6d4a2-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="6d4a2-104">属性</span><span class="sxs-lookup"><span data-stu-id="6d4a2-104">Properties</span></span>
|<span data-ttu-id="6d4a2-105">属性</span><span class="sxs-lookup"><span data-stu-id="6d4a2-105">Property</span></span>|<span data-ttu-id="6d4a2-106">类型</span><span class="sxs-lookup"><span data-stu-id="6d4a2-106">Type</span></span>|<span data-ttu-id="6d4a2-107">说明</span><span class="sxs-lookup"><span data-stu-id="6d4a2-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d4a2-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="6d4a2-108">movieRating</span></span>|<span data-ttu-id="6d4a2-109">String</span><span class="sxs-lookup"><span data-stu-id="6d4a2-109">String</span></span>|<span data-ttu-id="6d4a2-110">为德国选择的电影评级可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="6d4a2-110">Movies rating selected for Germany Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="6d4a2-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="6d4a2-111">tvRating</span></span>|<span data-ttu-id="6d4a2-112">String</span><span class="sxs-lookup"><span data-stu-id="6d4a2-112">String</span></span>|<span data-ttu-id="6d4a2-113">为德国选择的电视评级可取值为：`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="6d4a2-113">TV rating selected for Germany Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d4a2-114">关系</span><span class="sxs-lookup"><span data-stu-id="6d4a2-114">Relationships</span></span>
<span data-ttu-id="6d4a2-115">无</span><span class="sxs-lookup"><span data-stu-id="6d4a2-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6d4a2-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d4a2-116">JSON Representation</span></span>
<span data-ttu-id="6d4a2-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d4a2-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```



