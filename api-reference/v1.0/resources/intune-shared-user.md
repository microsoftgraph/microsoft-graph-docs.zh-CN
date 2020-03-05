---
title: 用户资源类型
description: 表示 Azure Active Directory 用户对象。
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 52a353f4e4d99f5d68812bd89ea0b9467ee7e5c9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447785"
---
# <a name="user-resource-type"></a><span data-ttu-id="b7782-103">用户资源类型</span><span class="sxs-lookup"><span data-stu-id="b7782-103">user resource type</span></span>

<span data-ttu-id="b7782-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b7782-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7782-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b7782-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7782-106">表示 Azure Active Directory 用户对象。</span><span class="sxs-lookup"><span data-stu-id="b7782-106">Represents an Azure Active Directory user object.</span></span>

## <a name="methods"></a><span data-ttu-id="b7782-107">方法</span><span class="sxs-lookup"><span data-stu-id="b7782-107">Methods</span></span>
|<span data-ttu-id="b7782-108">方法</span><span class="sxs-lookup"><span data-stu-id="b7782-108">Method</span></span>|<span data-ttu-id="b7782-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b7782-109">Return Type</span></span>|<span data-ttu-id="b7782-110">说明</span><span class="sxs-lookup"><span data-stu-id="b7782-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7782-111">[列出用户](../api/intune-shared-user-list.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b7782-111">[List users](../api/intune-shared-user-list.md) objects.</span></span>|<span data-ttu-id="b7782-112">[user](../resources/intune-shared-user.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b7782-112">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="b7782-113">列出 [user](../resources/intune-shared-user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b7782-113">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>|
|<span data-ttu-id="b7782-114">[获取用户](../api/intune-shared-user-get.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b7782-114">[Get user](../api/intune-shared-user-get.md) object.</span></span>|<span data-ttu-id="b7782-115">[user](../resources/intune-shared-user.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b7782-115">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="b7782-116">读取 [user](../resources/intune-shared-user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b7782-116">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="b7782-117">[创建用户](../api/intune-shared-user-create.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b7782-117">[Create user](../api/intune-shared-user-create.md) object.</span></span>|<span data-ttu-id="b7782-118">[user](../resources/intune-shared-user.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b7782-118">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="b7782-119">创建新的 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b7782-119">Create a new [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="b7782-120">[删除用户](../api/intune-shared-user-delete.md)。</span><span class="sxs-lookup"><span data-stu-id="b7782-120">[Delete user](../api/intune-shared-user-delete.md).</span></span>|<span data-ttu-id="b7782-121">无</span><span class="sxs-lookup"><span data-stu-id="b7782-121">None</span></span>|<span data-ttu-id="b7782-122">删除 [user](../resources/intune-shared-user.md)。</span><span class="sxs-lookup"><span data-stu-id="b7782-122">Deletes a [user](../resources/intune-shared-user.md).</span></span>|
|<span data-ttu-id="b7782-123">[更新 user](../api/intune-shared-user-update.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b7782-123">[Update user](../api/intune-shared-user-update.md) object.</span></span>|[<span data-ttu-id="b7782-124">user</span><span class="sxs-lookup"><span data-stu-id="b7782-124">user</span></span>](../resources/intune-shared-user.md)|<span data-ttu-id="b7782-125">更新 [user](../resources/intune-shared-user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b7782-125">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="b7782-126">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="b7782-126">**Device management**</span></span>|
|[<span data-ttu-id="b7782-127">removeAllDevicesFromManagement 操作</span><span class="sxs-lookup"><span data-stu-id="b7782-127">removeAllDevicesFromManagement action</span></span>](../api/intune-shared-user-removealldevicesfrommanagement.md)|<span data-ttu-id="b7782-128">无</span><span class="sxs-lookup"><span data-stu-id="b7782-128">None</span></span>|<span data-ttu-id="b7782-129">停用该用户管理的所有设备</span><span class="sxs-lookup"><span data-stu-id="b7782-129">Retire all devices from management for this user</span></span>|
|<span data-ttu-id="b7782-130">**移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="b7782-130">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="b7782-131">getManagedAppDiagnosticStatuses 函数</span><span class="sxs-lookup"><span data-stu-id="b7782-131">getManagedAppDiagnosticStatuses function</span></span>](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="b7782-132">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b7782-132">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="b7782-133">获取给定用户的诊断验证状态。</span><span class="sxs-lookup"><span data-stu-id="b7782-133">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="b7782-134">getManagedAppPolicies 函数</span><span class="sxs-lookup"><span data-stu-id="b7782-134">getManagedAppPolicies function</span></span>](../api/intune-shared-user-getmanagedapppolicies.md)|<span data-ttu-id="b7782-135">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b7782-135">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="b7782-136">获取给定用户的应用限制。</span><span class="sxs-lookup"><span data-stu-id="b7782-136">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="b7782-137">wipeManagedAppRegistrationsByDeviceTag 操作</span><span class="sxs-lookup"><span data-stu-id="b7782-137">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="b7782-138">无</span><span class="sxs-lookup"><span data-stu-id="b7782-138">None</span></span>|<span data-ttu-id="b7782-139">对含有指定设备标记的应用注册发布擦除操作。</span><span class="sxs-lookup"><span data-stu-id="b7782-139">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="b7782-140">属性</span><span class="sxs-lookup"><span data-stu-id="b7782-140">Properties</span></span>
|<span data-ttu-id="b7782-141">属性</span><span class="sxs-lookup"><span data-stu-id="b7782-141">Property</span></span>|<span data-ttu-id="b7782-142">类型</span><span class="sxs-lookup"><span data-stu-id="b7782-142">Type</span></span>|<span data-ttu-id="b7782-143">说明</span><span class="sxs-lookup"><span data-stu-id="b7782-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7782-144">id</span><span class="sxs-lookup"><span data-stu-id="b7782-144">id</span></span>|<span data-ttu-id="b7782-145">String</span><span class="sxs-lookup"><span data-stu-id="b7782-145">String</span></span>|<span data-ttu-id="b7782-146">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b7782-146">Unique identifier of the user.</span></span>|
|<span data-ttu-id="b7782-147">**载入**</span><span class="sxs-lookup"><span data-stu-id="b7782-147">**Onboarding**</span></span>|
|<span data-ttu-id="b7782-148">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="b7782-148">deviceEnrollmentLimit</span></span>|<span data-ttu-id="b7782-149">Int32</span><span class="sxs-lookup"><span data-stu-id="b7782-149">Int32</span></span>|<span data-ttu-id="b7782-150">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="b7782-150">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="b7782-151">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="b7782-151">Allowed values are 5 or 1000.</span></span>|


## <a name="relationships"></a><span data-ttu-id="b7782-152">关系</span><span class="sxs-lookup"><span data-stu-id="b7782-152">Relationships</span></span>
|<span data-ttu-id="b7782-153">关系</span><span class="sxs-lookup"><span data-stu-id="b7782-153">Relationship</span></span>|<span data-ttu-id="b7782-154">类型</span><span class="sxs-lookup"><span data-stu-id="b7782-154">Type</span></span>|<span data-ttu-id="b7782-155">说明</span><span class="sxs-lookup"><span data-stu-id="b7782-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7782-156">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="b7782-156">**Device management**</span></span>|
|<span data-ttu-id="b7782-157">managedDevices</span><span class="sxs-lookup"><span data-stu-id="b7782-157">managedDevices</span></span>|<span data-ttu-id="b7782-158">[managedDevice](../resources/intune-devices-manageddevice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b7782-158">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="b7782-159">与用户关联的管理设备。</span><span class="sxs-lookup"><span data-stu-id="b7782-159">The managed devices associated with the user.</span></span>|
|<span data-ttu-id="b7782-160">**移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="b7782-160">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="b7782-161">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="b7782-161">managedAppRegistrations</span></span>|<span data-ttu-id="b7782-162">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b7782-162">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="b7782-163">属于用户的零个或多个托管的应用注册。</span><span class="sxs-lookup"><span data-stu-id="b7782-163">Zero or more managed app registrations that belong to the user.</span></span>|
|<span data-ttu-id="b7782-164">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="b7782-164">**Troubleshooting**</span></span>|
|<span data-ttu-id="b7782-165">deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="b7782-165">deviceManagementTroubleshootingEvents</span></span>|<span data-ttu-id="b7782-166">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b7782-166">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="b7782-167">此用户的故障排除事件列表。</span><span class="sxs-lookup"><span data-stu-id="b7782-167">The list of troubleshooting events for this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7782-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b7782-168">JSON Representation</span></span>
<span data-ttu-id="b7782-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7782-169">Here is a JSON representation of the resource.</span></span>
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

