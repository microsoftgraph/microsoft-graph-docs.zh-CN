---
title: 删除 windowsDomainJoinConfiguration
description: 删除 windowsDomainJoinConfiguration。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 019c8e273c29321b54308c2e7a7fa65d6ccc9877
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702794"
---
# <a name="delete-windowsdomainjoinconfiguration"></a><span data-ttu-id="8f8ef-103">删除 windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="8f8ef-103">Delete windowsDomainJoinConfiguration</span></span>

<span data-ttu-id="8f8ef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f8ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f8ef-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8f8ef-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8f8ef-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8f8ef-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f8ef-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8f8ef-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f8ef-108">删除 [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="8f8ef-108">Deletes a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8f8ef-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="8f8ef-109">Prerequisites</span></span>
<span data-ttu-id="8f8ef-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f8ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f8ef-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f8ef-112">Permission type</span></span>|<span data-ttu-id="8f8ef-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8f8ef-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f8ef-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f8ef-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8f8ef-115">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="8f8ef-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8f8ef-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f8ef-116">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="8f8ef-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f8ef-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f8ef-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f8ef-118">Not supported.</span></span>|
|<span data-ttu-id="8f8ef-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f8ef-119">Application</span></span>||
| <span data-ttu-id="8f8ef-120">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="8f8ef-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8f8ef-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f8ef-121">DeviceManagementConfiguration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f8ef-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f8ef-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8f8ef-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f8ef-123">Request headers</span></span>
|<span data-ttu-id="8f8ef-124">标头</span><span class="sxs-lookup"><span data-stu-id="8f8ef-124">Header</span></span>|<span data-ttu-id="8f8ef-125">值</span><span class="sxs-lookup"><span data-stu-id="8f8ef-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f8ef-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f8ef-126">Authorization</span></span>|<span data-ttu-id="8f8ef-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8f8ef-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f8ef-128">接受</span><span class="sxs-lookup"><span data-stu-id="8f8ef-128">Accept</span></span>|<span data-ttu-id="8f8ef-129">application/json</span><span class="sxs-lookup"><span data-stu-id="8f8ef-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f8ef-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f8ef-130">Request body</span></span>
<span data-ttu-id="8f8ef-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8f8ef-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f8ef-132">响应</span><span class="sxs-lookup"><span data-stu-id="8f8ef-132">Response</span></span>
<span data-ttu-id="8f8ef-133">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8f8ef-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8f8ef-134">示例</span><span class="sxs-lookup"><span data-stu-id="8f8ef-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="8f8ef-135">请求</span><span class="sxs-lookup"><span data-stu-id="8f8ef-135">Request</span></span>
<span data-ttu-id="8f8ef-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8f8ef-136">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="8f8ef-137">响应</span><span class="sxs-lookup"><span data-stu-id="8f8ef-137">Response</span></span>
<span data-ttu-id="8f8ef-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8f8ef-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```











