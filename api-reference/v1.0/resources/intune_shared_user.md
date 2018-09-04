# <a name="user-resource-type"></a><span data-ttu-id="60372-101">用户资源类型</span><span class="sxs-lookup"><span data-stu-id="60372-101">user resource type</span></span>

> <span data-ttu-id="60372-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="60372-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60372-103">表示 Azure Active Directory 用户对象。</span><span class="sxs-lookup"><span data-stu-id="60372-103">Represents an Azure Active Directory user object.</span></span>

## <a name="methods"></a><span data-ttu-id="60372-104">方法</span><span class="sxs-lookup"><span data-stu-id="60372-104">Methods</span></span>
|<span data-ttu-id="60372-105">方法</span><span class="sxs-lookup"><span data-stu-id="60372-105">Method</span></span>|<span data-ttu-id="60372-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="60372-106">Return Type</span></span>|<span data-ttu-id="60372-107">描述</span><span class="sxs-lookup"><span data-stu-id="60372-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60372-108">[列出用户](../api/intune_shared_user_list.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60372-108">[List users](../api/intune_shared_user_list.md) objects.</span></span>|
|<span data-ttu-id="60372-109">[获取用户](../api/intune_shared_user_get.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60372-109">[Get user](../api/intune_shared_user_get.md) object.</span></span>|
|<span data-ttu-id="60372-110">[创建用户](../api/intune_shared_user_create.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60372-110">Create a new [user](../api/intune_shared_user_create.md) object.</span></span>|
|<span data-ttu-id="60372-111">[删除用户](../api/intune_shared_user_delete.md) 。</span><span class="sxs-lookup"><span data-stu-id="60372-111">Delete user</span></span>|
|<span data-ttu-id="60372-112">[更新用户](../api/intune_shared_user_update.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60372-112">Update user object.</span></span>|
|<span data-ttu-id="60372-113">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="60372-113">**Device management**</span></span>|
|[<span data-ttu-id="60372-114">removeAllDevicesFromManagement 操作</span><span class="sxs-lookup"><span data-stu-id="60372-114">removeAllDevicesFromManagement action</span></span>](../api/intune_shared_user_removealldevicesfrommanagement.md)|<span data-ttu-id="60372-115">无</span><span class="sxs-lookup"><span data-stu-id="60372-115">None</span></span>|<span data-ttu-id="60372-116">注销该用户对所有设备的管理</span><span class="sxs-lookup"><span data-stu-id="60372-116">Retire all devices from management for this user</span></span>|
|<span data-ttu-id="60372-117">**移动应用程序管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="60372-117">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="60372-118">getManagedAppDiagnosticStatuses 函数</span><span class="sxs-lookup"><span data-stu-id="60372-118">getManagedAppDiagnosticStatuses function</span></span>](../api/intune_shared_user_getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="60372-119">[managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="60372-119">[managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="60372-120">获取给定用户的诊断验证状态。</span><span class="sxs-lookup"><span data-stu-id="60372-120">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="60372-121">getManagedAppPolicies 函数</span><span class="sxs-lookup"><span data-stu-id="60372-121">getManagedAppPolicies function</span></span>](../api/intune_shared_user_getmanagedapppolicies.md)|<span data-ttu-id="60372-122">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="60372-122">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="60372-123">获取给定用户的应用限制。</span><span class="sxs-lookup"><span data-stu-id="60372-123">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="60372-124">wipeManagedAppRegistrationsByDeviceTag 操作</span><span class="sxs-lookup"><span data-stu-id="60372-124">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune_shared_user_wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="60372-125">无</span><span class="sxs-lookup"><span data-stu-id="60372-125">None</span></span>|<span data-ttu-id="60372-126">对含有指定设备标记的应用注册发布擦除操作。</span><span class="sxs-lookup"><span data-stu-id="60372-126">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="60372-127">属性</span><span class="sxs-lookup"><span data-stu-id="60372-127">Properties</span></span>
|<span data-ttu-id="60372-128">属性</span><span class="sxs-lookup"><span data-stu-id="60372-128">Property</span></span>|<span data-ttu-id="60372-129">类型</span><span class="sxs-lookup"><span data-stu-id="60372-129">Type</span></span>|<span data-ttu-id="60372-130">说明</span><span class="sxs-lookup"><span data-stu-id="60372-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60372-131">id</span><span class="sxs-lookup"><span data-stu-id="60372-131">id</span></span>|<span data-ttu-id="60372-132">字符串</span><span class="sxs-lookup"><span data-stu-id="60372-132">String</span></span>|<span data-ttu-id="60372-133">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="60372-133">Unique identifier of the user.</span></span>|
|<span data-ttu-id="60372-134">**加入**</span><span class="sxs-lookup"><span data-stu-id="60372-134">**On-boarding**</span></span>|
|<span data-ttu-id="60372-135">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="60372-135">deviceEnrollmentLimit</span></span>|<span data-ttu-id="60372-136">Int32</span><span class="sxs-lookup"><span data-stu-id="60372-136">Int32</span></span>|<span data-ttu-id="60372-137">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="60372-137">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="60372-138">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="60372-138">Allowed values are 5 or 1000.</span></span>|


## <a name="relationships"></a><span data-ttu-id="60372-139">关系</span><span class="sxs-lookup"><span data-stu-id="60372-139">Relationships</span></span>
|<span data-ttu-id="60372-140">关系</span><span class="sxs-lookup"><span data-stu-id="60372-140">Relationship</span></span>|<span data-ttu-id="60372-141">类型</span><span class="sxs-lookup"><span data-stu-id="60372-141">Type</span></span>|<span data-ttu-id="60372-142">描述</span><span class="sxs-lookup"><span data-stu-id="60372-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60372-143">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="60372-143">**Device management**</span></span>|
|<span data-ttu-id="60372-144">managedDevices</span><span class="sxs-lookup"><span data-stu-id="60372-144">managedDevices</span></span>|<span data-ttu-id="60372-145">[managedDevice](../resources/intune_devices_manageddevice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="60372-145">[managedDevice](../resources/intune_devices_manageddevice.md) collection</span></span>|<span data-ttu-id="60372-146">与用户关联的管理设备。</span><span class="sxs-lookup"><span data-stu-id="60372-146">The managed devices associated with the user.</span></span>|
|<span data-ttu-id="60372-147">**移动应用程序管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="60372-147">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="60372-148">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="60372-148">managedAppRegistrations</span></span>|<span data-ttu-id="60372-149">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="60372-149">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) collection</span></span>|<span data-ttu-id="60372-150">属于用户的零个或多个管理应用程序注册。</span><span class="sxs-lookup"><span data-stu-id="60372-150">Zero or more managed app registrations that belong to the user.</span></span>|
|<span data-ttu-id="60372-151">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="60372-151">**Troubleshooting**</span></span>|
|<span data-ttu-id="60372-152">deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="60372-152">deviceManagementTroubleshootingEvents</span></span>|<span data-ttu-id="60372-153">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="60372-153">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="60372-154">此用户的故障排除事件列表。</span><span class="sxs-lookup"><span data-stu-id="60372-154">The list of troubleshooting events for this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60372-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60372-155">JSON Representation</span></span>
<span data-ttu-id="60372-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60372-156">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 5
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Resource microsoft.graph.user is defined in multiple files: /api-reference/v1.0/resources/intune_shared_user.md, /api-reference/v1.0/resources/user.md",
  ]
}-->
