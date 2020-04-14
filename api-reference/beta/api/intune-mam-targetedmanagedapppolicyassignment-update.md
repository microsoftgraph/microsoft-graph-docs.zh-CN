---
title: 更新 targetedManagedAppPolicyAssignment
description: 更新 targetedManagedAppPolicyAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5fb591b2d1ccbc22260e21c0be73f52d62ae0b44
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448808"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="a6d00-103">更新 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="a6d00-103">Update targetedManagedAppPolicyAssignment</span></span>

<span data-ttu-id="a6d00-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6d00-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6d00-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a6d00-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6d00-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6d00-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6d00-107">更新 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a6d00-107">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6d00-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a6d00-108">Prerequisites</span></span>
<span data-ttu-id="a6d00-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6d00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6d00-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6d00-111">Permission type</span></span>|<span data-ttu-id="a6d00-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a6d00-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6d00-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6d00-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6d00-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6d00-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a6d00-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6d00-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6d00-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6d00-116">Not supported.</span></span>|
|<span data-ttu-id="a6d00-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6d00-117">Application</span></span>|<span data-ttu-id="a6d00-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6d00-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6d00-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6d00-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="a6d00-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6d00-120">Request headers</span></span>
|<span data-ttu-id="a6d00-121">标头</span><span class="sxs-lookup"><span data-stu-id="a6d00-121">Header</span></span>|<span data-ttu-id="a6d00-122">值</span><span class="sxs-lookup"><span data-stu-id="a6d00-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6d00-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6d00-123">Authorization</span></span>|<span data-ttu-id="a6d00-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a6d00-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6d00-125">接受</span><span class="sxs-lookup"><span data-stu-id="a6d00-125">Accept</span></span>|<span data-ttu-id="a6d00-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6d00-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6d00-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6d00-127">Request body</span></span>
<span data-ttu-id="a6d00-128">在请求正文中，提供 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6d00-128">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="a6d00-129">下表显示创建 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a6d00-129">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="a6d00-130">属性</span><span class="sxs-lookup"><span data-stu-id="a6d00-130">Property</span></span>|<span data-ttu-id="a6d00-131">类型</span><span class="sxs-lookup"><span data-stu-id="a6d00-131">Type</span></span>|<span data-ttu-id="a6d00-132">说明</span><span class="sxs-lookup"><span data-stu-id="a6d00-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6d00-133">id</span><span class="sxs-lookup"><span data-stu-id="a6d00-133">id</span></span>|<span data-ttu-id="a6d00-134">String</span><span class="sxs-lookup"><span data-stu-id="a6d00-134">String</span></span>|<span data-ttu-id="a6d00-135">Id</span><span class="sxs-lookup"><span data-stu-id="a6d00-135">Id</span></span>|
|<span data-ttu-id="a6d00-136">target</span><span class="sxs-lookup"><span data-stu-id="a6d00-136">target</span></span>|[<span data-ttu-id="a6d00-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a6d00-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a6d00-138">用于部署到组或应用的标识符</span><span class="sxs-lookup"><span data-stu-id="a6d00-138">Identifier for deployment to a group or app</span></span>|
|<span data-ttu-id="a6d00-139">source</span><span class="sxs-lookup"><span data-stu-id="a6d00-139">source</span></span>|[<span data-ttu-id="a6d00-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="a6d00-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="a6d00-141">用于部署到组、direct 或包裹/policySet 的资源类型。</span><span class="sxs-lookup"><span data-stu-id="a6d00-141">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="a6d00-142">可取值为：`direct`、`policySets`。</span><span class="sxs-lookup"><span data-stu-id="a6d00-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="a6d00-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="a6d00-143">sourceId</span></span>|<span data-ttu-id="a6d00-144">String</span><span class="sxs-lookup"><span data-stu-id="a6d00-144">String</span></span>|<span data-ttu-id="a6d00-145">用于部署到组的资源的标识符</span><span class="sxs-lookup"><span data-stu-id="a6d00-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="a6d00-146">响应</span><span class="sxs-lookup"><span data-stu-id="a6d00-146">Response</span></span>
<span data-ttu-id="a6d00-147">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a6d00-147">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6d00-148">示例</span><span class="sxs-lookup"><span data-stu-id="a6d00-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6d00-149">请求</span><span class="sxs-lookup"><span data-stu-id="a6d00-149">Request</span></span>
<span data-ttu-id="a6d00-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a6d00-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 235

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="a6d00-151">响应</span><span class="sxs-lookup"><span data-stu-id="a6d00-151">Response</span></span>
<span data-ttu-id="a6d00-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a6d00-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 284

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```



