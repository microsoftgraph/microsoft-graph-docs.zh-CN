---
title: getOmaSettingPlainTextValue 函数
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7cd6e09c56d96c344ba8ba2fc4c29202dea63cd3
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868396"
---
# <a name="getomasettingplaintextvalue-function"></a><span data-ttu-id="703dd-103">getOmaSettingPlainTextValue 函数</span><span class="sxs-lookup"><span data-stu-id="703dd-103">getOmaSettingPlainTextValue function</span></span>

<span data-ttu-id="703dd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="703dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="703dd-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="703dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="703dd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="703dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="703dd-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="703dd-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="703dd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="703dd-108">Prerequisites</span></span>
<span data-ttu-id="703dd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="703dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="703dd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="703dd-111">Permission type</span></span>|<span data-ttu-id="703dd-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="703dd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="703dd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="703dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="703dd-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="703dd-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="703dd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="703dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="703dd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="703dd-116">Not supported.</span></span>|
|<span data-ttu-id="703dd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="703dd-117">Application</span></span>|<span data-ttu-id="703dd-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="703dd-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="703dd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="703dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/getOmaSettingPlainTextValue
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/getOmaSettingPlainTextValue
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/getOmaSettingPlainTextValue
```

## <a name="request-headers"></a><span data-ttu-id="703dd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="703dd-120">Request headers</span></span>
|<span data-ttu-id="703dd-121">标头</span><span class="sxs-lookup"><span data-stu-id="703dd-121">Header</span></span>|<span data-ttu-id="703dd-122">值</span><span class="sxs-lookup"><span data-stu-id="703dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="703dd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="703dd-123">Authorization</span></span>|<span data-ttu-id="703dd-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="703dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="703dd-125">接受</span><span class="sxs-lookup"><span data-stu-id="703dd-125">Accept</span></span>|<span data-ttu-id="703dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="703dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="703dd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="703dd-127">Request body</span></span>
<span data-ttu-id="703dd-128">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="703dd-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="703dd-129">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="703dd-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="703dd-130">属性</span><span class="sxs-lookup"><span data-stu-id="703dd-130">Property</span></span>|<span data-ttu-id="703dd-131">类型</span><span class="sxs-lookup"><span data-stu-id="703dd-131">Type</span></span>|<span data-ttu-id="703dd-132">说明</span><span class="sxs-lookup"><span data-stu-id="703dd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="703dd-133">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="703dd-133">secretReferenceValueId</span></span>|<span data-ttu-id="703dd-134">String</span><span class="sxs-lookup"><span data-stu-id="703dd-134">String</span></span>|<span data-ttu-id="703dd-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="703dd-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="703dd-136">响应</span><span class="sxs-lookup"><span data-stu-id="703dd-136">Response</span></span>
<span data-ttu-id="703dd-137">如果成功，此函数在响应 `200 OK` 正文中返回 响应代码和 String。</span><span class="sxs-lookup"><span data-stu-id="703dd-137">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="703dd-138">示例</span><span class="sxs-lookup"><span data-stu-id="703dd-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="703dd-139">请求</span><span class="sxs-lookup"><span data-stu-id="703dd-139">Request</span></span>
<span data-ttu-id="703dd-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="703dd-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/getOmaSettingPlainTextValue(secretReferenceValueId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="703dd-141">响应</span><span class="sxs-lookup"><span data-stu-id="703dd-141">Response</span></span>
<span data-ttu-id="703dd-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="703dd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 57

{
  "value": "Get Oma Setting Plain Text Value value"
}
```




