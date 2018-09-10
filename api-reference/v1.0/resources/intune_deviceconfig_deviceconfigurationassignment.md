# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="4a851-101">deviceConfigurationAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="4a851-101">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="4a851-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4a851-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a851-103">设备配置分配实体将 AAD 组分配到特定设备配置。</span><span class="sxs-lookup"><span data-stu-id="4a851-103">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="4a851-104">方法</span><span class="sxs-lookup"><span data-stu-id="4a851-104">Methods</span></span>
|<span data-ttu-id="4a851-105">方法</span><span class="sxs-lookup"><span data-stu-id="4a851-105">Method</span></span>|<span data-ttu-id="4a851-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="4a851-106">Return Type</span></span>|<span data-ttu-id="4a851-107">说明</span><span class="sxs-lookup"><span data-stu-id="4a851-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4a851-108">列出 deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="4a851-108">List deviceConfigurationAssignments</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_list.md)|<span data-ttu-id="4a851-109">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4a851-109">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="4a851-110">列出 [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4a851-110">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="4a851-111">获取 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4a851-111">Get deviceConfigurationAssignment</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_get.md)|[<span data-ttu-id="4a851-112">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4a851-112">deviceConfigurationAssignment</span></span>](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|<span data-ttu-id="4a851-113">读取 [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4a851-113">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="4a851-114">创建 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4a851-114">Create deviceConfigurationAssignment</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_create.md)|[<span data-ttu-id="4a851-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4a851-115">deviceConfigurationAssignment</span></span>](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|<span data-ttu-id="4a851-116">创建新的 [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4a851-116">Create a new [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="4a851-117">删除 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4a851-117">Delete deviceConfigurationAssignment</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_delete.md)|<span data-ttu-id="4a851-118">无</span><span class="sxs-lookup"><span data-stu-id="4a851-118">None</span></span>|<span data-ttu-id="4a851-119">删除 [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="4a851-119">Deletes a [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="4a851-120">更新 deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4a851-120">Update deviceConfigurationAssignment</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_update.md)|[<span data-ttu-id="4a851-121">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4a851-121">deviceConfigurationAssignment</span></span>](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|<span data-ttu-id="4a851-122">更新 [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4a851-122">Update the properties of a [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4a851-123">属性</span><span class="sxs-lookup"><span data-stu-id="4a851-123">Properties</span></span>
|<span data-ttu-id="4a851-124">属性</span><span class="sxs-lookup"><span data-stu-id="4a851-124">Property</span></span>|<span data-ttu-id="4a851-125">类型</span><span class="sxs-lookup"><span data-stu-id="4a851-125">Type</span></span>|<span data-ttu-id="4a851-126">说明</span><span class="sxs-lookup"><span data-stu-id="4a851-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a851-127">ID</span><span class="sxs-lookup"><span data-stu-id="4a851-127">id</span></span>|<span data-ttu-id="4a851-128">字符串</span><span class="sxs-lookup"><span data-stu-id="4a851-128">String</span></span>|<span data-ttu-id="4a851-129">分配的键。</span><span class="sxs-lookup"><span data-stu-id="4a851-129">The key of the assignment.</span></span>|
|<span data-ttu-id="4a851-130">target</span><span class="sxs-lookup"><span data-stu-id="4a851-130">target</span></span>|[<span data-ttu-id="4a851-131">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4a851-131">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4a851-132">设备配置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="4a851-132">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a851-133">关系</span><span class="sxs-lookup"><span data-stu-id="4a851-133">Relationships</span></span>
<span data-ttu-id="4a851-134">无</span><span class="sxs-lookup"><span data-stu-id="4a851-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4a851-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a851-135">JSON Representation</span></span>
<span data-ttu-id="4a851-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a851-136">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```








