---
title: 删除 windowsWifiConfiguration
description: 删除 windowsWifiConfiguration。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2486c351c561fb69e878f310fc88df4b1a041328
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49300309"
---
# <a name="delete-windowswificonfiguration"></a><span data-ttu-id="7aa18-103">删除 windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="7aa18-103">Delete windowsWifiConfiguration</span></span>

<span data-ttu-id="7aa18-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7aa18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7aa18-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7aa18-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7aa18-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7aa18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7aa18-107">删除 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="7aa18-107">Deletes a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7aa18-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7aa18-108">Prerequisites</span></span>
<span data-ttu-id="7aa18-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7aa18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aa18-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7aa18-111">Permission type</span></span>|<span data-ttu-id="7aa18-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7aa18-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7aa18-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7aa18-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7aa18-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aa18-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7aa18-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7aa18-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7aa18-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7aa18-116">Not supported.</span></span>|
|<span data-ttu-id="7aa18-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7aa18-117">Application</span></span>|<span data-ttu-id="7aa18-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aa18-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7aa18-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7aa18-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7aa18-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7aa18-120">Request headers</span></span>
|<span data-ttu-id="7aa18-121">标头</span><span class="sxs-lookup"><span data-stu-id="7aa18-121">Header</span></span>|<span data-ttu-id="7aa18-122">值</span><span class="sxs-lookup"><span data-stu-id="7aa18-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7aa18-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7aa18-123">Authorization</span></span>|<span data-ttu-id="7aa18-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7aa18-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7aa18-125">接受</span><span class="sxs-lookup"><span data-stu-id="7aa18-125">Accept</span></span>|<span data-ttu-id="7aa18-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7aa18-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7aa18-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7aa18-127">Request body</span></span>
<span data-ttu-id="7aa18-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7aa18-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7aa18-129">响应</span><span class="sxs-lookup"><span data-stu-id="7aa18-129">Response</span></span>
<span data-ttu-id="7aa18-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7aa18-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7aa18-131">示例</span><span class="sxs-lookup"><span data-stu-id="7aa18-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7aa18-132">请求</span><span class="sxs-lookup"><span data-stu-id="7aa18-132">Request</span></span>
<span data-ttu-id="7aa18-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7aa18-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="7aa18-134">响应</span><span class="sxs-lookup"><span data-stu-id="7aa18-134">Response</span></span>
<span data-ttu-id="7aa18-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7aa18-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




