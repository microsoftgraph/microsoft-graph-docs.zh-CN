---
title: 更新 targetedManagedAppPolicyAssignment
description: 更新 targetedManagedAppPolicyAssignment 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32e03d719a631e1237eafac4404f9a9607dde188
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988054"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="3c706-103">更新 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="3c706-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="3c706-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3c706-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c706-105">更新 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3c706-105">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c706-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="3c706-106">Prerequisites</span></span>
<span data-ttu-id="3c706-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c706-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c706-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c706-109">Permission type</span></span>|<span data-ttu-id="3c706-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3c706-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c706-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c706-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3c706-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c706-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3c706-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c706-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c706-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c706-114">Not supported.</span></span>|
|<span data-ttu-id="3c706-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c706-115">Application</span></span>|<span data-ttu-id="3c706-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c706-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c706-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c706-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="3c706-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c706-118">Request headers</span></span>
|<span data-ttu-id="3c706-119">标头</span><span class="sxs-lookup"><span data-stu-id="3c706-119">Header</span></span>|<span data-ttu-id="3c706-120">值</span><span class="sxs-lookup"><span data-stu-id="3c706-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c706-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c706-121">Authorization</span></span>|<span data-ttu-id="3c706-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3c706-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c706-123">接受</span><span class="sxs-lookup"><span data-stu-id="3c706-123">Accept</span></span>|<span data-ttu-id="3c706-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3c706-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c706-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c706-125">Request body</span></span>
<span data-ttu-id="3c706-126">在请求正文中，提供 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c706-126">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="3c706-127">下表显示创建 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3c706-127">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="3c706-128">属性</span><span class="sxs-lookup"><span data-stu-id="3c706-128">Property</span></span>|<span data-ttu-id="3c706-129">类型</span><span class="sxs-lookup"><span data-stu-id="3c706-129">Type</span></span>|<span data-ttu-id="3c706-130">说明</span><span class="sxs-lookup"><span data-stu-id="3c706-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c706-131">id</span><span class="sxs-lookup"><span data-stu-id="3c706-131">id</span></span>|<span data-ttu-id="3c706-132">String</span><span class="sxs-lookup"><span data-stu-id="3c706-132">String</span></span>|<span data-ttu-id="3c706-133">Id</span><span class="sxs-lookup"><span data-stu-id="3c706-133">Id</span></span>|
|<span data-ttu-id="3c706-134">target</span><span class="sxs-lookup"><span data-stu-id="3c706-134">target</span></span>|[<span data-ttu-id="3c706-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3c706-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3c706-136">组或应用的部署标识符</span><span class="sxs-lookup"><span data-stu-id="3c706-136">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="3c706-137">响应</span><span class="sxs-lookup"><span data-stu-id="3c706-137">Response</span></span>
<span data-ttu-id="3c706-138">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3c706-138">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c706-139">示例</span><span class="sxs-lookup"><span data-stu-id="3c706-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c706-140">请求</span><span class="sxs-lookup"><span data-stu-id="3c706-140">Request</span></span>
<span data-ttu-id="3c706-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3c706-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="3c706-142">响应</span><span class="sxs-lookup"><span data-stu-id="3c706-142">Response</span></span>
<span data-ttu-id="3c706-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3c706-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 223

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



