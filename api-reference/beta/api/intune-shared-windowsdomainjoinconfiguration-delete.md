---
title: 删除 windowsDomainJoinConfiguration
description: 删除 windowsDomainJoinConfiguration。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1d99fd2971efb3330d370af6cad99b8137f689ce
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866956"
---
# <a name="delete-windowsdomainjoinconfiguration"></a><span data-ttu-id="03b46-103">删除 windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="03b46-103">Delete windowsDomainJoinConfiguration</span></span>

<span data-ttu-id="03b46-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03b46-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03b46-105">**重要提示：** Microsoft Graph 中的 /beta 版本下的 API 可能会更改。</span><span class="sxs-lookup"><span data-stu-id="03b46-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="03b46-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="03b46-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03b46-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03b46-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03b46-108">删除 [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="03b46-108">Deletes a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="03b46-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="03b46-109">Prerequisites</span></span>
<span data-ttu-id="03b46-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03b46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03b46-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="03b46-112">Permission type</span></span>|<span data-ttu-id="03b46-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="03b46-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03b46-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03b46-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="03b46-115">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="03b46-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="03b46-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03b46-116">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="03b46-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03b46-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03b46-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="03b46-118">Not supported.</span></span>|
|<span data-ttu-id="03b46-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="03b46-119">Application</span></span>||
| <span data-ttu-id="03b46-120">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="03b46-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="03b46-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03b46-121">DeviceManagementConfiguration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03b46-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03b46-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="03b46-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="03b46-123">Request headers</span></span>
|<span data-ttu-id="03b46-124">标头</span><span class="sxs-lookup"><span data-stu-id="03b46-124">Header</span></span>|<span data-ttu-id="03b46-125">值</span><span class="sxs-lookup"><span data-stu-id="03b46-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03b46-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="03b46-126">Authorization</span></span>|<span data-ttu-id="03b46-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="03b46-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03b46-128">接受</span><span class="sxs-lookup"><span data-stu-id="03b46-128">Accept</span></span>|<span data-ttu-id="03b46-129">application/json</span><span class="sxs-lookup"><span data-stu-id="03b46-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03b46-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="03b46-130">Request body</span></span>
<span data-ttu-id="03b46-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="03b46-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03b46-132">响应</span><span class="sxs-lookup"><span data-stu-id="03b46-132">Response</span></span>
<span data-ttu-id="03b46-133">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="03b46-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="03b46-134">示例</span><span class="sxs-lookup"><span data-stu-id="03b46-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="03b46-135">请求</span><span class="sxs-lookup"><span data-stu-id="03b46-135">Request</span></span>
<span data-ttu-id="03b46-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03b46-136">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="03b46-137">响应</span><span class="sxs-lookup"><span data-stu-id="03b46-137">Response</span></span>
<span data-ttu-id="03b46-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="03b46-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```










