---
title: 更新 targetedManagedAppPolicyAssignment
description: 更新 targetedManagedAppPolicyAssignment 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2beaa0f25b5000eb02fdc4942a63b66e58f8549d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018111"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="b828b-103">更新 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="b828b-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="b828b-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b828b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b828b-105">更新 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b828b-105">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b828b-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="b828b-106">Prerequisites</span></span>
<span data-ttu-id="b828b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b828b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b828b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b828b-109">Permission type</span></span>|<span data-ttu-id="b828b-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b828b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b828b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b828b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b828b-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b828b-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b828b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b828b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b828b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b828b-114">Not supported.</span></span>|
|<span data-ttu-id="b828b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b828b-115">Application</span></span>|<span data-ttu-id="b828b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b828b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b828b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b828b-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b828b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b828b-118">Request headers</span></span>
|<span data-ttu-id="b828b-119">标头</span><span class="sxs-lookup"><span data-stu-id="b828b-119">Header</span></span>|<span data-ttu-id="b828b-120">值</span><span class="sxs-lookup"><span data-stu-id="b828b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b828b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b828b-121">Authorization</span></span>|<span data-ttu-id="b828b-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b828b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b828b-123">接受</span><span class="sxs-lookup"><span data-stu-id="b828b-123">Accept</span></span>|<span data-ttu-id="b828b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b828b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b828b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b828b-125">Request body</span></span>
<span data-ttu-id="b828b-126">在请求正文中，提供 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b828b-126">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="b828b-127">下表显示创建 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b828b-127">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="b828b-128">属性</span><span class="sxs-lookup"><span data-stu-id="b828b-128">Property</span></span>|<span data-ttu-id="b828b-129">类型</span><span class="sxs-lookup"><span data-stu-id="b828b-129">Type</span></span>|<span data-ttu-id="b828b-130">说明</span><span class="sxs-lookup"><span data-stu-id="b828b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b828b-131">id</span><span class="sxs-lookup"><span data-stu-id="b828b-131">id</span></span>|<span data-ttu-id="b828b-132">String</span><span class="sxs-lookup"><span data-stu-id="b828b-132">String</span></span>|<span data-ttu-id="b828b-133">Id</span><span class="sxs-lookup"><span data-stu-id="b828b-133">Id</span></span>|
|<span data-ttu-id="b828b-134">target</span><span class="sxs-lookup"><span data-stu-id="b828b-134">target</span></span>|[<span data-ttu-id="b828b-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b828b-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b828b-136">组或应用的部署标识符</span><span class="sxs-lookup"><span data-stu-id="b828b-136">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="b828b-137">响应</span><span class="sxs-lookup"><span data-stu-id="b828b-137">Response</span></span>
<span data-ttu-id="b828b-138">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b828b-138">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b828b-139">示例</span><span class="sxs-lookup"><span data-stu-id="b828b-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="b828b-140">请求</span><span class="sxs-lookup"><span data-stu-id="b828b-140">Request</span></span>
<span data-ttu-id="b828b-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b828b-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b828b-142">响应</span><span class="sxs-lookup"><span data-stu-id="b828b-142">Response</span></span>
<span data-ttu-id="b828b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b828b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



