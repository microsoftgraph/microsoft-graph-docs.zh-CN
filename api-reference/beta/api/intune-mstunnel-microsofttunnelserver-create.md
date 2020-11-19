---
title: 创建 microsoftTunnelServer
description: 创建新的 microsoftTunnelServer 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 146de9c8b03d2934ad6507b5adf2aecc3d778d75
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301527"
---
# <a name="create-microsofttunnelserver"></a><span data-ttu-id="74240-103">创建 microsoftTunnelServer</span><span class="sxs-lookup"><span data-stu-id="74240-103">Create microsoftTunnelServer</span></span>

<span data-ttu-id="74240-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74240-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74240-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="74240-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74240-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="74240-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74240-107">创建新的 [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="74240-107">Create a new [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74240-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="74240-108">Prerequisites</span></span>
<span data-ttu-id="74240-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74240-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74240-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="74240-111">Permission type</span></span>|<span data-ttu-id="74240-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="74240-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74240-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74240-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74240-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74240-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="74240-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74240-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74240-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="74240-116">Not supported.</span></span>|
|<span data-ttu-id="74240-117">Application</span><span class="sxs-lookup"><span data-stu-id="74240-117">Application</span></span>|<span data-ttu-id="74240-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74240-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="74240-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74240-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers
```

## <a name="request-headers"></a><span data-ttu-id="74240-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="74240-120">Request headers</span></span>
|<span data-ttu-id="74240-121">标头</span><span class="sxs-lookup"><span data-stu-id="74240-121">Header</span></span>|<span data-ttu-id="74240-122">值</span><span class="sxs-lookup"><span data-stu-id="74240-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74240-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74240-123">Authorization</span></span>|<span data-ttu-id="74240-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="74240-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74240-125">接受</span><span class="sxs-lookup"><span data-stu-id="74240-125">Accept</span></span>|<span data-ttu-id="74240-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74240-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74240-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="74240-127">Request body</span></span>
<span data-ttu-id="74240-128">在请求正文中，提供 microsoftTunnelServer 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74240-128">In the request body, supply a JSON representation for the microsoftTunnelServer object.</span></span>

<span data-ttu-id="74240-129">下表显示创建 microsoftTunnelServer 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="74240-129">The following table shows the properties that are required when you create the microsoftTunnelServer.</span></span>

|<span data-ttu-id="74240-130">属性</span><span class="sxs-lookup"><span data-stu-id="74240-130">Property</span></span>|<span data-ttu-id="74240-131">类型</span><span class="sxs-lookup"><span data-stu-id="74240-131">Type</span></span>|<span data-ttu-id="74240-132">说明</span><span class="sxs-lookup"><span data-stu-id="74240-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74240-133">id</span><span class="sxs-lookup"><span data-stu-id="74240-133">id</span></span>|<span data-ttu-id="74240-134">字符串</span><span class="sxs-lookup"><span data-stu-id="74240-134">String</span></span>|<span data-ttu-id="74240-135">MicrosoftTunnelServer 的 Id</span><span class="sxs-lookup"><span data-stu-id="74240-135">The MicrosoftTunnelServer's Id</span></span>|
|<span data-ttu-id="74240-136">displayName</span><span class="sxs-lookup"><span data-stu-id="74240-136">displayName</span></span>|<span data-ttu-id="74240-137">字符串</span><span class="sxs-lookup"><span data-stu-id="74240-137">String</span></span>|<span data-ttu-id="74240-138">MicrosoftTunnelServer 的显示名称</span><span class="sxs-lookup"><span data-stu-id="74240-138">The MicrosoftTunnelServer's display name</span></span>|
|<span data-ttu-id="74240-139">tunnelServerHealthStatus</span><span class="sxs-lookup"><span data-stu-id="74240-139">tunnelServerHealthStatus</span></span>|[<span data-ttu-id="74240-140">microsoftTunnelServerHealthStatus</span><span class="sxs-lookup"><span data-stu-id="74240-140">microsoftTunnelServerHealthStatus</span></span>](../resources/intune-mstunnel-microsofttunnelserverhealthstatus.md)|<span data-ttu-id="74240-141">MicrosoftTunnelServer 的运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="74240-141">The MicrosoftTunnelServer's health status.</span></span> <span data-ttu-id="74240-142">可取值为：`unknown`、`healthy`、`unhealthy`、`warning`、`offline`、`upgradeInProgress` 或 `upgradeFailed`。</span><span class="sxs-lookup"><span data-stu-id="74240-142">Possible values are: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.</span></span>|
|<span data-ttu-id="74240-143">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="74240-143">lastCheckinDateTime</span></span>|<span data-ttu-id="74240-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74240-144">DateTimeOffset</span></span>|<span data-ttu-id="74240-145">上次签入的 MicrosoftTunnelServer</span><span class="sxs-lookup"><span data-stu-id="74240-145">When the MicrosoftTunnelServer last checked in</span></span>|



## <a name="response"></a><span data-ttu-id="74240-146">响应</span><span class="sxs-lookup"><span data-stu-id="74240-146">Response</span></span>
<span data-ttu-id="74240-147">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="74240-147">If successful, this method returns a `201 Created` response code and a [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74240-148">示例</span><span class="sxs-lookup"><span data-stu-id="74240-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="74240-149">请求</span><span class="sxs-lookup"><span data-stu-id="74240-149">Request</span></span>
<span data-ttu-id="74240-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="74240-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="74240-151">响应</span><span class="sxs-lookup"><span data-stu-id="74240-151">Response</span></span>
<span data-ttu-id="74240-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="74240-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




