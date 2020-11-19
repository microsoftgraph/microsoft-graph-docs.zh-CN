---
title: 删除 microsoftTunnelServer
description: 删除 microsoftTunnelServer。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: de4e61ce8868566b5a28f891e53adab1544c379b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301526"
---
# <a name="delete-microsofttunnelserver"></a><span data-ttu-id="1f124-103">删除 microsoftTunnelServer</span><span class="sxs-lookup"><span data-stu-id="1f124-103">Delete microsoftTunnelServer</span></span>

<span data-ttu-id="1f124-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f124-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f124-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1f124-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f124-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1f124-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f124-107">删除 [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)。</span><span class="sxs-lookup"><span data-stu-id="1f124-107">Deletes a [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f124-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1f124-108">Prerequisites</span></span>
<span data-ttu-id="1f124-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1f124-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f124-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f124-111">Permission type</span></span>|<span data-ttu-id="1f124-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1f124-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f124-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f124-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f124-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f124-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1f124-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f124-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f124-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f124-116">Not supported.</span></span>|
|<span data-ttu-id="1f124-117">Application</span><span class="sxs-lookup"><span data-stu-id="1f124-117">Application</span></span>|<span data-ttu-id="1f124-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f124-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f124-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f124-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers/{microsoftTunnelServerId}
```

## <a name="request-headers"></a><span data-ttu-id="1f124-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f124-120">Request headers</span></span>
|<span data-ttu-id="1f124-121">标头</span><span class="sxs-lookup"><span data-stu-id="1f124-121">Header</span></span>|<span data-ttu-id="1f124-122">值</span><span class="sxs-lookup"><span data-stu-id="1f124-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f124-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f124-123">Authorization</span></span>|<span data-ttu-id="1f124-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1f124-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f124-125">接受</span><span class="sxs-lookup"><span data-stu-id="1f124-125">Accept</span></span>|<span data-ttu-id="1f124-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1f124-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f124-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f124-127">Request body</span></span>
<span data-ttu-id="1f124-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1f124-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f124-129">响应</span><span class="sxs-lookup"><span data-stu-id="1f124-129">Response</span></span>
<span data-ttu-id="1f124-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1f124-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1f124-131">示例</span><span class="sxs-lookup"><span data-stu-id="1f124-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f124-132">请求</span><span class="sxs-lookup"><span data-stu-id="1f124-132">Request</span></span>
<span data-ttu-id="1f124-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1f124-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers/{microsoftTunnelServerId}
```

### <a name="response"></a><span data-ttu-id="1f124-134">响应</span><span class="sxs-lookup"><span data-stu-id="1f124-134">Response</span></span>
<span data-ttu-id="1f124-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1f124-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




