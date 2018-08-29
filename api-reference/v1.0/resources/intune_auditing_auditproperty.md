# <a name="auditproperty-resource-type"></a><span data-ttu-id="2be04-101">auditProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="2be04-101">auditProperty resource type</span></span>

> <span data-ttu-id="2be04-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2be04-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2be04-103">包含审核属性的属性的类。</span><span class="sxs-lookup"><span data-stu-id="2be04-103">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="2be04-104">属性</span><span class="sxs-lookup"><span data-stu-id="2be04-104">Properties</span></span>
|<span data-ttu-id="2be04-105">属性</span><span class="sxs-lookup"><span data-stu-id="2be04-105">Property</span></span>|<span data-ttu-id="2be04-106">类型</span><span class="sxs-lookup"><span data-stu-id="2be04-106">Type</span></span>|<span data-ttu-id="2be04-107">说明</span><span class="sxs-lookup"><span data-stu-id="2be04-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2be04-108">displayName</span><span class="sxs-lookup"><span data-stu-id="2be04-108">displayName</span></span>|<span data-ttu-id="2be04-109">String</span><span class="sxs-lookup"><span data-stu-id="2be04-109">String</span></span>|<span data-ttu-id="2be04-110">显示名称。</span><span class="sxs-lookup"><span data-stu-id="2be04-110">Display name.</span></span>|
|<span data-ttu-id="2be04-111">oldValue</span><span class="sxs-lookup"><span data-stu-id="2be04-111">oldValue</span></span>|<span data-ttu-id="2be04-112">String</span><span class="sxs-lookup"><span data-stu-id="2be04-112">String</span></span>|<span data-ttu-id="2be04-113">旧值。</span><span class="sxs-lookup"><span data-stu-id="2be04-113">Old value.</span></span>|
|<span data-ttu-id="2be04-114">NewValue</span><span class="sxs-lookup"><span data-stu-id="2be04-114">newValue</span></span>|<span data-ttu-id="2be04-115">String</span><span class="sxs-lookup"><span data-stu-id="2be04-115">String</span></span>|<span data-ttu-id="2be04-116">新值。</span><span class="sxs-lookup"><span data-stu-id="2be04-116">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2be04-117">关系</span><span class="sxs-lookup"><span data-stu-id="2be04-117">Relationships</span></span>
<span data-ttu-id="2be04-118">无</span><span class="sxs-lookup"><span data-stu-id="2be04-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2be04-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2be04-119">JSON Representation</span></span>
<span data-ttu-id="2be04-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2be04-120">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```



