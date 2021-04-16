---
title: 创建 microsoftTunnelServer
description: 创建新的 microsoftTunnelServer 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ea72ef3f00ab3076ffafe2e68ffc1e3bb1cbe31
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863196"
---
# <a name="create-microsofttunnelserver"></a><span data-ttu-id="51ba4-103">创建 microsoftTunnelServer</span><span class="sxs-lookup"><span data-stu-id="51ba4-103">Create microsoftTunnelServer</span></span>

<span data-ttu-id="51ba4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51ba4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51ba4-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="51ba4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51ba4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51ba4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51ba4-107">创建新的 [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="51ba4-107">Create a new [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51ba4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="51ba4-108">Prerequisites</span></span>
<span data-ttu-id="51ba4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="51ba4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51ba4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="51ba4-111">Permission type</span></span>|<span data-ttu-id="51ba4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="51ba4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51ba4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51ba4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51ba4-114">DeviceManagementConfiguration.ReadWrite.All、MicrosoftTunnelGateway.Read.All、MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51ba4-114">DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|
|<span data-ttu-id="51ba4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51ba4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51ba4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="51ba4-116">Not supported.</span></span>|
|<span data-ttu-id="51ba4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="51ba4-117">Application</span></span>|<span data-ttu-id="51ba4-118">MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51ba4-118">MicrosoftTunnelGateway.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51ba4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51ba4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers
```

## <a name="request-headers"></a><span data-ttu-id="51ba4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="51ba4-120">Request headers</span></span>
|<span data-ttu-id="51ba4-121">标头</span><span class="sxs-lookup"><span data-stu-id="51ba4-121">Header</span></span>|<span data-ttu-id="51ba4-122">值</span><span class="sxs-lookup"><span data-stu-id="51ba4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51ba4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="51ba4-123">Authorization</span></span>|<span data-ttu-id="51ba4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="51ba4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51ba4-125">接受</span><span class="sxs-lookup"><span data-stu-id="51ba4-125">Accept</span></span>|<span data-ttu-id="51ba4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51ba4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51ba4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="51ba4-127">Request body</span></span>
<span data-ttu-id="51ba4-128">在请求正文中，提供 microsoftTunnelServer 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51ba4-128">In the request body, supply a JSON representation for the microsoftTunnelServer object.</span></span>

<span data-ttu-id="51ba4-129">下表显示创建 microsoftTunnelServer 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="51ba4-129">The following table shows the properties that are required when you create the microsoftTunnelServer.</span></span>

|<span data-ttu-id="51ba4-130">属性</span><span class="sxs-lookup"><span data-stu-id="51ba4-130">Property</span></span>|<span data-ttu-id="51ba4-131">类型</span><span class="sxs-lookup"><span data-stu-id="51ba4-131">Type</span></span>|<span data-ttu-id="51ba4-132">说明</span><span class="sxs-lookup"><span data-stu-id="51ba4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51ba4-133">id</span><span class="sxs-lookup"><span data-stu-id="51ba4-133">id</span></span>|<span data-ttu-id="51ba4-134">String</span><span class="sxs-lookup"><span data-stu-id="51ba4-134">String</span></span>|<span data-ttu-id="51ba4-135">MicrosoftTunnelServer 的 ID</span><span class="sxs-lookup"><span data-stu-id="51ba4-135">The MicrosoftTunnelServer's Id</span></span>|
|<span data-ttu-id="51ba4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="51ba4-136">displayName</span></span>|<span data-ttu-id="51ba4-137">String</span><span class="sxs-lookup"><span data-stu-id="51ba4-137">String</span></span>|<span data-ttu-id="51ba4-138">MicrosoftTunnelServer 的显示名称</span><span class="sxs-lookup"><span data-stu-id="51ba4-138">The MicrosoftTunnelServer's display name</span></span>|
|<span data-ttu-id="51ba4-139">tunnelServerHealthStatus</span><span class="sxs-lookup"><span data-stu-id="51ba4-139">tunnelServerHealthStatus</span></span>|[<span data-ttu-id="51ba4-140">microsoftTunnelServerHealthStatus</span><span class="sxs-lookup"><span data-stu-id="51ba4-140">microsoftTunnelServerHealthStatus</span></span>](../resources/intune-mstunnel-microsofttunnelserverhealthstatus.md)|<span data-ttu-id="51ba4-141">MicrosoftTunnelServer 的运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="51ba4-141">The MicrosoftTunnelServer's health status.</span></span> <span data-ttu-id="51ba4-142">可取值为：`unknown`、`healthy`、`unhealthy`、`warning`、`offline`、`upgradeInProgress` 或 `upgradeFailed`。</span><span class="sxs-lookup"><span data-stu-id="51ba4-142">Possible values are: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.</span></span>|
|<span data-ttu-id="51ba4-143">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="51ba4-143">lastCheckinDateTime</span></span>|<span data-ttu-id="51ba4-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51ba4-144">DateTimeOffset</span></span>|<span data-ttu-id="51ba4-145">MicrosoftTunnelServer 上次签入时间</span><span class="sxs-lookup"><span data-stu-id="51ba4-145">When the MicrosoftTunnelServer last checked in</span></span>|



## <a name="response"></a><span data-ttu-id="51ba4-146">响应</span><span class="sxs-lookup"><span data-stu-id="51ba4-146">Response</span></span>
<span data-ttu-id="51ba4-147">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="51ba4-147">If successful, this method returns a `201 Created` response code and a [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51ba4-148">示例</span><span class="sxs-lookup"><span data-stu-id="51ba4-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="51ba4-149">请求</span><span class="sxs-lookup"><span data-stu-id="51ba4-149">Request</span></span>
<span data-ttu-id="51ba4-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="51ba4-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers
Content-type: application/json
Content-length: 208

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServer",
  "displayName": "Display Name value",
  "tunnelServerHealthStatus": "healthy",
  "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
}
```

### <a name="response"></a><span data-ttu-id="51ba4-151">响应</span><span class="sxs-lookup"><span data-stu-id="51ba4-151">Response</span></span>
<span data-ttu-id="51ba4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="51ba4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 257

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServer",
  "id": "b5cf0aee-0aee-b5cf-ee0a-cfb5ee0acfb5",
  "displayName": "Display Name value",
  "tunnelServerHealthStatus": "healthy",
  "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
}
```




