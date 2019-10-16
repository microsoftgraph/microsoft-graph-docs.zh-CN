---
title: 删除 windowsDomainJoinConfiguration
description: 删除 windowsDomainJoinConfiguration。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e5cb9759f0a60a371695b4f077e5220d248b1b5b
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536838"
---
# <a name="delete-windowsdomainjoinconfiguration"></a><span data-ttu-id="4016b-103">删除 windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="4016b-103">Delete windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="4016b-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4016b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4016b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4016b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4016b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4016b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4016b-107">删除[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="4016b-107">Deletes a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4016b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4016b-108">Prerequisites</span></span>
<span data-ttu-id="4016b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4016b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4016b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4016b-111">Permission type</span></span>|<span data-ttu-id="4016b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4016b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4016b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4016b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4016b-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="4016b-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4016b-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4016b-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="4016b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4016b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4016b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4016b-117">Not supported.</span></span>|
|<span data-ttu-id="4016b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="4016b-118">Application</span></span>||
| <span data-ttu-id="4016b-119">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="4016b-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4016b-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4016b-120">DeviceManagementConfiguration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4016b-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4016b-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4016b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="4016b-122">Request headers</span></span>
|<span data-ttu-id="4016b-123">标头</span><span class="sxs-lookup"><span data-stu-id="4016b-123">Header</span></span>|<span data-ttu-id="4016b-124">值</span><span class="sxs-lookup"><span data-stu-id="4016b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4016b-125">授权</span><span class="sxs-lookup"><span data-stu-id="4016b-125">Authorization</span></span>|<span data-ttu-id="4016b-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4016b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4016b-127">接受</span><span class="sxs-lookup"><span data-stu-id="4016b-127">Accept</span></span>|<span data-ttu-id="4016b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4016b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4016b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4016b-129">Request body</span></span>
<span data-ttu-id="4016b-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4016b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4016b-131">响应</span><span class="sxs-lookup"><span data-stu-id="4016b-131">Response</span></span>
<span data-ttu-id="4016b-132">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4016b-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4016b-133">示例</span><span class="sxs-lookup"><span data-stu-id="4016b-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="4016b-134">请求</span><span class="sxs-lookup"><span data-stu-id="4016b-134">Request</span></span>
<span data-ttu-id="4016b-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4016b-135">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="4016b-136">响应</span><span class="sxs-lookup"><span data-stu-id="4016b-136">Response</span></span>
<span data-ttu-id="4016b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4016b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









