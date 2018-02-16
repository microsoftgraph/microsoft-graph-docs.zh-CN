# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="79bf1-101">mediaContentRatingNewZealand 资源类型</span><span class="sxs-lookup"><span data-stu-id="79bf1-101">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="79bf1-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="79bf1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79bf1-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="79bf1-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="79bf1-104">属性</span><span class="sxs-lookup"><span data-stu-id="79bf1-104">Properties</span></span>
|<span data-ttu-id="79bf1-105">属性</span><span class="sxs-lookup"><span data-stu-id="79bf1-105">Property</span></span>|<span data-ttu-id="79bf1-106">类型</span><span class="sxs-lookup"><span data-stu-id="79bf1-106">Type</span></span>|<span data-ttu-id="79bf1-107">说明</span><span class="sxs-lookup"><span data-stu-id="79bf1-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79bf1-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="79bf1-108">movieRating</span></span>|<span data-ttu-id="79bf1-109">String</span><span class="sxs-lookup"><span data-stu-id="79bf1-109">String</span></span>|<span data-ttu-id="79bf1-110">为新西兰选择的电影评级可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16``agesAbove18``restricted``agesAbove16Restricted`。</span><span class="sxs-lookup"><span data-stu-id="79bf1-110">Movies rating selected for New Zealand Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="79bf1-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="79bf1-111">tvRating</span></span>|<span data-ttu-id="79bf1-112">String</span><span class="sxs-lookup"><span data-stu-id="79bf1-112">String</span></span>|<span data-ttu-id="79bf1-113">为新西兰选择的电视评级可取值为：`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults`。</span><span class="sxs-lookup"><span data-stu-id="79bf1-113">TV rating selected for New Zealand Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79bf1-114">关系</span><span class="sxs-lookup"><span data-stu-id="79bf1-114">Relationships</span></span>
<span data-ttu-id="79bf1-115">无</span><span class="sxs-lookup"><span data-stu-id="79bf1-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="79bf1-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="79bf1-116">JSON Representation</span></span>
<span data-ttu-id="79bf1-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79bf1-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



