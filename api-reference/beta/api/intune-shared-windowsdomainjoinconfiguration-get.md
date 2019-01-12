---
title: 获取 windowsDomainJoinConfiguration
description: 读取属性和 windowsDomainJoinConfiguration 对象的关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 64a295ae105a69865e304c45d08e339eadbf7936
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950240"
---
# <a name="get-windowsdomainjoinconfiguration"></a><span data-ttu-id="cb62b-103">获取 windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="cb62b-103">Get windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="cb62b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cb62b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb62b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cb62b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cb62b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cb62b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb62b-107">读取属性和[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="cb62b-107">Read properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb62b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cb62b-108">Prerequisites</span></span>

<span data-ttu-id="cb62b-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="cb62b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb62b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb62b-111">Permission type</span></span>|<span data-ttu-id="cb62b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cb62b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb62b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb62b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="cb62b-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="cb62b-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="cb62b-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb62b-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="cb62b-116">&nbsp; &nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="cb62b-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="cb62b-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb62b-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
|<span data-ttu-id="cb62b-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb62b-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb62b-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb62b-119">Not supported.</span></span>|
|<span data-ttu-id="cb62b-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb62b-120">Application</span></span>|<span data-ttu-id="cb62b-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb62b-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb62b-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb62b-122">HTTP Request</span></span>
<span data-ttu-id="cb62b-123">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="cb62b-123">**Device configuration**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="cb62b-124">**注册**</span><span class="sxs-lookup"><span data-stu-id="cb62b-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cb62b-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cb62b-125">Optional query parameters</span></span>

<span data-ttu-id="cb62b-126">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cb62b-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb62b-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb62b-127">Request headers</span></span>

|<span data-ttu-id="cb62b-128">标头</span><span class="sxs-lookup"><span data-stu-id="cb62b-128">Header</span></span>|<span data-ttu-id="cb62b-129">值</span><span class="sxs-lookup"><span data-stu-id="cb62b-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb62b-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb62b-130">Authorization</span></span>|<span data-ttu-id="cb62b-131">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cb62b-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb62b-132">Accept</span><span class="sxs-lookup"><span data-stu-id="cb62b-132">Accept</span></span>|<span data-ttu-id="cb62b-133">application/json</span><span class="sxs-lookup"><span data-stu-id="cb62b-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb62b-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb62b-134">Request body</span></span>

<span data-ttu-id="cb62b-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cb62b-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb62b-136">响应</span><span class="sxs-lookup"><span data-stu-id="cb62b-136">Response</span></span>

<span data-ttu-id="cb62b-137">如果成功，此方法返回`200 OK`响应正文中的响应代码和[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cb62b-137">If successful, this method returns a `200 OK` response code and [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb62b-138">示例</span><span class="sxs-lookup"><span data-stu-id="cb62b-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb62b-139">请求</span><span class="sxs-lookup"><span data-stu-id="cb62b-139">Request</span></span>

<span data-ttu-id="cb62b-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cb62b-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="cb62b-141">响应</span><span class="sxs-lookup"><span data-stu-id="cb62b-141">Response</span></span>

<span data-ttu-id="cb62b-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cb62b-142">Here is an example of the response.</span></span> <span data-ttu-id="cb62b-143">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cb62b-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cb62b-144">从实际的调用返回的属性取决于上下文。</span><span class="sxs-lookup"><span data-stu-id="cb62b-144">Properties returned from an actual call depend on the context.</span></span>

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



