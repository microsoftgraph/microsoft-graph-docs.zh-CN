# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="4c384-101">mediaContentRatingUnitedKingdom 资源类型</span><span class="sxs-lookup"><span data-stu-id="4c384-101">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="4c384-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4c384-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c384-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4c384-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="4c384-104">属性</span><span class="sxs-lookup"><span data-stu-id="4c384-104">Properties</span></span>
|<span data-ttu-id="4c384-105">属性</span><span class="sxs-lookup"><span data-stu-id="4c384-105">Property</span></span>|<span data-ttu-id="4c384-106">类型</span><span class="sxs-lookup"><span data-stu-id="4c384-106">Type</span></span>|<span data-ttu-id="4c384-107">说明</span><span class="sxs-lookup"><span data-stu-id="4c384-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c384-108">movieRating</span><span class="sxs-lookup"><span data-stu-id="4c384-108">movieRating</span></span>|<span data-ttu-id="4c384-109">String</span><span class="sxs-lookup"><span data-stu-id="4c384-109">String</span></span>|<span data-ttu-id="4c384-110">为英国选择的电影评级可取值为：`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15``adults`。</span><span class="sxs-lookup"><span data-stu-id="4c384-110">Movies rating selected for United Kingdom Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="4c384-111">tvRating</span><span class="sxs-lookup"><span data-stu-id="4c384-111">tvRating</span></span>|<span data-ttu-id="4c384-112">String</span><span class="sxs-lookup"><span data-stu-id="4c384-112">String</span></span>|<span data-ttu-id="4c384-113">为英国选择的电视评级可取值为：`allAllowed`、`allBlocked`、`caution`。</span><span class="sxs-lookup"><span data-stu-id="4c384-113">TV rating selected for United Kingdom Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c384-114">关系</span><span class="sxs-lookup"><span data-stu-id="4c384-114">Relationships</span></span>
<span data-ttu-id="4c384-115">无</span><span class="sxs-lookup"><span data-stu-id="4c384-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4c384-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4c384-116">JSON Representation</span></span>
<span data-ttu-id="4c384-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c384-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```



