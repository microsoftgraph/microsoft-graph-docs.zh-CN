---
title: 更新 microsoftTunnelServer
description: 更新 microsoftTunnelServer 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a5094f510552b8b27329b475e048141ba1165954
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301520"
---
# <a name="update-microsofttunnelserver"></a><span data-ttu-id="5615b-103">更新 microsoftTunnelServer</span><span class="sxs-lookup"><span data-stu-id="5615b-103">Update microsoftTunnelServer</span></span>

<span data-ttu-id="5615b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5615b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5615b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5615b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5615b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5615b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5615b-107">更新 [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5615b-107">Update the properties of a [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5615b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5615b-108">Prerequisites</span></span>
<span data-ttu-id="5615b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5615b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5615b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5615b-111">Permission type</span></span>|<span data-ttu-id="5615b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5615b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5615b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5615b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5615b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5615b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5615b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5615b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5615b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5615b-116">Not supported.</span></span>|
|<span data-ttu-id="5615b-117">Application</span><span class="sxs-lookup"><span data-stu-id="5615b-117">Application</span></span>|<span data-ttu-id="5615b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5615b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5615b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5615b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers/{microsoftTunnelServerId}
```

## <a name="request-headers"></a><span data-ttu-id="5615b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5615b-120">Request headers</span></span>
|<span data-ttu-id="5615b-121">标头</span><span class="sxs-lookup"><span data-stu-id="5615b-121">Header</span></span>|<span data-ttu-id="5615b-122">值</span><span class="sxs-lookup"><span data-stu-id="5615b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5615b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5615b-123">Authorization</span></span>|<span data-ttu-id="5615b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5615b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5615b-125">接受</span><span class="sxs-lookup"><span data-stu-id="5615b-125">Accept</span></span>|<span data-ttu-id="5615b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5615b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5615b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5615b-127">Request body</span></span>
<span data-ttu-id="5615b-128">在请求正文中，提供 [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5615b-128">In the request body, supply a JSON representation for the [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) object.</span></span>

<span data-ttu-id="5615b-129">下表显示创建 [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5615b-129">The following table shows the properties that are required when you create the [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md).</span></span>

|<span data-ttu-id="5615b-130">属性</span><span class="sxs-lookup"><span data-stu-id="5615b-130">Property</span></span>|<span data-ttu-id="5615b-131">类型</span><span class="sxs-lookup"><span data-stu-id="5615b-131">Type</span></span>|<span data-ttu-id="5615b-132">说明</span><span class="sxs-lookup"><span data-stu-id="5615b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5615b-133">id</span><span class="sxs-lookup"><span data-stu-id="5615b-133">id</span></span>|<span data-ttu-id="5615b-134">字符串</span><span class="sxs-lookup"><span data-stu-id="5615b-134">String</span></span>|<span data-ttu-id="5615b-135">MicrosoftTunnelServer 的 Id</span><span class="sxs-lookup"><span data-stu-id="5615b-135">The MicrosoftTunnelServer's Id</span></span>|
|<span data-ttu-id="5615b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5615b-136">displayName</span></span>|<span data-ttu-id="5615b-137">字符串</span><span class="sxs-lookup"><span data-stu-id="5615b-137">String</span></span>|<span data-ttu-id="5615b-138">MicrosoftTunnelServer 的显示名称</span><span class="sxs-lookup"><span data-stu-id="5615b-138">The MicrosoftTunnelServer's display name</span></span>|
|<span data-ttu-id="5615b-139">tunnelServerHealthStatus</span><span class="sxs-lookup"><span data-stu-id="5615b-139">tunnelServerHealthStatus</span></span>|[<span data-ttu-id="5615b-140">microsoftTunnelServerHealthStatus</span><span class="sxs-lookup"><span data-stu-id="5615b-140">microsoftTunnelServerHealthStatus</span></span>](../resources/intune-mstunnel-microsofttunnelserverhealthstatus.md)|<span data-ttu-id="5615b-141">MicrosoftTunnelServer 的运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="5615b-141">The MicrosoftTunnelServer's health status.</span></span> <span data-ttu-id="5615b-142">可取值为：`unknown`、`healthy`、`unhealthy`、`warning`、`offline`、`upgradeInProgress` 或 `upgradeFailed`。</span><span class="sxs-lookup"><span data-stu-id="5615b-142">Possible values are: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.</span></span>|
|<span data-ttu-id="5615b-143">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="5615b-143">lastCheckinDateTime</span></span>|<span data-ttu-id="5615b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5615b-144">DateTimeOffset</span></span>|<span data-ttu-id="5615b-145">上次签入的 MicrosoftTunnelServer</span><span class="sxs-lookup"><span data-stu-id="5615b-145">When the MicrosoftTunnelServer last checked in</span></span>|



## <a name="response"></a><span data-ttu-id="5615b-146">响应</span><span class="sxs-lookup"><span data-stu-id="5615b-146">Response</span></span>
<span data-ttu-id="5615b-147">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5615b-147">If successful, this method returns a `200 OK` response code and an updated [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5615b-148">示例</span><span class="sxs-lookup"><span data-stu-id="5615b-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="5615b-149">请求</span><span class="sxs-lookup"><span data-stu-id="5615b-149">Request</span></span>
<span data-ttu-id="5615b-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5615b-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers/{microsoftTunnelServerId}
Content-type: application/json
Content-length: 208

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServer",
  "displayName": "Display Name value",
  "tunnelServerHealthStatus": "healthy",
  "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
}
```

### <a name="response"></a><span data-ttu-id="5615b-151">响应</span><span class="sxs-lookup"><span data-stu-id="5615b-151">Response</span></span>
<span data-ttu-id="5615b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5615b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




