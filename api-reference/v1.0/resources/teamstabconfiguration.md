# <a name="teamstabconfiguration-resource-type-open-type"></a><span data-ttu-id="52dec-101">teamsTabConfiguration 资源类型 （打开类型）</span><span class="sxs-lookup"><span data-stu-id="52dec-101">teamsTabConfiguration resource type (Open Type)</span></span>



<span data-ttu-id="52dec-102">确定内容的[选项卡上](teamstab.md)的设置。选项卡以交互方式配置时，此信息由选项卡提供程序应用程序设置。</span><span class="sxs-lookup"><span data-stu-id="52dec-102">The settings that determine the content of a [tab](teamstab.md). When a tab is interactively configured, this information is set by the tab provider application.</span></span>
<span data-ttu-id="52dec-103">除了下面的属性中，某些选项卡提供程序应用程序指定其他自定义属性。</span><span class="sxs-lookup"><span data-stu-id="52dec-103">In addition to the properties below, some tab provider applications specify additional custom properties.</span></span>

## <a name="properties"></a><span data-ttu-id="52dec-104">属性</span><span class="sxs-lookup"><span data-stu-id="52dec-104">Properties</span></span>

|<span data-ttu-id="52dec-105">属性</span><span class="sxs-lookup"><span data-stu-id="52dec-105">Property</span></span>|<span data-ttu-id="52dec-106">类型</span><span class="sxs-lookup"><span data-stu-id="52dec-106">Type</span></span>|<span data-ttu-id="52dec-107">说明</span><span class="sxs-lookup"><span data-stu-id="52dec-107">Description</span></span>|
|-|-|-|
|  <span data-ttu-id="52dec-108">entityId</span><span class="sxs-lookup"><span data-stu-id="52dec-108">entityId</span></span>   |   <span data-ttu-id="52dec-109">string</span><span class="sxs-lookup"><span data-stu-id="52dec-109">string</span></span> |  <span data-ttu-id="52dec-110">选项卡上的服务提供商托管实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="52dec-110">Identifier for the entity hosted by the tab provider.</span></span>     |
|  <span data-ttu-id="52dec-111">contentUrl</span><span class="sxs-lookup"><span data-stu-id="52dec-111">contentUrl</span></span> |   <span data-ttu-id="52dec-112">string</span><span class="sxs-lookup"><span data-stu-id="52dec-112">string</span></span> |  <span data-ttu-id="52dec-113">用于呈现团队中的选项卡内容的 Url。</span><span class="sxs-lookup"><span data-stu-id="52dec-113">Url used for rendering tab contents in Teams.</span></span> <span data-ttu-id="52dec-114">必需。</span><span class="sxs-lookup"><span data-stu-id="52dec-114">Required.</span></span>    |
|  <span data-ttu-id="52dec-115">removeUrl</span><span class="sxs-lookup"><span data-stu-id="52dec-115">removeUrl</span></span>  |   <span data-ttu-id="52dec-116">string</span><span class="sxs-lookup"><span data-stu-id="52dec-116">string</span></span> |  <span data-ttu-id="52dec-117">使用团队客户端中移除一个选项卡时调用团队客户端的 Url。</span><span class="sxs-lookup"><span data-stu-id="52dec-117">Url called by Teams client when a Tab is removed using the Teams Client.</span></span>     |
|  <span data-ttu-id="52dec-118">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="52dec-118">websiteUrl</span></span> |   <span data-ttu-id="52dec-119">string</span><span class="sxs-lookup"><span data-stu-id="52dec-119">string</span></span> |  <span data-ttu-id="52dec-120">显示选项卡团队之外的内容的 Url。</span><span class="sxs-lookup"><span data-stu-id="52dec-120">Url for showing tab contents outside of Teams.</span></span>     |

## <a name="json-representation"></a><span data-ttu-id="52dec-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52dec-121">JSON representation</span></span>

<span data-ttu-id="52dec-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52dec-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTabConfiguration"
}-->

```json
{
   "entityId": "string",
   "contentUrl": "string (HTTPS Url)",
   "websiteUrl": "string (HTTPS Url)",
   "removeUrl": "string (HTTPS Url)"  
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
