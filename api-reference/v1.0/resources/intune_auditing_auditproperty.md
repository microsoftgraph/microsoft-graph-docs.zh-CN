# <a name="auditproperty-resource-type"></a><span data-ttu-id="5a618-101">auditProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="5a618-101">auditProperty resource type</span></span>

> <span data-ttu-id="5a618-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5a618-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a618-103">包含审核属性的属性的类。</span><span class="sxs-lookup"><span data-stu-id="5a618-103">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="5a618-104">属性</span><span class="sxs-lookup"><span data-stu-id="5a618-104">Properties</span></span>
|<span data-ttu-id="5a618-105">属性</span><span class="sxs-lookup"><span data-stu-id="5a618-105">Property</span></span>|<span data-ttu-id="5a618-106">类型</span><span class="sxs-lookup"><span data-stu-id="5a618-106">Type</span></span>|<span data-ttu-id="5a618-107">说明</span><span class="sxs-lookup"><span data-stu-id="5a618-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a618-108">displayName</span><span class="sxs-lookup"><span data-stu-id="5a618-108">displayName</span></span>|<span data-ttu-id="5a618-109">String</span><span class="sxs-lookup"><span data-stu-id="5a618-109">String</span></span>|<span data-ttu-id="5a618-110">显示名称。</span><span class="sxs-lookup"><span data-stu-id="5a618-110">Display Name</span></span>|
|<span data-ttu-id="5a618-111">oldValue</span><span class="sxs-lookup"><span data-stu-id="5a618-111">OldValue</span></span>|<span data-ttu-id="5a618-112">String</span><span class="sxs-lookup"><span data-stu-id="5a618-112">String</span></span>|<span data-ttu-id="5a618-113">旧值。</span><span class="sxs-lookup"><span data-stu-id="5a618-113">Old value.</span></span>|
|<span data-ttu-id="5a618-114">NewValue</span><span class="sxs-lookup"><span data-stu-id="5a618-114">newvalue</span></span>|<span data-ttu-id="5a618-115">String</span><span class="sxs-lookup"><span data-stu-id="5a618-115">String</span></span>|<span data-ttu-id="5a618-116">新值。</span><span class="sxs-lookup"><span data-stu-id="5a618-116">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a618-117">关系</span><span class="sxs-lookup"><span data-stu-id="5a618-117">Relationships</span></span>
<span data-ttu-id="5a618-118">无</span><span class="sxs-lookup"><span data-stu-id="5a618-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5a618-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a618-119">JSON Representation</span></span>
<span data-ttu-id="5a618-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a618-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```



