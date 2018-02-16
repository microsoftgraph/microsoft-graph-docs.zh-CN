# <a name="auditresource-resource-type"></a><span data-ttu-id="55a6c-101">auditResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="55a6c-101">auditResource resource type</span></span>

> <span data-ttu-id="55a6c-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="55a6c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55a6c-103">包含审核资源的属性的类。</span><span class="sxs-lookup"><span data-stu-id="55a6c-103">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="55a6c-104">属性</span><span class="sxs-lookup"><span data-stu-id="55a6c-104">Properties</span></span>
|<span data-ttu-id="55a6c-105">属性</span><span class="sxs-lookup"><span data-stu-id="55a6c-105">Property</span></span>|<span data-ttu-id="55a6c-106">类型</span><span class="sxs-lookup"><span data-stu-id="55a6c-106">Type</span></span>|<span data-ttu-id="55a6c-107">说明</span><span class="sxs-lookup"><span data-stu-id="55a6c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55a6c-108">displayName</span><span class="sxs-lookup"><span data-stu-id="55a6c-108">displayName</span></span>|<span data-ttu-id="55a6c-109">String</span><span class="sxs-lookup"><span data-stu-id="55a6c-109">String</span></span>|<span data-ttu-id="55a6c-110">显示名称。</span><span class="sxs-lookup"><span data-stu-id="55a6c-110">Display Name</span></span>|
|<span data-ttu-id="55a6c-111">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="55a6c-111">modifiedProperties</span></span>|<span data-ttu-id="55a6c-112">[auditProperty](../resources/intune_auditing_auditproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="55a6c-112">[auditProperty](../resources/intune_auditing_auditproperty.md) collection</span></span>|<span data-ttu-id="55a6c-113">已修改属性列表。</span><span class="sxs-lookup"><span data-stu-id="55a6c-113">List of managed properties</span></span>|
|<span data-ttu-id="55a6c-114">type</span><span class="sxs-lookup"><span data-stu-id="55a6c-114">type</span></span>|<span data-ttu-id="55a6c-115">String</span><span class="sxs-lookup"><span data-stu-id="55a6c-115">String</span></span>|<span data-ttu-id="55a6c-116">审核资源的类型。</span><span class="sxs-lookup"><span data-stu-id="55a6c-116">Audit resource's type.</span></span>|
|<span data-ttu-id="55a6c-117">resourceId</span><span class="sxs-lookup"><span data-stu-id="55a6c-117">resourceId</span></span>|<span data-ttu-id="55a6c-118">String</span><span class="sxs-lookup"><span data-stu-id="55a6c-118">String</span></span>|<span data-ttu-id="55a6c-119">审核资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="55a6c-119">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55a6c-120">关系</span><span class="sxs-lookup"><span data-stu-id="55a6c-120">Relationships</span></span>
<span data-ttu-id="55a6c-121">无</span><span class="sxs-lookup"><span data-stu-id="55a6c-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="55a6c-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55a6c-122">JSON Representation</span></span>
<span data-ttu-id="55a6c-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55a6c-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```



