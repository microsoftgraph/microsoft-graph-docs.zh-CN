---
title: 创建 windowsAutopilotDeploymentProfileAssignment
description: 创建新的 windowsAutopilotDeploymentProfileAssignment 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bff01991a56b5a4fd6c63f591fb973c430987e98
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37187735"
---
# <a name="create-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="26ca8-103">创建 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="26ca8-103">Create windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="26ca8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="26ca8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26ca8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="26ca8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26ca8-106">创建新的[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="26ca8-106">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26ca8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="26ca8-107">Prerequisites</span></span>
<span data-ttu-id="26ca8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26ca8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26ca8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="26ca8-110">Permission type</span></span>|<span data-ttu-id="26ca8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="26ca8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26ca8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26ca8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26ca8-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26ca8-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="26ca8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26ca8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26ca8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="26ca8-115">Not supported.</span></span>|
|<span data-ttu-id="26ca8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="26ca8-116">Application</span></span>|<span data-ttu-id="26ca8-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26ca8-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26ca8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26ca8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="26ca8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="26ca8-119">Request headers</span></span>
|<span data-ttu-id="26ca8-120">标头</span><span class="sxs-lookup"><span data-stu-id="26ca8-120">Header</span></span>|<span data-ttu-id="26ca8-121">值</span><span class="sxs-lookup"><span data-stu-id="26ca8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26ca8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="26ca8-122">Authorization</span></span>|<span data-ttu-id="26ca8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="26ca8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26ca8-124">接受</span><span class="sxs-lookup"><span data-stu-id="26ca8-124">Accept</span></span>|<span data-ttu-id="26ca8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26ca8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26ca8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="26ca8-126">Request body</span></span>
<span data-ttu-id="26ca8-127">在请求正文中，提供 windowsAutopilotDeploymentProfileAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26ca8-127">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfileAssignment object.</span></span>

<span data-ttu-id="26ca8-128">下表显示创建 windowsAutopilotDeploymentProfileAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="26ca8-128">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfileAssignment.</span></span>

|<span data-ttu-id="26ca8-129">属性</span><span class="sxs-lookup"><span data-stu-id="26ca8-129">Property</span></span>|<span data-ttu-id="26ca8-130">类型</span><span class="sxs-lookup"><span data-stu-id="26ca8-130">Type</span></span>|<span data-ttu-id="26ca8-131">说明</span><span class="sxs-lookup"><span data-stu-id="26ca8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26ca8-132">id</span><span class="sxs-lookup"><span data-stu-id="26ca8-132">id</span></span>|<span data-ttu-id="26ca8-133">String</span><span class="sxs-lookup"><span data-stu-id="26ca8-133">String</span></span>|<span data-ttu-id="26ca8-134">分配的键。</span><span class="sxs-lookup"><span data-stu-id="26ca8-134">The key of the assignment.</span></span>|
|<span data-ttu-id="26ca8-135">target</span><span class="sxs-lookup"><span data-stu-id="26ca8-135">target</span></span>|[<span data-ttu-id="26ca8-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="26ca8-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="26ca8-137">Windows Autopilot 部署配置文件的分配目标。</span><span class="sxs-lookup"><span data-stu-id="26ca8-137">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="26ca8-138">响应</span><span class="sxs-lookup"><span data-stu-id="26ca8-138">Response</span></span>
<span data-ttu-id="26ca8-139">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="26ca8-139">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26ca8-140">示例</span><span class="sxs-lookup"><span data-stu-id="26ca8-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="26ca8-141">请求</span><span class="sxs-lookup"><span data-stu-id="26ca8-141">Request</span></span>
<span data-ttu-id="26ca8-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="26ca8-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="26ca8-143">响应</span><span class="sxs-lookup"><span data-stu-id="26ca8-143">Response</span></span>
<span data-ttu-id="26ca8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="26ca8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




