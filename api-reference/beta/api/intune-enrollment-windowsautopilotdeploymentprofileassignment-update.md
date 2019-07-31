---
title: 更新 windowsAutopilotDeploymentProfileAssignment
description: 更新 windowsAutopilotDeploymentProfileAssignment 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 620895db33ddffbf48e8e9b17cc1ea4f84cc508a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984970"
---
# <a name="update-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="1b100-103">更新 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="1b100-103">Update windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="1b100-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1b100-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b100-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1b100-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b100-106">更新[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1b100-106">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b100-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1b100-107">Prerequisites</span></span>
<span data-ttu-id="1b100-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b100-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b100-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b100-110">Permission type</span></span>|<span data-ttu-id="1b100-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1b100-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b100-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b100-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1b100-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b100-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1b100-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b100-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b100-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b100-115">Not supported.</span></span>|
|<span data-ttu-id="1b100-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b100-116">Application</span></span>|<span data-ttu-id="1b100-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b100-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b100-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b100-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1b100-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b100-119">Request headers</span></span>
|<span data-ttu-id="1b100-120">标头</span><span class="sxs-lookup"><span data-stu-id="1b100-120">Header</span></span>|<span data-ttu-id="1b100-121">值</span><span class="sxs-lookup"><span data-stu-id="1b100-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b100-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b100-122">Authorization</span></span>|<span data-ttu-id="1b100-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1b100-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b100-124">接受</span><span class="sxs-lookup"><span data-stu-id="1b100-124">Accept</span></span>|<span data-ttu-id="1b100-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1b100-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b100-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1b100-126">Request body</span></span>
<span data-ttu-id="1b100-127">在请求正文中, 提供[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b100-127">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

<span data-ttu-id="1b100-128">下表显示创建[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1b100-128">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

|<span data-ttu-id="1b100-129">属性</span><span class="sxs-lookup"><span data-stu-id="1b100-129">Property</span></span>|<span data-ttu-id="1b100-130">类型</span><span class="sxs-lookup"><span data-stu-id="1b100-130">Type</span></span>|<span data-ttu-id="1b100-131">说明</span><span class="sxs-lookup"><span data-stu-id="1b100-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b100-132">id</span><span class="sxs-lookup"><span data-stu-id="1b100-132">id</span></span>|<span data-ttu-id="1b100-133">String</span><span class="sxs-lookup"><span data-stu-id="1b100-133">String</span></span>|<span data-ttu-id="1b100-134">分配的键。</span><span class="sxs-lookup"><span data-stu-id="1b100-134">The key of the assignment.</span></span>|
|<span data-ttu-id="1b100-135">target</span><span class="sxs-lookup"><span data-stu-id="1b100-135">target</span></span>|[<span data-ttu-id="1b100-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1b100-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1b100-137">Windows Autopilot 部署配置文件的分配目标。</span><span class="sxs-lookup"><span data-stu-id="1b100-137">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="1b100-138">响应</span><span class="sxs-lookup"><span data-stu-id="1b100-138">Response</span></span>
<span data-ttu-id="1b100-139">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1b100-139">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b100-140">示例</span><span class="sxs-lookup"><span data-stu-id="1b100-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b100-141">请求</span><span class="sxs-lookup"><span data-stu-id="1b100-141">Request</span></span>
<span data-ttu-id="1b100-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1b100-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1b100-143">响应</span><span class="sxs-lookup"><span data-stu-id="1b100-143">Response</span></span>
<span data-ttu-id="1b100-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1b100-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





