---
title: 获取 windowsDomainJoinConfiguration
description: 读取 windowsDomainJoinConfiguration 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 717800ee8399b83ec8d9c38fd7fade2a3ba6a924
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194325"
---
# <a name="get-windowsdomainjoinconfiguration"></a><span data-ttu-id="5e301-103">获取 windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="5e301-103">Get windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="5e301-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5e301-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5e301-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5e301-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e301-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e301-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e301-107">读取[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5e301-107">Read properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e301-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5e301-108">Prerequisites</span></span>

<span data-ttu-id="5e301-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e301-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e301-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e301-111">Permission type</span></span>|<span data-ttu-id="5e301-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5e301-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e301-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e301-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5e301-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="5e301-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5e301-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e301-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="5e301-116">&nbsp;&nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="5e301-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="5e301-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e301-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
|<span data-ttu-id="5e301-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e301-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e301-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e301-119">Not supported.</span></span>|
|<span data-ttu-id="5e301-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e301-120">Application</span></span>||
| <span data-ttu-id="5e301-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="5e301-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5e301-122">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e301-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="5e301-123">&nbsp;&nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="5e301-123">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="5e301-124">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e301-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e301-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e301-125">HTTP Request</span></span>
<span data-ttu-id="5e301-126">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="5e301-126">**Device configuration**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="5e301-127">**开户**</span><span class="sxs-lookup"><span data-stu-id="5e301-127">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5e301-128">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5e301-128">Optional query parameters</span></span>

<span data-ttu-id="5e301-129">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5e301-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5e301-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e301-130">Request headers</span></span>

|<span data-ttu-id="5e301-131">标头</span><span class="sxs-lookup"><span data-stu-id="5e301-131">Header</span></span>|<span data-ttu-id="5e301-132">值</span><span class="sxs-lookup"><span data-stu-id="5e301-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e301-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e301-133">Authorization</span></span>|<span data-ttu-id="5e301-134">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5e301-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e301-135">接受</span><span class="sxs-lookup"><span data-stu-id="5e301-135">Accept</span></span>|<span data-ttu-id="5e301-136">application/json</span><span class="sxs-lookup"><span data-stu-id="5e301-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e301-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e301-137">Request body</span></span>

<span data-ttu-id="5e301-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5e301-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e301-139">响应</span><span class="sxs-lookup"><span data-stu-id="5e301-139">Response</span></span>

<span data-ttu-id="5e301-140">如果成功，此方法在响应`200 OK`正文中返回响应代码和[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5e301-140">If successful, this method returns a `200 OK` response code and [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e301-141">示例</span><span class="sxs-lookup"><span data-stu-id="5e301-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e301-142">请求</span><span class="sxs-lookup"><span data-stu-id="5e301-142">Request</span></span>

<span data-ttu-id="5e301-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5e301-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="5e301-144">响应</span><span class="sxs-lookup"><span data-stu-id="5e301-144">Response</span></span>

<span data-ttu-id="5e301-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5e301-145">Here is an example of the response.</span></span> <span data-ttu-id="5e301-146">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5e301-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5e301-147">从实际调用返回的属性取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="5e301-147">Properties returned from an actual call depend on the context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 560

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
    "id": "40118d08-8d08-4011-088d-1140088d1140",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "computerNameStaticPrefix": "Computer Name Static Prefix value",
    "computerNameSuffixRandomCharCount": 1,
    "activeDirectoryDomainName": "Active Directory Domain Name value"
  }
}
```







