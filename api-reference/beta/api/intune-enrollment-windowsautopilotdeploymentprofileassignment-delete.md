---
title: 删除 windowsAutopilotDeploymentProfileAssignment
description: 删除 windowsAutopilotDeploymentProfileAssignment。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9ad934b5692b5cc848eab7daed429e7cf6440c73
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419994"
---
# <a name="delete-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="e42b4-103">删除 windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="e42b4-103">Delete windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="e42b4-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e42b4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e42b4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e42b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e42b4-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e42b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e42b4-107">删除[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="e42b4-107">Deletes a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e42b4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e42b4-108">Prerequisites</span></span>
<span data-ttu-id="e42b4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e42b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e42b4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e42b4-111">Permission type</span></span>|<span data-ttu-id="e42b4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e42b4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e42b4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e42b4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e42b4-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e42b4-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e42b4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e42b4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e42b4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e42b4-116">Not supported.</span></span>|
|<span data-ttu-id="e42b4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e42b4-117">Application</span></span>|<span data-ttu-id="e42b4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e42b4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e42b4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e42b4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e42b4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e42b4-120">Request headers</span></span>
|<span data-ttu-id="e42b4-121">标头</span><span class="sxs-lookup"><span data-stu-id="e42b4-121">Header</span></span>|<span data-ttu-id="e42b4-122">值</span><span class="sxs-lookup"><span data-stu-id="e42b4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e42b4-123">授权</span><span class="sxs-lookup"><span data-stu-id="e42b4-123">Authorization</span></span>|<span data-ttu-id="e42b4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e42b4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e42b4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e42b4-125">Accept</span></span>|<span data-ttu-id="e42b4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e42b4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e42b4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e42b4-127">Request body</span></span>
<span data-ttu-id="e42b4-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e42b4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e42b4-129">响应</span><span class="sxs-lookup"><span data-stu-id="e42b4-129">Response</span></span>
<span data-ttu-id="e42b4-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e42b4-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e42b4-131">示例</span><span class="sxs-lookup"><span data-stu-id="e42b4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e42b4-132">请求</span><span class="sxs-lookup"><span data-stu-id="e42b4-132">Request</span></span>
<span data-ttu-id="e42b4-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e42b4-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

### <a name="response"></a><span data-ttu-id="e42b4-134">响应</span><span class="sxs-lookup"><span data-stu-id="e42b4-134">Response</span></span>
<span data-ttu-id="e42b4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e42b4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




