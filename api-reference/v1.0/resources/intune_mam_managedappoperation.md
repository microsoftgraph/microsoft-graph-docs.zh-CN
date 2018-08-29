# <a name="managedappoperation-resource-type"></a><span data-ttu-id="a25fd-101">managedAppOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="a25fd-101">managedAppOperation resource type</span></span>

> <span data-ttu-id="a25fd-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a25fd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a25fd-103">表示对应用注册应用的操作。</span><span class="sxs-lookup"><span data-stu-id="a25fd-103">Represents an operation applied against an app registration.</span></span>
## <a name="methods"></a><span data-ttu-id="a25fd-104">方法</span><span class="sxs-lookup"><span data-stu-id="a25fd-104">Methods</span></span>
|<span data-ttu-id="a25fd-105">方法</span><span class="sxs-lookup"><span data-stu-id="a25fd-105">Method</span></span>|<span data-ttu-id="a25fd-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="a25fd-106">Return Type</span></span>|<span data-ttu-id="a25fd-107">说明</span><span class="sxs-lookup"><span data-stu-id="a25fd-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a25fd-108">列出 managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="a25fd-108">List managedAppOperations</span></span>](../api/intune_mam_managedappoperation_list.md)|<span data-ttu-id="a25fd-109">[managedAppOperation](../resources/intune_mam_managedappoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a25fd-109">[managedAppOperation](../resources/intune_mam_managedappoperation.md) collection</span></span>|<span data-ttu-id="a25fd-110">列出 [managedAppOperation](../resources/intune_mam_managedappoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a25fd-110">List properties and relationships of the [managedAppOperation](../resources/intune_mam_managedappoperation.md) objects.</span></span>|
|[<span data-ttu-id="a25fd-111">获取 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="a25fd-111">Get managedAppOperation</span></span>](../api/intune_mam_managedappoperation_get.md)|[<span data-ttu-id="a25fd-112">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="a25fd-112">managedAppOperation</span></span>](../resources/intune_mam_managedappoperation.md)|<span data-ttu-id="a25fd-113">读取 [managedAppOperation](../resources/intune_mam_managedappoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a25fd-113">Read properties and relationships of the [managedAppOperation](../resources/intune_mam_managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="a25fd-114">创建 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="a25fd-114">Create managedAppOperation</span></span>](../api/intune_mam_managedappoperation_create.md)|[<span data-ttu-id="a25fd-115">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="a25fd-115">managedAppOperation</span></span>](../resources/intune_mam_managedappoperation.md)|<span data-ttu-id="a25fd-116">创建新的 [managedAppOperation](../resources/intune_mam_managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a25fd-116">Create a new [managedAppOperation](../resources/intune_mam_managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="a25fd-117">删除 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="a25fd-117">Delete managedAppOperation</span></span>](../api/intune_mam_managedappoperation_delete.md)|<span data-ttu-id="a25fd-118">无</span><span class="sxs-lookup"><span data-stu-id="a25fd-118">None</span></span>|<span data-ttu-id="a25fd-119">删除 [managedAppOperation](../resources/intune_mam_managedappoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="a25fd-119">Deletes a [managedAppOperation](../resources/intune_mam_managedappoperation.md).</span></span>|
|[<span data-ttu-id="a25fd-120">更新 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="a25fd-120">Update managedAppOperation</span></span>](../api/intune_mam_managedappoperation_update.md)|[<span data-ttu-id="a25fd-121">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="a25fd-121">managedAppOperation</span></span>](../resources/intune_mam_managedappoperation.md)|<span data-ttu-id="a25fd-122">更新 [managedAppOperation](../resources/intune_mam_managedappoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a25fd-122">Update the properties of a [managedAppOperation](../resources/intune_mam_managedappoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a25fd-123">属性</span><span class="sxs-lookup"><span data-stu-id="a25fd-123">Properties</span></span>
|<span data-ttu-id="a25fd-124">属性</span><span class="sxs-lookup"><span data-stu-id="a25fd-124">Property</span></span>|<span data-ttu-id="a25fd-125">类型</span><span class="sxs-lookup"><span data-stu-id="a25fd-125">Type</span></span>|<span data-ttu-id="a25fd-126">说明</span><span class="sxs-lookup"><span data-stu-id="a25fd-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a25fd-127">displayName</span><span class="sxs-lookup"><span data-stu-id="a25fd-127">displayName</span></span>|<span data-ttu-id="a25fd-128">String</span><span class="sxs-lookup"><span data-stu-id="a25fd-128">String</span></span>|<span data-ttu-id="a25fd-129">操作名称。</span><span class="sxs-lookup"><span data-stu-id="a25fd-129">The operation name.</span></span>|
|<span data-ttu-id="a25fd-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a25fd-130">lastModifiedDateTime</span></span>|<span data-ttu-id="a25fd-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a25fd-131">DateTimeOffset</span></span>|<span data-ttu-id="a25fd-132">上次修改应用操作的时间。</span><span class="sxs-lookup"><span data-stu-id="a25fd-132">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="a25fd-133">state</span><span class="sxs-lookup"><span data-stu-id="a25fd-133">state</span></span>|<span data-ttu-id="a25fd-134">String</span><span class="sxs-lookup"><span data-stu-id="a25fd-134">String</span></span>|<span data-ttu-id="a25fd-135">操作的当前状态</span><span class="sxs-lookup"><span data-stu-id="a25fd-135">The current state of the operation</span></span>|
|<span data-ttu-id="a25fd-136">id</span><span class="sxs-lookup"><span data-stu-id="a25fd-136">id</span></span>|<span data-ttu-id="a25fd-137">String</span><span class="sxs-lookup"><span data-stu-id="a25fd-137">String</span></span>|<span data-ttu-id="a25fd-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a25fd-138">Key of the entity.</span></span>|
|<span data-ttu-id="a25fd-139">version</span><span class="sxs-lookup"><span data-stu-id="a25fd-139">version</span></span>|<span data-ttu-id="a25fd-140">String</span><span class="sxs-lookup"><span data-stu-id="a25fd-140">String</span></span>|<span data-ttu-id="a25fd-141">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="a25fd-141">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a25fd-142">关系</span><span class="sxs-lookup"><span data-stu-id="a25fd-142">Relationships</span></span>
<span data-ttu-id="a25fd-143">无</span><span class="sxs-lookup"><span data-stu-id="a25fd-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a25fd-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a25fd-144">JSON Representation</span></span>
<span data-ttu-id="a25fd-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a25fd-145">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedAppOperation"
}-->
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



