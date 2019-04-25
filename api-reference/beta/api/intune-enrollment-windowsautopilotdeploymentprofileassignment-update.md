---
title: 更新 windowsAutopilotDeploymentProfileAssignment
description: 更新 windowsAutopilotDeploymentProfileAssignment 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 562ae8b137754acc3475ba98fb335a4f7e7310dd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532658"
---
# <a name="update-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="b8dd3-103">更新 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="b8dd3-103">Update windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="b8dd3-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b8dd3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8dd3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b8dd3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8dd3-106">更新[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b8dd3-106">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8dd3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b8dd3-107">Prerequisites</span></span>
<span data-ttu-id="b8dd3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b8dd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8dd3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8dd3-110">Permission type</span></span>|<span data-ttu-id="b8dd3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b8dd3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8dd3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8dd3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b8dd3-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8dd3-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b8dd3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8dd3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8dd3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8dd3-115">Not supported.</span></span>|
|<span data-ttu-id="b8dd3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8dd3-116">Application</span></span>|<span data-ttu-id="b8dd3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8dd3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8dd3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8dd3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b8dd3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8dd3-119">Request headers</span></span>
|<span data-ttu-id="b8dd3-120">标头</span><span class="sxs-lookup"><span data-stu-id="b8dd3-120">Header</span></span>|<span data-ttu-id="b8dd3-121">值</span><span class="sxs-lookup"><span data-stu-id="b8dd3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8dd3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8dd3-122">Authorization</span></span>|<span data-ttu-id="b8dd3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b8dd3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8dd3-124">接受</span><span class="sxs-lookup"><span data-stu-id="b8dd3-124">Accept</span></span>|<span data-ttu-id="b8dd3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b8dd3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8dd3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8dd3-126">Request body</span></span>
<span data-ttu-id="b8dd3-127">在请求正文中, 提供[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8dd3-127">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

<span data-ttu-id="b8dd3-128">下表显示创建[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b8dd3-128">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

|<span data-ttu-id="b8dd3-129">属性</span><span class="sxs-lookup"><span data-stu-id="b8dd3-129">Property</span></span>|<span data-ttu-id="b8dd3-130">类型</span><span class="sxs-lookup"><span data-stu-id="b8dd3-130">Type</span></span>|<span data-ttu-id="b8dd3-131">说明</span><span class="sxs-lookup"><span data-stu-id="b8dd3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8dd3-132">id</span><span class="sxs-lookup"><span data-stu-id="b8dd3-132">id</span></span>|<span data-ttu-id="b8dd3-133">String</span><span class="sxs-lookup"><span data-stu-id="b8dd3-133">String</span></span>|<span data-ttu-id="b8dd3-134">分配的键。</span><span class="sxs-lookup"><span data-stu-id="b8dd3-134">The key of the assignment.</span></span>|
|<span data-ttu-id="b8dd3-135">target</span><span class="sxs-lookup"><span data-stu-id="b8dd3-135">target</span></span>|[<span data-ttu-id="b8dd3-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b8dd3-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b8dd3-137">Windows Autopilot 部署配置文件的分配目标。</span><span class="sxs-lookup"><span data-stu-id="b8dd3-137">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="b8dd3-138">响应</span><span class="sxs-lookup"><span data-stu-id="b8dd3-138">Response</span></span>
<span data-ttu-id="b8dd3-139">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b8dd3-139">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8dd3-140">示例</span><span class="sxs-lookup"><span data-stu-id="b8dd3-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8dd3-141">请求</span><span class="sxs-lookup"><span data-stu-id="b8dd3-141">Request</span></span>
<span data-ttu-id="b8dd3-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b8dd3-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="b8dd3-143">响应</span><span class="sxs-lookup"><span data-stu-id="b8dd3-143">Response</span></span>
<span data-ttu-id="b8dd3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b8dd3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "id": "de7e1e1e-1e1e-de7e-1e1e-7ede1e1e7ede",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





