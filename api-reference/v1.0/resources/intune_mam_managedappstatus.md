# <a name="managedappstatus-resource-type"></a><span data-ttu-id="12766-101">managedAppStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="12766-101">managedAppStatus resource type</span></span>

> <span data-ttu-id="12766-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="12766-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12766-103">表示组织的应用保护和配置状态。</span><span class="sxs-lookup"><span data-stu-id="12766-103">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="12766-104">方法</span><span class="sxs-lookup"><span data-stu-id="12766-104">Methods</span></span>
|<span data-ttu-id="12766-105">方法</span><span class="sxs-lookup"><span data-stu-id="12766-105">Method</span></span>|<span data-ttu-id="12766-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="12766-106">Return Type</span></span>|<span data-ttu-id="12766-107">说明</span><span class="sxs-lookup"><span data-stu-id="12766-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="12766-108">列出 managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="12766-108">List managedAppStatuses</span></span>](../api/intune_mam_managedappstatus_list.md)|<span data-ttu-id="12766-109">[managedAppStatus](../resources/intune_mam_managedappstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12766-109">[managedAppStatus](../resources/intune_mam_managedappstatus.md) collection</span></span>|<span data-ttu-id="12766-110">列出 [managedAppStatus](../resources/intune_mam_managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="12766-110">List properties and relationships of the [managedAppStatus](../resources/intune_mam_managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="12766-111">获取 managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="12766-111">Get managedAppStatus</span></span>](../api/intune_mam_managedappstatus_get.md)|[<span data-ttu-id="12766-112">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="12766-112">managedAppStatus</span></span>](../resources/intune_mam_managedappstatus.md)|<span data-ttu-id="12766-113">读取 [managedAppStatus](../resources/intune_mam_managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="12766-113">Read properties and relationships of the [managedAppStatus](../resources/intune_mam_managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="12766-114">属性</span><span class="sxs-lookup"><span data-stu-id="12766-114">Properties</span></span>
|<span data-ttu-id="12766-115">属性</span><span class="sxs-lookup"><span data-stu-id="12766-115">Property</span></span>|<span data-ttu-id="12766-116">类型</span><span class="sxs-lookup"><span data-stu-id="12766-116">Type</span></span>|<span data-ttu-id="12766-117">说明</span><span class="sxs-lookup"><span data-stu-id="12766-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12766-118">displayName</span><span class="sxs-lookup"><span data-stu-id="12766-118">displayName</span></span>|<span data-ttu-id="12766-119">String</span><span class="sxs-lookup"><span data-stu-id="12766-119">String</span></span>|<span data-ttu-id="12766-120">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="12766-120">Friendly name of the status report.</span></span>|
|<span data-ttu-id="12766-121">id</span><span class="sxs-lookup"><span data-stu-id="12766-121">id</span></span>|<span data-ttu-id="12766-122">String</span><span class="sxs-lookup"><span data-stu-id="12766-122">String</span></span>|<span data-ttu-id="12766-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="12766-123">Key of the entity.</span></span>|
|<span data-ttu-id="12766-124">version</span><span class="sxs-lookup"><span data-stu-id="12766-124">version</span></span>|<span data-ttu-id="12766-125">String</span><span class="sxs-lookup"><span data-stu-id="12766-125">String</span></span>|<span data-ttu-id="12766-126">实体版本。</span><span class="sxs-lookup"><span data-stu-id="12766-126">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12766-127">关系</span><span class="sxs-lookup"><span data-stu-id="12766-127">Relationships</span></span>
<span data-ttu-id="12766-128">无</span><span class="sxs-lookup"><span data-stu-id="12766-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="12766-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12766-129">JSON Representation</span></span>
<span data-ttu-id="12766-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12766-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```



