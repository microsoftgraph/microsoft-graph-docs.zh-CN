# <a name="managedappstatus-resource-type"></a><span data-ttu-id="a0aa2-101">managedAppStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="a0aa2-101">managedAppStatus resource type</span></span>

> <span data-ttu-id="a0aa2-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a0aa2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0aa2-103">表示组织的应用保护和配置状态。</span><span class="sxs-lookup"><span data-stu-id="a0aa2-103">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="a0aa2-104">方法</span><span class="sxs-lookup"><span data-stu-id="a0aa2-104">Methods</span></span>
|<span data-ttu-id="a0aa2-105">方法</span><span class="sxs-lookup"><span data-stu-id="a0aa2-105">Method</span></span>|<span data-ttu-id="a0aa2-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="a0aa2-106">Return Type</span></span>|<span data-ttu-id="a0aa2-107">说明</span><span class="sxs-lookup"><span data-stu-id="a0aa2-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a0aa2-108">列出 managedAppStatuses</span><span class="sxs-lookup"><span data-stu-id="a0aa2-108">List managedAppStatuses</span></span>](../api/intune_mam_managedappstatus_list.md)|<span data-ttu-id="a0aa2-109">[managedAppStatus](../resources/intune_mam_managedappstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a0aa2-109">[managedAppStatus](../resources/intune_mam_managedappstatus.md) collection</span></span>|<span data-ttu-id="a0aa2-110">列出 [managedAppStatus](../resources/intune_mam_managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a0aa2-110">List properties and relationships of the [managedAppStatus](../resources/intune_mam_managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="a0aa2-111">获取 managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="a0aa2-111">Get managedAppStatus</span></span>](../api/intune_mam_managedappstatus_get.md)|[<span data-ttu-id="a0aa2-112">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="a0aa2-112">managedAppStatus</span></span>](../resources/intune_mam_managedappstatus.md)|<span data-ttu-id="a0aa2-113">读取 [managedAppStatus](../resources/intune_mam_managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a0aa2-113">Read properties and relationships of the [managedAppStatus](../resources/intune_mam_managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a0aa2-114">属性</span><span class="sxs-lookup"><span data-stu-id="a0aa2-114">Properties</span></span>
|<span data-ttu-id="a0aa2-115">属性</span><span class="sxs-lookup"><span data-stu-id="a0aa2-115">Property</span></span>|<span data-ttu-id="a0aa2-116">类型</span><span class="sxs-lookup"><span data-stu-id="a0aa2-116">Type</span></span>|<span data-ttu-id="a0aa2-117">说明</span><span class="sxs-lookup"><span data-stu-id="a0aa2-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0aa2-118">displayName</span><span class="sxs-lookup"><span data-stu-id="a0aa2-118">displayName</span></span>|<span data-ttu-id="a0aa2-119">字符串</span><span class="sxs-lookup"><span data-stu-id="a0aa2-119">String</span></span>|<span data-ttu-id="a0aa2-120">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="a0aa2-120">Friendly name of the status report.</span></span>|
|<span data-ttu-id="a0aa2-121">id</span><span class="sxs-lookup"><span data-stu-id="a0aa2-121">id</span></span>|<span data-ttu-id="a0aa2-122">字符串</span><span class="sxs-lookup"><span data-stu-id="a0aa2-122">String</span></span>|<span data-ttu-id="a0aa2-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a0aa2-123">Key of the entity.</span></span>|
|<span data-ttu-id="a0aa2-124">version</span><span class="sxs-lookup"><span data-stu-id="a0aa2-124">version</span></span>|<span data-ttu-id="a0aa2-125">字符串</span><span class="sxs-lookup"><span data-stu-id="a0aa2-125">String</span></span>|<span data-ttu-id="a0aa2-126">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="a0aa2-126">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0aa2-127">关系</span><span class="sxs-lookup"><span data-stu-id="a0aa2-127">Relationships</span></span>
<span data-ttu-id="a0aa2-128">无</span><span class="sxs-lookup"><span data-stu-id="a0aa2-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a0aa2-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0aa2-129">JSON Representation</span></span>
<span data-ttu-id="a0aa2-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0aa2-130">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```








