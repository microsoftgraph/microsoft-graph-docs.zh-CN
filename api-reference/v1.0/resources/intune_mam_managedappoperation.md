# <a name="managedappoperation-resource-type"></a><span data-ttu-id="1fb77-101">managedAppOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="1fb77-101">managedAppOperation resource type</span></span>

> <span data-ttu-id="1fb77-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1fb77-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1fb77-103">表示对应用注册应用的操作。</span><span class="sxs-lookup"><span data-stu-id="1fb77-103">Represents an operation applied against an app registration.</span></span>
## <a name="methods"></a><span data-ttu-id="1fb77-104">方法</span><span class="sxs-lookup"><span data-stu-id="1fb77-104">Methods</span></span>
|<span data-ttu-id="1fb77-105">方法</span><span class="sxs-lookup"><span data-stu-id="1fb77-105">Method</span></span>|<span data-ttu-id="1fb77-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="1fb77-106">Return Type</span></span>|<span data-ttu-id="1fb77-107">说明</span><span class="sxs-lookup"><span data-stu-id="1fb77-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1fb77-108">列出 managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="1fb77-108">List managedAppOperations</span></span>](../api/intune_mam_managedappoperation_list.md)|<span data-ttu-id="1fb77-109">[managedAppOperation](../resources/intune_mam_managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1fb77-109">[managedAppOperation](../resources/intune_mam_managedappoperation.md) collection</span></span>|<span data-ttu-id="1fb77-110">列出 [managedAppOperation](../resources/intune_mam_managedappoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1fb77-110">List properties and relationships of the [managedAppOperation](../resources/intune_mam_managedappoperation.md) objects.</span></span>|
|[<span data-ttu-id="1fb77-111">获取 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="1fb77-111">Get managedAppOperation</span></span>](../api/intune_mam_managedappoperation_get.md)|[<span data-ttu-id="1fb77-112">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="1fb77-112">managedAppOperation</span></span>](../resources/intune_mam_managedappoperation.md)|<span data-ttu-id="1fb77-113">读取 [managedAppOperation](../resources/intune_mam_managedappoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1fb77-113">Read properties and relationships of the [managedAppOperation](../resources/intune_mam_managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="1fb77-114">创建 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="1fb77-114">Create managedAppOperation</span></span>](../api/intune_mam_managedappoperation_create.md)|[<span data-ttu-id="1fb77-115">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="1fb77-115">managedAppOperation</span></span>](../resources/intune_mam_managedappoperation.md)|<span data-ttu-id="1fb77-116">创建新的 [managedAppOperation](../resources/intune_mam_managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1fb77-116">Create a new [managedAppOperation](../resources/intune_mam_managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="1fb77-117">删除 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="1fb77-117">Delete managedAppOperation</span></span>](../api/intune_mam_managedappoperation_delete.md)|<span data-ttu-id="1fb77-118">无</span><span class="sxs-lookup"><span data-stu-id="1fb77-118">None</span></span>|<span data-ttu-id="1fb77-119">删除 [managedAppOperation](../resources/intune_mam_managedappoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="1fb77-119">Deletes a [managedAppOperation](../resources/intune_mam_managedappoperation.md).</span></span>|
|[<span data-ttu-id="1fb77-120">更新 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="1fb77-120">Update managedAppOperation</span></span>](../api/intune_mam_managedappoperation_update.md)|[<span data-ttu-id="1fb77-121">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="1fb77-121">managedAppOperation</span></span>](../resources/intune_mam_managedappoperation.md)|<span data-ttu-id="1fb77-122">更新 [managedAppOperation](../resources/intune_mam_managedappoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1fb77-122">Update the properties of a [managedAppOperation](../resources/intune_mam_managedappoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1fb77-123">属性</span><span class="sxs-lookup"><span data-stu-id="1fb77-123">Properties</span></span>
|<span data-ttu-id="1fb77-124">属性</span><span class="sxs-lookup"><span data-stu-id="1fb77-124">Property</span></span>|<span data-ttu-id="1fb77-125">类型</span><span class="sxs-lookup"><span data-stu-id="1fb77-125">Type</span></span>|<span data-ttu-id="1fb77-126">说明</span><span class="sxs-lookup"><span data-stu-id="1fb77-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fb77-127">displayName</span><span class="sxs-lookup"><span data-stu-id="1fb77-127">displayName</span></span>|<span data-ttu-id="1fb77-128">String</span><span class="sxs-lookup"><span data-stu-id="1fb77-128">String</span></span>|<span data-ttu-id="1fb77-129">操作名称。</span><span class="sxs-lookup"><span data-stu-id="1fb77-129">The operation name.</span></span>|
|<span data-ttu-id="1fb77-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1fb77-130">lastModifiedDateTime</span></span>|<span data-ttu-id="1fb77-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fb77-131">DateTimeOffset</span></span>|<span data-ttu-id="1fb77-132">上次修改应用操作的时间。</span><span class="sxs-lookup"><span data-stu-id="1fb77-132">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="1fb77-133">state</span><span class="sxs-lookup"><span data-stu-id="1fb77-133">state</span></span>|<span data-ttu-id="1fb77-134">String</span><span class="sxs-lookup"><span data-stu-id="1fb77-134">String</span></span>|<span data-ttu-id="1fb77-135">操作的当前状态</span><span class="sxs-lookup"><span data-stu-id="1fb77-135">The current state of the operation</span></span>|
|<span data-ttu-id="1fb77-136">id</span><span class="sxs-lookup"><span data-stu-id="1fb77-136">id</span></span>|<span data-ttu-id="1fb77-137">String</span><span class="sxs-lookup"><span data-stu-id="1fb77-137">String</span></span>|<span data-ttu-id="1fb77-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1fb77-138">Key of the entity.</span></span>|
|<span data-ttu-id="1fb77-139">version</span><span class="sxs-lookup"><span data-stu-id="1fb77-139">version</span></span>|<span data-ttu-id="1fb77-140">String</span><span class="sxs-lookup"><span data-stu-id="1fb77-140">String</span></span>|<span data-ttu-id="1fb77-141">实体版本。</span><span class="sxs-lookup"><span data-stu-id="1fb77-141">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1fb77-142">关系</span><span class="sxs-lookup"><span data-stu-id="1fb77-142">Relationships</span></span>
<span data-ttu-id="1fb77-143">无</span><span class="sxs-lookup"><span data-stu-id="1fb77-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1fb77-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1fb77-144">JSON Representation</span></span>
<span data-ttu-id="1fb77-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1fb77-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "id": "String (identifier)",
  "version": "String"
}
```



