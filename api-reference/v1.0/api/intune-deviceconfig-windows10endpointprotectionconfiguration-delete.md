---
title: 删除 windows10EndpointProtectionConfiguration
description: 删除 windows10EndpointProtectionConfiguration。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 11debd48b3749e6a4d5d0e46577cbbfea8e99682
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758286"
---
# <a name="delete-windows10endpointprotectionconfiguration"></a><span data-ttu-id="a6f4f-103">删除 windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="a6f4f-103">Delete windows10EndpointProtectionConfiguration</span></span>

<span data-ttu-id="a6f4f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6f4f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6f4f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6f4f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6f4f-106">删除 [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="a6f4f-106">Deletes a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6f4f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a6f4f-107">Prerequisites</span></span>
<span data-ttu-id="a6f4f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6f4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6f4f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6f4f-110">Permission type</span></span>|<span data-ttu-id="a6f4f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a6f4f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6f4f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6f4f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6f4f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6f4f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a6f4f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6f4f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6f4f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6f4f-115">Not supported.</span></span>|
|<span data-ttu-id="a6f4f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6f4f-116">Application</span></span>|<span data-ttu-id="a6f4f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6f4f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6f4f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6f4f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a6f4f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6f4f-119">Request headers</span></span>
|<span data-ttu-id="a6f4f-120">标头</span><span class="sxs-lookup"><span data-stu-id="a6f4f-120">Header</span></span>|<span data-ttu-id="a6f4f-121">值</span><span class="sxs-lookup"><span data-stu-id="a6f4f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6f4f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6f4f-122">Authorization</span></span>|<span data-ttu-id="a6f4f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a6f4f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6f4f-124">接受</span><span class="sxs-lookup"><span data-stu-id="a6f4f-124">Accept</span></span>|<span data-ttu-id="a6f4f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a6f4f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6f4f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6f4f-126">Request body</span></span>
<span data-ttu-id="a6f4f-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a6f4f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6f4f-128">响应</span><span class="sxs-lookup"><span data-stu-id="a6f4f-128">Response</span></span>
<span data-ttu-id="a6f4f-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a6f4f-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a6f4f-130">示例</span><span class="sxs-lookup"><span data-stu-id="a6f4f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6f4f-131">请求</span><span class="sxs-lookup"><span data-stu-id="a6f4f-131">Request</span></span>
<span data-ttu-id="a6f4f-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a6f4f-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="a6f4f-133">响应</span><span class="sxs-lookup"><span data-stu-id="a6f4f-133">Response</span></span>
<span data-ttu-id="a6f4f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a6f4f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




