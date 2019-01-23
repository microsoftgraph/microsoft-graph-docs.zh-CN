---
title: 更新 targetedManagedAppPolicyAssignment
description: 更新 targetedManagedAppPolicyAssignment 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: da22dcaa56691e3e248664ca32941e29eaa9100a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401493"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="bc9cc-103">更新 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="bc9cc-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="bc9cc-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="bc9cc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bc9cc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bc9cc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc9cc-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bc9cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc9cc-107">更新 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bc9cc-107">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc9cc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bc9cc-108">Prerequisites</span></span>
<span data-ttu-id="bc9cc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="bc9cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bc9cc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc9cc-111">Permission type</span></span>|<span data-ttu-id="bc9cc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bc9cc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc9cc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc9cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc9cc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc9cc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bc9cc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc9cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc9cc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc9cc-116">Not supported.</span></span>|
|<span data-ttu-id="bc9cc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc9cc-117">Application</span></span>|<span data-ttu-id="bc9cc-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc9cc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc9cc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc9cc-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="bc9cc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc9cc-120">Request headers</span></span>
|<span data-ttu-id="bc9cc-121">标头</span><span class="sxs-lookup"><span data-stu-id="bc9cc-121">Header</span></span>|<span data-ttu-id="bc9cc-122">值</span><span class="sxs-lookup"><span data-stu-id="bc9cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc9cc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc9cc-123">Authorization</span></span>|<span data-ttu-id="bc9cc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bc9cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc9cc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bc9cc-125">Accept</span></span>|<span data-ttu-id="bc9cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc9cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc9cc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc9cc-127">Request body</span></span>
<span data-ttu-id="bc9cc-128">在请求正文中，提供 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc9cc-128">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="bc9cc-129">下表显示创建 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bc9cc-129">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="bc9cc-130">属性</span><span class="sxs-lookup"><span data-stu-id="bc9cc-130">Property</span></span>|<span data-ttu-id="bc9cc-131">类型</span><span class="sxs-lookup"><span data-stu-id="bc9cc-131">Type</span></span>|<span data-ttu-id="bc9cc-132">说明</span><span class="sxs-lookup"><span data-stu-id="bc9cc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc9cc-133">id</span><span class="sxs-lookup"><span data-stu-id="bc9cc-133">id</span></span>|<span data-ttu-id="bc9cc-134">String</span><span class="sxs-lookup"><span data-stu-id="bc9cc-134">String</span></span>|<span data-ttu-id="bc9cc-135">Id</span><span class="sxs-lookup"><span data-stu-id="bc9cc-135">Id</span></span>|
|<span data-ttu-id="bc9cc-136">target</span><span class="sxs-lookup"><span data-stu-id="bc9cc-136">target</span></span>|[<span data-ttu-id="bc9cc-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bc9cc-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="bc9cc-138">组或应用的部署标识符</span><span class="sxs-lookup"><span data-stu-id="bc9cc-138">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="bc9cc-139">响应</span><span class="sxs-lookup"><span data-stu-id="bc9cc-139">Response</span></span>
<span data-ttu-id="bc9cc-140">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bc9cc-140">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc9cc-141">示例</span><span class="sxs-lookup"><span data-stu-id="bc9cc-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc9cc-142">请求</span><span class="sxs-lookup"><span data-stu-id="bc9cc-142">Request</span></span>
<span data-ttu-id="bc9cc-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bc9cc-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="bc9cc-144">响应</span><span class="sxs-lookup"><span data-stu-id="bc9cc-144">Response</span></span>
<span data-ttu-id="bc9cc-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bc9cc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




