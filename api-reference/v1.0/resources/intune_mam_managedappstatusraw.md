# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="5f4e0-101">managedAppStatusRaw 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f4e0-101">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="5f4e0-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5f4e0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f4e0-103">表示有关组织应用保护和配置的非类型化状态报告。</span><span class="sxs-lookup"><span data-stu-id="5f4e0-103">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="5f4e0-104">继承自 [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="5f4e0-104">Inherits from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="5f4e0-105">方法</span><span class="sxs-lookup"><span data-stu-id="5f4e0-105">Methods</span></span>
|<span data-ttu-id="5f4e0-106">方法</span><span class="sxs-lookup"><span data-stu-id="5f4e0-106">Method</span></span>|<span data-ttu-id="5f4e0-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="5f4e0-107">Return Type</span></span>|<span data-ttu-id="5f4e0-108">说明</span><span class="sxs-lookup"><span data-stu-id="5f4e0-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5f4e0-109">列出 managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="5f4e0-109">List managedAppStatusRaws</span></span>](../api/intune_mam_managedappstatusraw_list.md)|<span data-ttu-id="5f4e0-110">[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5f4e0-110">[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) collection</span></span>|<span data-ttu-id="5f4e0-111">列出 [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5f4e0-111">List properties and relationships of the [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="5f4e0-112">获取 managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="5f4e0-112">Get managedAppStatusRaw</span></span>](../api/intune_mam_managedappstatusraw_get.md)|[<span data-ttu-id="5f4e0-113">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="5f4e0-113">managedAppStatusRaw</span></span>](../resources/intune_mam_managedappstatusraw.md)|<span data-ttu-id="5f4e0-114">读取 [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5f4e0-114">Read properties and relationships of the [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5f4e0-115">属性</span><span class="sxs-lookup"><span data-stu-id="5f4e0-115">Properties</span></span>
|<span data-ttu-id="5f4e0-116">属性</span><span class="sxs-lookup"><span data-stu-id="5f4e0-116">Property</span></span>|<span data-ttu-id="5f4e0-117">类型</span><span class="sxs-lookup"><span data-stu-id="5f4e0-117">Type</span></span>|<span data-ttu-id="5f4e0-118">说明</span><span class="sxs-lookup"><span data-stu-id="5f4e0-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f4e0-119">displayName</span><span class="sxs-lookup"><span data-stu-id="5f4e0-119">displayName</span></span>|<span data-ttu-id="5f4e0-120">String</span><span class="sxs-lookup"><span data-stu-id="5f4e0-120">String</span></span>|<span data-ttu-id="5f4e0-121">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="5f4e0-121">Friendly name of the status report.</span></span> <span data-ttu-id="5f4e0-122">继承自 [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="5f4e0-122">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="5f4e0-123">id</span><span class="sxs-lookup"><span data-stu-id="5f4e0-123">id</span></span>|<span data-ttu-id="5f4e0-124">String</span><span class="sxs-lookup"><span data-stu-id="5f4e0-124">String</span></span>|<span data-ttu-id="5f4e0-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5f4e0-125">Key of the entity.</span></span> <span data-ttu-id="5f4e0-126">继承自 [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="5f4e0-126">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="5f4e0-127">version</span><span class="sxs-lookup"><span data-stu-id="5f4e0-127">version</span></span>|<span data-ttu-id="5f4e0-128">String</span><span class="sxs-lookup"><span data-stu-id="5f4e0-128">String</span></span>|<span data-ttu-id="5f4e0-129">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="5f4e0-129">Version of the entity.</span></span> <span data-ttu-id="5f4e0-130">继承自 [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="5f4e0-130">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="5f4e0-131">content</span><span class="sxs-lookup"><span data-stu-id="5f4e0-131">content</span></span>|[<span data-ttu-id="5f4e0-132">Json</span><span class="sxs-lookup"><span data-stu-id="5f4e0-132">Json</span></span>](../resources/intune_mam_json.md)|<span data-ttu-id="5f4e0-133">状态报告内容。</span><span class="sxs-lookup"><span data-stu-id="5f4e0-133">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f4e0-134">关系</span><span class="sxs-lookup"><span data-stu-id="5f4e0-134">Relationships</span></span>
<span data-ttu-id="5f4e0-135">无</span><span class="sxs-lookup"><span data-stu-id="5f4e0-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5f4e0-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f4e0-136">JSON Representation</span></span>
<span data-ttu-id="5f4e0-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f4e0-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```



