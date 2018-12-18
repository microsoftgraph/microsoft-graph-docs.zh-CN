---
title: 删除 activeDirectoryWindowsAutopilotDeploymentProfile
description: 删除 activeDirectoryWindowsAutopilotDeploymentProfile。
author: tfitzmac
ms.openlocfilehash: 0ae86497a437b2064994d82a8e0c04e54ec3d245
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338855"
---
# <a name="delete-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="29f66-103">删除 activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="29f66-103">Delete activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="29f66-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="29f66-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29f66-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="29f66-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29f66-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="29f66-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29f66-107">删除[activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="29f66-107">Deletes a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="29f66-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="29f66-108">Prerequisites</span></span>
<span data-ttu-id="29f66-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="29f66-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29f66-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="29f66-111">Permission type</span></span>|<span data-ttu-id="29f66-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="29f66-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29f66-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29f66-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29f66-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29f66-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="29f66-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29f66-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29f66-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="29f66-116">Not supported.</span></span>|
|<span data-ttu-id="29f66-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="29f66-117">Application</span></span>|<span data-ttu-id="29f66-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="29f66-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29f66-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29f66-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
DELETE /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
DELETE /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="29f66-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="29f66-120">Request headers</span></span>
|<span data-ttu-id="29f66-121">标头</span><span class="sxs-lookup"><span data-stu-id="29f66-121">Header</span></span>|<span data-ttu-id="29f66-122">值</span><span class="sxs-lookup"><span data-stu-id="29f66-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29f66-123">授权</span><span class="sxs-lookup"><span data-stu-id="29f66-123">Authorization</span></span>|<span data-ttu-id="29f66-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="29f66-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29f66-125">Accept</span><span class="sxs-lookup"><span data-stu-id="29f66-125">Accept</span></span>|<span data-ttu-id="29f66-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29f66-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29f66-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="29f66-127">Request body</span></span>
<span data-ttu-id="29f66-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="29f66-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29f66-129">响应</span><span class="sxs-lookup"><span data-stu-id="29f66-129">Response</span></span>
<span data-ttu-id="29f66-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="29f66-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="29f66-131">示例</span><span class="sxs-lookup"><span data-stu-id="29f66-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="29f66-132">请求</span><span class="sxs-lookup"><span data-stu-id="29f66-132">Request</span></span>
<span data-ttu-id="29f66-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="29f66-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="29f66-134">响应</span><span class="sxs-lookup"><span data-stu-id="29f66-134">Response</span></span>
<span data-ttu-id="29f66-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="29f66-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





