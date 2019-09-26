---
title: 删除 activeDirectoryWindowsAutopilotDeploymentProfile
description: 删除 activeDirectoryWindowsAutopilotDeploymentProfile。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a2e08a9ba7e91fc26bd7013420500d8772e88f2e
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37187982"
---
# <a name="delete-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="d25bb-103">删除 activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="d25bb-103">Delete activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="d25bb-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d25bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d25bb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d25bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d25bb-106">删除[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="d25bb-106">Deletes a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d25bb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d25bb-107">Prerequisites</span></span>
<span data-ttu-id="d25bb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d25bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d25bb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d25bb-110">Permission type</span></span>|<span data-ttu-id="d25bb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d25bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d25bb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d25bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d25bb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d25bb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d25bb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d25bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d25bb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d25bb-115">Not supported.</span></span>|
|<span data-ttu-id="d25bb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d25bb-116">Application</span></span>|<span data-ttu-id="d25bb-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d25bb-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d25bb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d25bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
DELETE /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
DELETE /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="d25bb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d25bb-119">Request headers</span></span>
|<span data-ttu-id="d25bb-120">标头</span><span class="sxs-lookup"><span data-stu-id="d25bb-120">Header</span></span>|<span data-ttu-id="d25bb-121">值</span><span class="sxs-lookup"><span data-stu-id="d25bb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d25bb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d25bb-122">Authorization</span></span>|<span data-ttu-id="d25bb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d25bb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d25bb-124">接受</span><span class="sxs-lookup"><span data-stu-id="d25bb-124">Accept</span></span>|<span data-ttu-id="d25bb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d25bb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d25bb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d25bb-126">Request body</span></span>
<span data-ttu-id="d25bb-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d25bb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d25bb-128">响应</span><span class="sxs-lookup"><span data-stu-id="d25bb-128">Response</span></span>
<span data-ttu-id="d25bb-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d25bb-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d25bb-130">示例</span><span class="sxs-lookup"><span data-stu-id="d25bb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d25bb-131">请求</span><span class="sxs-lookup"><span data-stu-id="d25bb-131">Request</span></span>
<span data-ttu-id="d25bb-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d25bb-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="d25bb-133">响应</span><span class="sxs-lookup"><span data-stu-id="d25bb-133">Response</span></span>
<span data-ttu-id="d25bb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d25bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




