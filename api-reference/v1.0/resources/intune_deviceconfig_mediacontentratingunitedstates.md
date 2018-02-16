# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="9fce6-101">mediaContentRatingUnitedStates 资源类型</span><span class="sxs-lookup"><span data-stu-id="9fce6-101">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="9fce6-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9fce6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9fce6-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9fce6-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="9fce6-104">属性</span><span class="sxs-lookup"><span data-stu-id="9fce6-104">Properties</span></span>
|<span data-ttu-id="9fce6-105">属性</span><span class="sxs-lookup"><span data-stu-id="9fce6-105">Property</span></span>|<span data-ttu-id="9fce6-106">类型</span><span class="sxs-lookup"><span data-stu-id="9fce6-106">Type</span></span>|<span data-ttu-id="9fce6-107">说明</span><span class="sxs-lookup"><span data-stu-id="9fce6-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fce6-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="9fce6-108">movieRating</span></span>|<span data-ttu-id="9fce6-109">String</span><span class="sxs-lookup"><span data-stu-id="9fce6-109">String</span></span>|<span data-ttu-id="9fce6-110">为美国选择的电影评级可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="9fce6-110">Movies rating selected for United States Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="9fce6-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="9fce6-111">tvRating</span></span>|<span data-ttu-id="9fce6-112">String</span><span class="sxs-lookup"><span data-stu-id="9fce6-112">String</span></span>|<span data-ttu-id="9fce6-113">为美国选择的电视评级可取值为：`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="9fce6-113">TV rating selected for United States Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fce6-114">关系</span><span class="sxs-lookup"><span data-stu-id="9fce6-114">Relationships</span></span>
<span data-ttu-id="9fce6-115">无</span><span class="sxs-lookup"><span data-stu-id="9fce6-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9fce6-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9fce6-116">JSON Representation</span></span>
<span data-ttu-id="9fce6-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9fce6-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



