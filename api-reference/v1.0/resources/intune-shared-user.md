---
title: 用户资源类型
description: 表示 Azure Active Directory 用户对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f486e3202535882d719e5f6c083b583321e917b5
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732385"
---
# <a name="user-resource-type"></a><span data-ttu-id="d975b-103">用户资源类型</span><span class="sxs-lookup"><span data-stu-id="d975b-103">user resource type</span></span>

<span data-ttu-id="d975b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d975b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d975b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d975b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d975b-106">表示 Azure Active Directory 用户对象。</span><span class="sxs-lookup"><span data-stu-id="d975b-106">Represents an Azure Active Directory user object.</span></span>

## <a name="methods"></a><span data-ttu-id="d975b-107">Methods</span><span class="sxs-lookup"><span data-stu-id="d975b-107">Methods</span></span>
|<span data-ttu-id="d975b-108">方法</span><span class="sxs-lookup"><span data-stu-id="d975b-108">Method</span></span>|<span data-ttu-id="d975b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d975b-109">Return Type</span></span>|<span data-ttu-id="d975b-110">Description</span><span class="sxs-lookup"><span data-stu-id="d975b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d975b-111">[列出 users](../api/intune-shared-user-list.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d975b-111">[List users](../api/intune-shared-user-list.md) objects.</span></span>|<span data-ttu-id="d975b-112">[user](../resources/intune-shared-user.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d975b-112">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="d975b-113">列出 [user](../resources/intune-shared-user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d975b-113">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>|
|<span data-ttu-id="d975b-114">[获取 user](../api/intune-shared-user-get.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d975b-114">[Get user](../api/intune-shared-user-get.md) object.</span></span>|<span data-ttu-id="d975b-115">[user](../resources/intune-shared-user.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d975b-115">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="d975b-116">读取 [user](../resources/intune-shared-user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d975b-116">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="d975b-117">[创建 user](../api/intune-shared-user-create.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d975b-117">[Create user](../api/intune-shared-user-create.md) object.</span></span>|<span data-ttu-id="d975b-118">[user](../resources/intune-shared-user.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d975b-118">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="d975b-119">创建新的 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d975b-119">Create a new [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="d975b-120">[删除用户](../api/intune-shared-user-delete.md)。</span><span class="sxs-lookup"><span data-stu-id="d975b-120">[Delete user](../api/intune-shared-user-delete.md).</span></span>|<span data-ttu-id="d975b-121">无</span><span class="sxs-lookup"><span data-stu-id="d975b-121">None</span></span>|<span data-ttu-id="d975b-122">删除 [user](../resources/intune-shared-user.md)。</span><span class="sxs-lookup"><span data-stu-id="d975b-122">Deletes a [user](../resources/intune-shared-user.md).</span></span>|
|<span data-ttu-id="d975b-123">[更新 user](../api/intune-shared-user-update.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d975b-123">[Update user](../api/intune-shared-user-update.md) object.</span></span>|[<span data-ttu-id="d975b-124">user</span><span class="sxs-lookup"><span data-stu-id="d975b-124">user</span></span>](../resources/intune-shared-user.md)|<span data-ttu-id="d975b-125">更新 [user](../resources/intune-shared-user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d975b-125">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="d975b-126">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="d975b-126">**Device management**</span></span>|
|[<span data-ttu-id="d975b-127">removeAllDevicesFromManagement 操作</span><span class="sxs-lookup"><span data-stu-id="d975b-127">removeAllDevicesFromManagement action</span></span>](../api/intune-shared-user-removealldevicesfrommanagement.md)|<span data-ttu-id="d975b-128">无</span><span class="sxs-lookup"><span data-stu-id="d975b-128">None</span></span>|<span data-ttu-id="d975b-129">停用该用户管理的所有设备</span><span class="sxs-lookup"><span data-stu-id="d975b-129">Retire all devices from management for this user</span></span>|
|<span data-ttu-id="d975b-130">**移动应用管理(MAM)**</span><span class="sxs-lookup"><span data-stu-id="d975b-130">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="d975b-131">getManagedAppDiagnosticStatuses 函数</span><span class="sxs-lookup"><span data-stu-id="d975b-131">getManagedAppDiagnosticStatuses function</span></span>](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="d975b-132">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d975b-132">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="d975b-133">获取给定用户的诊断验证状态。</span><span class="sxs-lookup"><span data-stu-id="d975b-133">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="d975b-134">getManagedAppPolicies 函数</span><span class="sxs-lookup"><span data-stu-id="d975b-134">getManagedAppPolicies function</span></span>](../api/intune-shared-user-getmanagedapppolicies.md)|<span data-ttu-id="d975b-135">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d975b-135">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="d975b-136">获取给定用户的应用限制。</span><span class="sxs-lookup"><span data-stu-id="d975b-136">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="d975b-137">wipeManagedAppRegistrationsByDeviceTag 操作</span><span class="sxs-lookup"><span data-stu-id="d975b-137">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="d975b-138">无</span><span class="sxs-lookup"><span data-stu-id="d975b-138">None</span></span>|<span data-ttu-id="d975b-139">对含有指定设备标记的应用注册发布擦除操作。</span><span class="sxs-lookup"><span data-stu-id="d975b-139">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="d975b-140">属性</span><span class="sxs-lookup"><span data-stu-id="d975b-140">Properties</span></span>
|<span data-ttu-id="d975b-141">属性</span><span class="sxs-lookup"><span data-stu-id="d975b-141">Property</span></span>|<span data-ttu-id="d975b-142">类型</span><span class="sxs-lookup"><span data-stu-id="d975b-142">Type</span></span>|<span data-ttu-id="d975b-143">说明</span><span class="sxs-lookup"><span data-stu-id="d975b-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d975b-144">id</span><span class="sxs-lookup"><span data-stu-id="d975b-144">id</span></span>|<span data-ttu-id="d975b-145">String</span><span class="sxs-lookup"><span data-stu-id="d975b-145">String</span></span>|<span data-ttu-id="d975b-146">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d975b-146">Unique identifier of the user.</span></span>|
|<span data-ttu-id="d975b-147">**载入**</span><span class="sxs-lookup"><span data-stu-id="d975b-147">**Onboarding**</span></span>|
|<span data-ttu-id="d975b-148">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="d975b-148">deviceEnrollmentLimit</span></span>|<span data-ttu-id="d975b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d975b-149">Int32</span></span>|<span data-ttu-id="d975b-150">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="d975b-150">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="d975b-151">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="d975b-151">Allowed values are 5 or 1000.</span></span>|


## <a name="relationships"></a><span data-ttu-id="d975b-152">关系</span><span class="sxs-lookup"><span data-stu-id="d975b-152">Relationships</span></span>
|<span data-ttu-id="d975b-153">关系</span><span class="sxs-lookup"><span data-stu-id="d975b-153">Relationship</span></span>|<span data-ttu-id="d975b-154">类型</span><span class="sxs-lookup"><span data-stu-id="d975b-154">Type</span></span>|<span data-ttu-id="d975b-155">Description</span><span class="sxs-lookup"><span data-stu-id="d975b-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d975b-156">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="d975b-156">**Device management**</span></span>|
|<span data-ttu-id="d975b-157">managedDevices</span><span class="sxs-lookup"><span data-stu-id="d975b-157">managedDevices</span></span>|<span data-ttu-id="d975b-158">[managedDevice](../resources/intune-devices-manageddevice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d975b-158">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="d975b-159">与用户关联的管理设备。</span><span class="sxs-lookup"><span data-stu-id="d975b-159">The managed devices associated with the user.</span></span>|
|<span data-ttu-id="d975b-160">**移动应用管理(MAM)**</span><span class="sxs-lookup"><span data-stu-id="d975b-160">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="d975b-161">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="d975b-161">managedAppRegistrations</span></span>|<span data-ttu-id="d975b-162">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d975b-162">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="d975b-163">属于用户的零个或多个托管的应用注册。</span><span class="sxs-lookup"><span data-stu-id="d975b-163">Zero or more managed app registrations that belong to the user.</span></span>|
|<span data-ttu-id="d975b-164">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="d975b-164">**Troubleshooting**</span></span>|
|<span data-ttu-id="d975b-165">deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="d975b-165">deviceManagementTroubleshootingEvents</span></span>|<span data-ttu-id="d975b-166">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d975b-166">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="d975b-167">此用户的故障排除事件列表。</span><span class="sxs-lookup"><span data-stu-id="d975b-167">The list of troubleshooting events for this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d975b-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d975b-168">JSON Representation</span></span>
<span data-ttu-id="d975b-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d975b-169">Here is a JSON representation of the resource.</span></span>
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






