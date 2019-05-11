---
title: 创建 windowsAutopilotDeploymentProfileAssignment
description: 创建新的 windowsAutopilotDeploymentProfileAssignment 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a27cdc87070bda020a9d2e2a6ba0fc5ed99ef101
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909139"
---
# <a name="create-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="c0c1f-103">创建 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="c0c1f-103">Create windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="c0c1f-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c0c1f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0c1f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c0c1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0c1f-106">创建新的[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c0c1f-106">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0c1f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c0c1f-107">Prerequisites</span></span>
<span data-ttu-id="c0c1f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0c1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0c1f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0c1f-110">Permission type</span></span>|<span data-ttu-id="c0c1f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c0c1f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0c1f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0c1f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c0c1f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0c1f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c0c1f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0c1f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0c1f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0c1f-115">Not supported.</span></span>|
|<span data-ttu-id="c0c1f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0c1f-116">Application</span></span>|<span data-ttu-id="c0c1f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0c1f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0c1f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0c1f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="c0c1f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0c1f-119">Request headers</span></span>
|<span data-ttu-id="c0c1f-120">标头</span><span class="sxs-lookup"><span data-stu-id="c0c1f-120">Header</span></span>|<span data-ttu-id="c0c1f-121">值</span><span class="sxs-lookup"><span data-stu-id="c0c1f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0c1f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0c1f-122">Authorization</span></span>|<span data-ttu-id="c0c1f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c0c1f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0c1f-124">接受</span><span class="sxs-lookup"><span data-stu-id="c0c1f-124">Accept</span></span>|<span data-ttu-id="c0c1f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c0c1f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0c1f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0c1f-126">Request body</span></span>
<span data-ttu-id="c0c1f-127">在请求正文中, 提供 windowsAutopilotDeploymentProfileAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0c1f-127">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfileAssignment object.</span></span>

<span data-ttu-id="c0c1f-128">下表显示创建 windowsAutopilotDeploymentProfileAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c0c1f-128">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfileAssignment.</span></span>

|<span data-ttu-id="c0c1f-129">属性</span><span class="sxs-lookup"><span data-stu-id="c0c1f-129">Property</span></span>|<span data-ttu-id="c0c1f-130">类型</span><span class="sxs-lookup"><span data-stu-id="c0c1f-130">Type</span></span>|<span data-ttu-id="c0c1f-131">说明</span><span class="sxs-lookup"><span data-stu-id="c0c1f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0c1f-132">id</span><span class="sxs-lookup"><span data-stu-id="c0c1f-132">id</span></span>|<span data-ttu-id="c0c1f-133">String</span><span class="sxs-lookup"><span data-stu-id="c0c1f-133">String</span></span>|<span data-ttu-id="c0c1f-134">分配的键。</span><span class="sxs-lookup"><span data-stu-id="c0c1f-134">The key of the assignment.</span></span>|
|<span data-ttu-id="c0c1f-135">target</span><span class="sxs-lookup"><span data-stu-id="c0c1f-135">target</span></span>|[<span data-ttu-id="c0c1f-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c0c1f-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c0c1f-137">Windows Autopilot 部署配置文件的分配目标。</span><span class="sxs-lookup"><span data-stu-id="c0c1f-137">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="c0c1f-138">响应</span><span class="sxs-lookup"><span data-stu-id="c0c1f-138">Response</span></span>
<span data-ttu-id="c0c1f-139">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c0c1f-139">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0c1f-140">示例</span><span class="sxs-lookup"><span data-stu-id="c0c1f-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0c1f-141">请求</span><span class="sxs-lookup"><span data-stu-id="c0c1f-141">Request</span></span>
<span data-ttu-id="c0c1f-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0c1f-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="c0c1f-143">响应</span><span class="sxs-lookup"><span data-stu-id="c0c1f-143">Response</span></span>
<span data-ttu-id="c0c1f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c0c1f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




