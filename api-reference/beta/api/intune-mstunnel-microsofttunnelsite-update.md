---
title: 更新 microsoftTunnelSite
description: 更新 microsoftTunnelSite 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 74a0396c4627a8c7f4e496df78964de0ff2965cd
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863827"
---
# <a name="update-microsofttunnelsite"></a><span data-ttu-id="211a8-103">更新 microsoftTunnelSite</span><span class="sxs-lookup"><span data-stu-id="211a8-103">Update microsoftTunnelSite</span></span>

<span data-ttu-id="211a8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="211a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="211a8-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="211a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="211a8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="211a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="211a8-107">更新 [microsoftTunnelSite 对象](../resources/intune-mstunnel-microsofttunnelsite.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="211a8-107">Update the properties of a [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="211a8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="211a8-108">Prerequisites</span></span>
<span data-ttu-id="211a8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="211a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="211a8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="211a8-111">Permission type</span></span>|<span data-ttu-id="211a8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="211a8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="211a8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="211a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="211a8-114">DeviceManagementConfiguration.ReadWrite.All、MicrosoftTunnelGateway.Read.All、MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="211a8-114">DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|
|<span data-ttu-id="211a8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="211a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="211a8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="211a8-116">Not supported.</span></span>|
|<span data-ttu-id="211a8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="211a8-117">Application</span></span>|<span data-ttu-id="211a8-118">MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="211a8-118">MicrosoftTunnelGateway.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="211a8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="211a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}
```

## <a name="request-headers"></a><span data-ttu-id="211a8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="211a8-120">Request headers</span></span>
|<span data-ttu-id="211a8-121">标头</span><span class="sxs-lookup"><span data-stu-id="211a8-121">Header</span></span>|<span data-ttu-id="211a8-122">值</span><span class="sxs-lookup"><span data-stu-id="211a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="211a8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="211a8-123">Authorization</span></span>|<span data-ttu-id="211a8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="211a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="211a8-125">接受</span><span class="sxs-lookup"><span data-stu-id="211a8-125">Accept</span></span>|<span data-ttu-id="211a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="211a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="211a8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="211a8-127">Request body</span></span>
<span data-ttu-id="211a8-128">在请求正文中，提供 [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="211a8-128">In the request body, supply a JSON representation for the [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) object.</span></span>

<span data-ttu-id="211a8-129">下表显示创建 [microsoftTunnelSite 时所需的属性](../resources/intune-mstunnel-microsofttunnelsite.md)。</span><span class="sxs-lookup"><span data-stu-id="211a8-129">The following table shows the properties that are required when you create the [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md).</span></span>

|<span data-ttu-id="211a8-130">属性</span><span class="sxs-lookup"><span data-stu-id="211a8-130">Property</span></span>|<span data-ttu-id="211a8-131">类型</span><span class="sxs-lookup"><span data-stu-id="211a8-131">Type</span></span>|<span data-ttu-id="211a8-132">说明</span><span class="sxs-lookup"><span data-stu-id="211a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="211a8-133">id</span><span class="sxs-lookup"><span data-stu-id="211a8-133">id</span></span>|<span data-ttu-id="211a8-134">String</span><span class="sxs-lookup"><span data-stu-id="211a8-134">String</span></span>|<span data-ttu-id="211a8-135">MicrosoftTunnelSite 的 ID</span><span class="sxs-lookup"><span data-stu-id="211a8-135">The MicrosoftTunnelSite's Id</span></span>|
|<span data-ttu-id="211a8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="211a8-136">displayName</span></span>|<span data-ttu-id="211a8-137">String</span><span class="sxs-lookup"><span data-stu-id="211a8-137">String</span></span>|<span data-ttu-id="211a8-138">MicrosoftTunnelSite 的显示名称</span><span class="sxs-lookup"><span data-stu-id="211a8-138">The MicrosoftTunnelSite's display name</span></span>|
|<span data-ttu-id="211a8-139">说明</span><span class="sxs-lookup"><span data-stu-id="211a8-139">description</span></span>|<span data-ttu-id="211a8-140">String</span><span class="sxs-lookup"><span data-stu-id="211a8-140">String</span></span>|<span data-ttu-id="211a8-141">MicrosoftTunnelSite 的说明</span><span class="sxs-lookup"><span data-stu-id="211a8-141">The MicrosoftTunnelSite's description</span></span>|
|<span data-ttu-id="211a8-142">publicAddress</span><span class="sxs-lookup"><span data-stu-id="211a8-142">publicAddress</span></span>|<span data-ttu-id="211a8-143">String</span><span class="sxs-lookup"><span data-stu-id="211a8-143">String</span></span>|<span data-ttu-id="211a8-144">MicrosoftTunnelSite 的公共域名或 IP 地址</span><span class="sxs-lookup"><span data-stu-id="211a8-144">The MicrosoftTunnelSite's public domain name or IP address</span></span>|
|<span data-ttu-id="211a8-145">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="211a8-145">roleScopeTagIds</span></span>|<span data-ttu-id="211a8-146">String 集合</span><span class="sxs-lookup"><span data-stu-id="211a8-146">String collection</span></span>|<span data-ttu-id="211a8-147">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="211a8-147">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="211a8-148">响应</span><span class="sxs-lookup"><span data-stu-id="211a8-148">Response</span></span>
<span data-ttu-id="211a8-149">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="211a8-149">If successful, this method returns a `200 OK` response code and an updated [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="211a8-150">示例</span><span class="sxs-lookup"><span data-stu-id="211a8-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="211a8-151">请求</span><span class="sxs-lookup"><span data-stu-id="211a8-151">Request</span></span>
<span data-ttu-id="211a8-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="211a8-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}
Content-type: application/json
Content-length: 246

{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "displayName": "Display Name value",
  "description": "Description value",
  "publicAddress": "Public Address value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="211a8-153">响应</span><span class="sxs-lookup"><span data-stu-id="211a8-153">Response</span></span>
<span data-ttu-id="211a8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="211a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "id": "b2f7dc3e-dc3e-b2f7-3edc-f7b23edcf7b2",
  "displayName": "Display Name value",
  "description": "Description value",
  "publicAddress": "Public Address value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




