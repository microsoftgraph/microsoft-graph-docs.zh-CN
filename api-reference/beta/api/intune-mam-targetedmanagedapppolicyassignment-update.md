---
title: 更新 targetedManagedAppPolicyAssignment
description: 更新 targetedManagedAppPolicyAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 923b0a6e26e13a8a8b51998ad027ecb7276dd8f8
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791901"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="e18da-103">更新 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="e18da-103">Update targetedManagedAppPolicyAssignment</span></span>

<span data-ttu-id="e18da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e18da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e18da-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e18da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e18da-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e18da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e18da-107">更新 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e18da-107">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e18da-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e18da-108">Prerequisites</span></span>
<span data-ttu-id="e18da-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e18da-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e18da-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e18da-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e18da-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e18da-111">Permission type</span></span>|<span data-ttu-id="e18da-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e18da-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e18da-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e18da-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e18da-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e18da-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e18da-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e18da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e18da-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e18da-116">Not supported.</span></span>|
|<span data-ttu-id="e18da-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e18da-117">Application</span></span>|<span data-ttu-id="e18da-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e18da-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e18da-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e18da-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e18da-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e18da-120">Request headers</span></span>
|<span data-ttu-id="e18da-121">标头</span><span class="sxs-lookup"><span data-stu-id="e18da-121">Header</span></span>|<span data-ttu-id="e18da-122">值</span><span class="sxs-lookup"><span data-stu-id="e18da-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e18da-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e18da-123">Authorization</span></span>|<span data-ttu-id="e18da-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e18da-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e18da-125">接受</span><span class="sxs-lookup"><span data-stu-id="e18da-125">Accept</span></span>|<span data-ttu-id="e18da-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e18da-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e18da-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e18da-127">Request body</span></span>
<span data-ttu-id="e18da-128">在请求正文中，提供 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e18da-128">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="e18da-129">下表显示创建 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e18da-129">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="e18da-130">属性</span><span class="sxs-lookup"><span data-stu-id="e18da-130">Property</span></span>|<span data-ttu-id="e18da-131">类型</span><span class="sxs-lookup"><span data-stu-id="e18da-131">Type</span></span>|<span data-ttu-id="e18da-132">说明</span><span class="sxs-lookup"><span data-stu-id="e18da-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e18da-133">id</span><span class="sxs-lookup"><span data-stu-id="e18da-133">id</span></span>|<span data-ttu-id="e18da-134">String</span><span class="sxs-lookup"><span data-stu-id="e18da-134">String</span></span>|<span data-ttu-id="e18da-135">Id</span><span class="sxs-lookup"><span data-stu-id="e18da-135">Id</span></span>|
|<span data-ttu-id="e18da-136">target</span><span class="sxs-lookup"><span data-stu-id="e18da-136">target</span></span>|[<span data-ttu-id="e18da-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e18da-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e18da-138">用于部署到组或应用的标识符</span><span class="sxs-lookup"><span data-stu-id="e18da-138">Identifier for deployment to a group or app</span></span>|
|<span data-ttu-id="e18da-139">source</span><span class="sxs-lookup"><span data-stu-id="e18da-139">source</span></span>|[<span data-ttu-id="e18da-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="e18da-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="e18da-141">用于部署到组、direct 或包裹/policySet 的资源类型。</span><span class="sxs-lookup"><span data-stu-id="e18da-141">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="e18da-142">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="e18da-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="e18da-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="e18da-143">sourceId</span></span>|<span data-ttu-id="e18da-144">String</span><span class="sxs-lookup"><span data-stu-id="e18da-144">String</span></span>|<span data-ttu-id="e18da-145">用于部署到组的资源的标识符</span><span class="sxs-lookup"><span data-stu-id="e18da-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="e18da-146">响应</span><span class="sxs-lookup"><span data-stu-id="e18da-146">Response</span></span>
<span data-ttu-id="e18da-147">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e18da-147">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e18da-148">示例</span><span class="sxs-lookup"><span data-stu-id="e18da-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="e18da-149">请求</span><span class="sxs-lookup"><span data-stu-id="e18da-149">Request</span></span>
<span data-ttu-id="e18da-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e18da-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 390

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="e18da-151">响应</span><span class="sxs-lookup"><span data-stu-id="e18da-151">Response</span></span>
<span data-ttu-id="e18da-152">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="e18da-152">Here is an example of the response.</span></span> <span data-ttu-id="e18da-153">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="e18da-153">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e18da-154">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="e18da-154">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```



