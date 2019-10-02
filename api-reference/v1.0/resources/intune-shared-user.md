---
title: 用户资源类型
description: 表示 Azure Active Directory 用户对象。
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 15fca0cedc6fe1da81da25688bbc447c1f8f475f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360102"
---
# <a name="user-resource-type"></a><span data-ttu-id="c9bcb-103">用户资源类型</span><span class="sxs-lookup"><span data-stu-id="c9bcb-103">user resource type</span></span>

> <span data-ttu-id="c9bcb-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9bcb-105">表示 Azure Active Directory 用户对象。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-105">Represents an Azure Active Directory user object.</span></span>

## <a name="methods"></a><span data-ttu-id="c9bcb-106">方法</span><span class="sxs-lookup"><span data-stu-id="c9bcb-106">Methods</span></span>
|<span data-ttu-id="c9bcb-107">方法</span><span class="sxs-lookup"><span data-stu-id="c9bcb-107">Method</span></span>|<span data-ttu-id="c9bcb-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="c9bcb-108">Return Type</span></span>|<span data-ttu-id="c9bcb-109">说明</span><span class="sxs-lookup"><span data-stu-id="c9bcb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9bcb-110">[列出用户](../api/intune-shared-user-list.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-110">[List users](../api/intune-shared-user-list.md) objects.</span></span>|<span data-ttu-id="c9bcb-111">[user](../resources/intune-shared-user.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9bcb-111">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="c9bcb-112">列出 [user](../resources/intune-shared-user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-112">List properties and relationships of the [user](../resources/intune-shared-user.md) objects.</span></span>|
|<span data-ttu-id="c9bcb-113">[获取用户](../api/intune-shared-user-get.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-113">[Get user](../api/intune-shared-user-get.md) object.</span></span>|<span data-ttu-id="c9bcb-114">[user](../resources/intune-shared-user.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9bcb-114">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="c9bcb-115">读取 [user](../resources/intune-shared-user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-115">Read properties and relationships of the [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="c9bcb-116">[创建用户](../api/intune-shared-user-create.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-116">[Create user](../api/intune-shared-user-create.md) object.</span></span>|<span data-ttu-id="c9bcb-117">[user](../resources/intune-shared-user.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9bcb-117">[user](../resources/intune-shared-user.md) collection</span></span>|<span data-ttu-id="c9bcb-118">创建新的 [user](../resources/intune-shared-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-118">Create a new [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="c9bcb-119">[删除用户](../api/intune-shared-user-delete.md)。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-119">[Delete user](../api/intune-shared-user-delete.md).</span></span>|<span data-ttu-id="c9bcb-120">无</span><span class="sxs-lookup"><span data-stu-id="c9bcb-120">None</span></span>|<span data-ttu-id="c9bcb-121">删除 [user](../resources/intune-shared-user.md)。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-121">Deletes a [user](../resources/intune-shared-user.md).</span></span>|
|<span data-ttu-id="c9bcb-122">[更新 user](../api/intune-shared-user-update.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-122">[Update user](../api/intune-shared-user-update.md) object.</span></span>|[<span data-ttu-id="c9bcb-123">user</span><span class="sxs-lookup"><span data-stu-id="c9bcb-123">user</span></span>](../resources/intune-shared-user.md)|<span data-ttu-id="c9bcb-124">更新 [user](../resources/intune-shared-user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-124">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>|
|<span data-ttu-id="c9bcb-125">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="c9bcb-125">**Device management**</span></span>|
|[<span data-ttu-id="c9bcb-126">removeAllDevicesFromManagement 操作</span><span class="sxs-lookup"><span data-stu-id="c9bcb-126">removeAllDevicesFromManagement action</span></span>](../api/intune-shared-user-removealldevicesfrommanagement.md)|<span data-ttu-id="c9bcb-127">无</span><span class="sxs-lookup"><span data-stu-id="c9bcb-127">None</span></span>|<span data-ttu-id="c9bcb-128">停用该用户管理的所有设备</span><span class="sxs-lookup"><span data-stu-id="c9bcb-128">Retire all devices from management for this user</span></span>|
|<span data-ttu-id="c9bcb-129">**移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="c9bcb-129">**Mobile app management (MAM)**</span></span>|
|[<span data-ttu-id="c9bcb-130">getManagedAppDiagnosticStatuses 函数</span><span class="sxs-lookup"><span data-stu-id="c9bcb-130">getManagedAppDiagnosticStatuses function</span></span>](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="c9bcb-131">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9bcb-131">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="c9bcb-132">获取给定用户的诊断验证状态。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-132">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="c9bcb-133">getManagedAppPolicies 函数</span><span class="sxs-lookup"><span data-stu-id="c9bcb-133">getManagedAppPolicies function</span></span>](../api/intune-shared-user-getmanagedapppolicies.md)|<span data-ttu-id="c9bcb-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9bcb-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="c9bcb-135">获取给定用户的应用限制。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-135">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="c9bcb-136">wipeManagedAppRegistrationsByDeviceTag 操作</span><span class="sxs-lookup"><span data-stu-id="c9bcb-136">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="c9bcb-137">无</span><span class="sxs-lookup"><span data-stu-id="c9bcb-137">None</span></span>|<span data-ttu-id="c9bcb-138">对含有指定设备标记的应用注册发布擦除操作。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-138">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="c9bcb-139">属性</span><span class="sxs-lookup"><span data-stu-id="c9bcb-139">Properties</span></span>
|<span data-ttu-id="c9bcb-140">属性</span><span class="sxs-lookup"><span data-stu-id="c9bcb-140">Property</span></span>|<span data-ttu-id="c9bcb-141">类型</span><span class="sxs-lookup"><span data-stu-id="c9bcb-141">Type</span></span>|<span data-ttu-id="c9bcb-142">说明</span><span class="sxs-lookup"><span data-stu-id="c9bcb-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9bcb-143">id</span><span class="sxs-lookup"><span data-stu-id="c9bcb-143">id</span></span>|<span data-ttu-id="c9bcb-144">String</span><span class="sxs-lookup"><span data-stu-id="c9bcb-144">String</span></span>|<span data-ttu-id="c9bcb-145">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-145">Unique identifier of the user.</span></span>|
|<span data-ttu-id="c9bcb-146">**载入**</span><span class="sxs-lookup"><span data-stu-id="c9bcb-146">**Onboarding**</span></span>|
|<span data-ttu-id="c9bcb-147">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="c9bcb-147">deviceEnrollmentLimit</span></span>|<span data-ttu-id="c9bcb-148">Int32</span><span class="sxs-lookup"><span data-stu-id="c9bcb-148">Int32</span></span>|<span data-ttu-id="c9bcb-149">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-149">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="c9bcb-150">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-150">Allowed values are 5 or 1000.</span></span>|


## <a name="relationships"></a><span data-ttu-id="c9bcb-151">关系</span><span class="sxs-lookup"><span data-stu-id="c9bcb-151">Relationships</span></span>
|<span data-ttu-id="c9bcb-152">关系</span><span class="sxs-lookup"><span data-stu-id="c9bcb-152">Relationship</span></span>|<span data-ttu-id="c9bcb-153">类型</span><span class="sxs-lookup"><span data-stu-id="c9bcb-153">Type</span></span>|<span data-ttu-id="c9bcb-154">说明</span><span class="sxs-lookup"><span data-stu-id="c9bcb-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9bcb-155">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="c9bcb-155">**Device management**</span></span>|
|<span data-ttu-id="c9bcb-156">managedDevices</span><span class="sxs-lookup"><span data-stu-id="c9bcb-156">managedDevices</span></span>|<span data-ttu-id="c9bcb-157">[managedDevice](../resources/intune-devices-manageddevice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9bcb-157">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="c9bcb-158">与用户关联的管理设备。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-158">The managed devices associated with the user.</span></span>|
|<span data-ttu-id="c9bcb-159">**移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="c9bcb-159">**Mobile app management (MAM)**</span></span>|
|<span data-ttu-id="c9bcb-160">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="c9bcb-160">managedAppRegistrations</span></span>|<span data-ttu-id="c9bcb-161">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9bcb-161">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="c9bcb-162">属于用户的零个或多个托管的应用注册。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-162">Zero or more managed app registrations that belong to the user.</span></span>|
|<span data-ttu-id="c9bcb-163">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="c9bcb-163">**Troubleshooting**</span></span>|
|<span data-ttu-id="c9bcb-164">deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="c9bcb-164">deviceManagementTroubleshootingEvents</span></span>|<span data-ttu-id="c9bcb-165">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9bcb-165">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) collection</span></span>|<span data-ttu-id="c9bcb-166">此用户的故障排除事件列表。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-166">The list of troubleshooting events for this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9bcb-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9bcb-167">JSON Representation</span></span>
<span data-ttu-id="c9bcb-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9bcb-168">Here is a JSON representation of the resource.</span></span>
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

