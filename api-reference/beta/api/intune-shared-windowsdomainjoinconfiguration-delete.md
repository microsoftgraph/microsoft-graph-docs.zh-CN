---
title: 删除 windowsDomainJoinConfiguration
description: 删除 windowsDomainJoinConfiguration。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3ce3ad8721e9ce1474af49ca412c8dc3ce71037f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347365"
---
# <a name="delete-windowsdomainjoinconfiguration"></a><span data-ttu-id="f4a5a-103">删除 windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="f4a5a-103">Delete windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="f4a5a-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f4a5a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f4a5a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f4a5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4a5a-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4a5a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4a5a-107">删除[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="f4a5a-107">Deletes a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f4a5a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f4a5a-108">Prerequisites</span></span>
<span data-ttu-id="f4a5a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4a5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4a5a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4a5a-111">Permission type</span></span>|<span data-ttu-id="f4a5a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f4a5a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4a5a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4a5a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f4a5a-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="f4a5a-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="f4a5a-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4a5a-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="f4a5a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4a5a-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4a5a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4a5a-117">Not supported.</span></span>|
|<span data-ttu-id="f4a5a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4a5a-118">Application</span></span>|<span data-ttu-id="f4a5a-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4a5a-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4a5a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4a5a-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f4a5a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4a5a-121">Request headers</span></span>
|<span data-ttu-id="f4a5a-122">标头</span><span class="sxs-lookup"><span data-stu-id="f4a5a-122">Header</span></span>|<span data-ttu-id="f4a5a-123">值</span><span class="sxs-lookup"><span data-stu-id="f4a5a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4a5a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4a5a-124">Authorization</span></span>|<span data-ttu-id="f4a5a-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f4a5a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4a5a-126">接受</span><span class="sxs-lookup"><span data-stu-id="f4a5a-126">Accept</span></span>|<span data-ttu-id="f4a5a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f4a5a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4a5a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4a5a-128">Request body</span></span>
<span data-ttu-id="f4a5a-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f4a5a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4a5a-130">响应</span><span class="sxs-lookup"><span data-stu-id="f4a5a-130">Response</span></span>
<span data-ttu-id="f4a5a-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f4a5a-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f4a5a-132">示例</span><span class="sxs-lookup"><span data-stu-id="f4a5a-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="f4a5a-133">请求</span><span class="sxs-lookup"><span data-stu-id="f4a5a-133">Request</span></span>
<span data-ttu-id="f4a5a-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4a5a-134">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f4a5a-135">响应</span><span class="sxs-lookup"><span data-stu-id="f4a5a-135">Response</span></span>
<span data-ttu-id="f4a5a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4a5a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






