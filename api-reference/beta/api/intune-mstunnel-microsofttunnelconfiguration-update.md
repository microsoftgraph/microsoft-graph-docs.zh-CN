---
title: 更新 microsoftTunnelConfiguration
description: 更新 microsoftTunnelConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9dd8018fb274dc9221eaa85a80f9cd2f15abcf90
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301528"
---
# <a name="update-microsofttunnelconfiguration"></a><span data-ttu-id="f03db-103">更新 microsoftTunnelConfiguration</span><span class="sxs-lookup"><span data-stu-id="f03db-103">Update microsoftTunnelConfiguration</span></span>

<span data-ttu-id="f03db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f03db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f03db-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f03db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f03db-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f03db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f03db-107">更新 [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f03db-107">Update the properties of a [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f03db-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f03db-108">Prerequisites</span></span>
<span data-ttu-id="f03db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f03db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f03db-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f03db-111">Permission type</span></span>|<span data-ttu-id="f03db-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f03db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f03db-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f03db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f03db-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f03db-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f03db-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f03db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f03db-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f03db-116">Not supported.</span></span>|
|<span data-ttu-id="f03db-117">Application</span><span class="sxs-lookup"><span data-stu-id="f03db-117">Application</span></span>|<span data-ttu-id="f03db-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f03db-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f03db-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f03db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/microsoftTunnelConfigurations/{microsoftTunnelConfigurationId}
PATCH /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="f03db-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f03db-120">Request headers</span></span>
|<span data-ttu-id="f03db-121">标头</span><span class="sxs-lookup"><span data-stu-id="f03db-121">Header</span></span>|<span data-ttu-id="f03db-122">值</span><span class="sxs-lookup"><span data-stu-id="f03db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f03db-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f03db-123">Authorization</span></span>|<span data-ttu-id="f03db-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f03db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f03db-125">接受</span><span class="sxs-lookup"><span data-stu-id="f03db-125">Accept</span></span>|<span data-ttu-id="f03db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f03db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f03db-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f03db-127">Request body</span></span>
<span data-ttu-id="f03db-128">在请求正文中，提供 [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f03db-128">In the request body, supply a JSON representation for the [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) object.</span></span>

<span data-ttu-id="f03db-129">下表显示创建 [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f03db-129">The following table shows the properties that are required when you create the [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md).</span></span>

|<span data-ttu-id="f03db-130">属性</span><span class="sxs-lookup"><span data-stu-id="f03db-130">Property</span></span>|<span data-ttu-id="f03db-131">类型</span><span class="sxs-lookup"><span data-stu-id="f03db-131">Type</span></span>|<span data-ttu-id="f03db-132">说明</span><span class="sxs-lookup"><span data-stu-id="f03db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f03db-133">id</span><span class="sxs-lookup"><span data-stu-id="f03db-133">id</span></span>|<span data-ttu-id="f03db-134">字符串</span><span class="sxs-lookup"><span data-stu-id="f03db-134">String</span></span>|<span data-ttu-id="f03db-135">MicrosoftTunnelConfiguration 的 Id</span><span class="sxs-lookup"><span data-stu-id="f03db-135">The MicrosoftTunnelConfiguration's Id</span></span>|
|<span data-ttu-id="f03db-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f03db-136">displayName</span></span>|<span data-ttu-id="f03db-137">字符串</span><span class="sxs-lookup"><span data-stu-id="f03db-137">String</span></span>|<span data-ttu-id="f03db-138">MicrosoftTunnelConfiguration 的显示名称</span><span class="sxs-lookup"><span data-stu-id="f03db-138">The MicrosoftTunnelConfiguration's display name</span></span>|
|<span data-ttu-id="f03db-139">description</span><span class="sxs-lookup"><span data-stu-id="f03db-139">description</span></span>|<span data-ttu-id="f03db-140">字符串</span><span class="sxs-lookup"><span data-stu-id="f03db-140">String</span></span>|<span data-ttu-id="f03db-141">MicrosoftTunnelConfiguration 的说明</span><span class="sxs-lookup"><span data-stu-id="f03db-141">The MicrosoftTunnelConfiguration's description</span></span>|
|<span data-ttu-id="f03db-142">network</span><span class="sxs-lookup"><span data-stu-id="f03db-142">network</span></span>|<span data-ttu-id="f03db-143">字符串</span><span class="sxs-lookup"><span data-stu-id="f03db-143">String</span></span>|<span data-ttu-id="f03db-144">将用于为客户端分配虚拟地址的子网</span><span class="sxs-lookup"><span data-stu-id="f03db-144">The subnet that will be used to allocate virtual address for the clients</span></span>|
|<span data-ttu-id="f03db-145">dnsServers</span><span class="sxs-lookup"><span data-stu-id="f03db-145">dnsServers</span></span>|<span data-ttu-id="f03db-146">String 集合</span><span class="sxs-lookup"><span data-stu-id="f03db-146">String collection</span></span>|<span data-ttu-id="f03db-147">客户端将使用的 DNS 服务器</span><span class="sxs-lookup"><span data-stu-id="f03db-147">The DNS servers that will be used by the clients</span></span>|
|<span data-ttu-id="f03db-148">defaultDomainSuffix</span><span class="sxs-lookup"><span data-stu-id="f03db-148">defaultDomainSuffix</span></span>|<span data-ttu-id="f03db-149">字符串</span><span class="sxs-lookup"><span data-stu-id="f03db-149">String</span></span>|<span data-ttu-id="f03db-150">客户端将使用的默认域附录</span><span class="sxs-lookup"><span data-stu-id="f03db-150">The Default Domain appendix that will be used by the clients</span></span>|
|<span data-ttu-id="f03db-151">routesInclude</span><span class="sxs-lookup"><span data-stu-id="f03db-151">routesInclude</span></span>|<span data-ttu-id="f03db-152">String 集合</span><span class="sxs-lookup"><span data-stu-id="f03db-152">String collection</span></span>|<span data-ttu-id="f03db-153">将由服务器路由的将</span><span class="sxs-lookup"><span data-stu-id="f03db-153">The routs that will be routed by the server</span></span>|
|<span data-ttu-id="f03db-154">routesExclude</span><span class="sxs-lookup"><span data-stu-id="f03db-154">routesExclude</span></span>|<span data-ttu-id="f03db-155">String 集合</span><span class="sxs-lookup"><span data-stu-id="f03db-155">String collection</span></span>|<span data-ttu-id="f03db-156">将不会由服务器路由的路由的子集</span><span class="sxs-lookup"><span data-stu-id="f03db-156">Subsets of the routes that will not be routed by the server</span></span>|
|<span data-ttu-id="f03db-157">splitDNS</span><span class="sxs-lookup"><span data-stu-id="f03db-157">splitDNS</span></span>|<span data-ttu-id="f03db-158">String 集合</span><span class="sxs-lookup"><span data-stu-id="f03db-158">String collection</span></span>|<span data-ttu-id="f03db-159">将使用所提供的 dns 服务器进行解析的域</span><span class="sxs-lookup"><span data-stu-id="f03db-159">The domains that will be resolved using the provided dns servers</span></span>|
|<span data-ttu-id="f03db-160">listenPort</span><span class="sxs-lookup"><span data-stu-id="f03db-160">listenPort</span></span>|<span data-ttu-id="f03db-161">Int32</span><span class="sxs-lookup"><span data-stu-id="f03db-161">Int32</span></span>|<span data-ttu-id="f03db-162">TCP 和 UPD 将在服务器上侦听的端口</span><span class="sxs-lookup"><span data-stu-id="f03db-162">The port that both TCP and UPD will listen over on the server</span></span>|
|<span data-ttu-id="f03db-163">advancedSettings</span><span class="sxs-lookup"><span data-stu-id="f03db-163">advancedSettings</span></span>|<span data-ttu-id="f03db-164">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f03db-164">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f03db-165">可能适用于服务器的其他设置</span><span class="sxs-lookup"><span data-stu-id="f03db-165">Additional settings that may be applied to the server</span></span>|
|<span data-ttu-id="f03db-166">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f03db-166">lastUpdateDateTime</span></span>|<span data-ttu-id="f03db-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f03db-167">DateTimeOffset</span></span>|<span data-ttu-id="f03db-168">上次更新 MicrosoftTunnelConfiguration 的时间</span><span class="sxs-lookup"><span data-stu-id="f03db-168">When the MicrosoftTunnelConfiguration was last updated</span></span>|
|<span data-ttu-id="f03db-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f03db-169">roleScopeTagIds</span></span>|<span data-ttu-id="f03db-170">String 集合</span><span class="sxs-lookup"><span data-stu-id="f03db-170">String collection</span></span>|<span data-ttu-id="f03db-171">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f03db-171">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="f03db-172">响应</span><span class="sxs-lookup"><span data-stu-id="f03db-172">Response</span></span>
<span data-ttu-id="f03db-173">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f03db-173">If successful, this method returns a `200 OK` response code and an updated [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f03db-174">示例</span><span class="sxs-lookup"><span data-stu-id="f03db-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="f03db-175">请求</span><span class="sxs-lookup"><span data-stu-id="f03db-175">Request</span></span>
<span data-ttu-id="f03db-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f03db-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelConfigurations/{microsoftTunnelConfigurationId}
Content-type: application/json
Content-length: 748

{
  "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "network": "Network value",
  "dnsServers": [
    "Dns Servers value"
  ],
  "defaultDomainSuffix": "Default Domain Suffix value",
  "routesInclude": [
    "Routes Include value"
  ],
  "routesExclude": [
    "Routes Exclude value"
  ],
  "splitDNS": [
    "Split DNS value"
  ],
  "listenPort": 10,
  "advancedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="f03db-177">响应</span><span class="sxs-lookup"><span data-stu-id="f03db-177">Response</span></span>
<span data-ttu-id="f03db-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f03db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 797

{
  "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
  "id": "b8bdb469-b469-b8bd-69b4-bdb869b4bdb8",
  "displayName": "Display Name value",
  "description": "Description value",
  "network": "Network value",
  "dnsServers": [
    "Dns Servers value"
  ],
  "defaultDomainSuffix": "Default Domain Suffix value",
  "routesInclude": [
    "Routes Include value"
  ],
  "routesExclude": [
    "Routes Exclude value"
  ],
  "splitDNS": [
    "Split DNS value"
  ],
  "listenPort": 10,
  "advancedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




