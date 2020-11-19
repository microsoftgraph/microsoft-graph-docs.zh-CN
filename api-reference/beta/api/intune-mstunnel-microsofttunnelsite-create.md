---
title: 创建 microsoftTunnelSite
description: 创建新的 microsoftTunnelSite 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2f1604133399aeb9f7a5787b195a3680f398c04c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301518"
---
# <a name="create-microsofttunnelsite"></a><span data-ttu-id="df7a4-103">创建 microsoftTunnelSite</span><span class="sxs-lookup"><span data-stu-id="df7a4-103">Create microsoftTunnelSite</span></span>

<span data-ttu-id="df7a4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df7a4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df7a4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="df7a4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df7a4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df7a4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df7a4-107">创建新的 [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df7a4-107">Create a new [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df7a4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="df7a4-108">Prerequisites</span></span>
<span data-ttu-id="df7a4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df7a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df7a4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="df7a4-111">Permission type</span></span>|<span data-ttu-id="df7a4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="df7a4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df7a4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df7a4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df7a4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df7a4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="df7a4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df7a4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df7a4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="df7a4-116">Not supported.</span></span>|
|<span data-ttu-id="df7a4-117">Application</span><span class="sxs-lookup"><span data-stu-id="df7a4-117">Application</span></span>|<span data-ttu-id="df7a4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df7a4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df7a4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df7a4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/microsoftTunnelSites
```

## <a name="request-headers"></a><span data-ttu-id="df7a4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="df7a4-120">Request headers</span></span>
|<span data-ttu-id="df7a4-121">标头</span><span class="sxs-lookup"><span data-stu-id="df7a4-121">Header</span></span>|<span data-ttu-id="df7a4-122">值</span><span class="sxs-lookup"><span data-stu-id="df7a4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df7a4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df7a4-123">Authorization</span></span>|<span data-ttu-id="df7a4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="df7a4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df7a4-125">接受</span><span class="sxs-lookup"><span data-stu-id="df7a4-125">Accept</span></span>|<span data-ttu-id="df7a4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df7a4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df7a4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="df7a4-127">Request body</span></span>
<span data-ttu-id="df7a4-128">在请求正文中，提供 microsoftTunnelSite 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df7a4-128">In the request body, supply a JSON representation for the microsoftTunnelSite object.</span></span>

<span data-ttu-id="df7a4-129">下表显示创建 microsoftTunnelSite 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="df7a4-129">The following table shows the properties that are required when you create the microsoftTunnelSite.</span></span>

|<span data-ttu-id="df7a4-130">属性</span><span class="sxs-lookup"><span data-stu-id="df7a4-130">Property</span></span>|<span data-ttu-id="df7a4-131">类型</span><span class="sxs-lookup"><span data-stu-id="df7a4-131">Type</span></span>|<span data-ttu-id="df7a4-132">说明</span><span class="sxs-lookup"><span data-stu-id="df7a4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df7a4-133">id</span><span class="sxs-lookup"><span data-stu-id="df7a4-133">id</span></span>|<span data-ttu-id="df7a4-134">字符串</span><span class="sxs-lookup"><span data-stu-id="df7a4-134">String</span></span>|<span data-ttu-id="df7a4-135">MicrosoftTunnelSite 的 Id</span><span class="sxs-lookup"><span data-stu-id="df7a4-135">The MicrosoftTunnelSite's Id</span></span>|
|<span data-ttu-id="df7a4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="df7a4-136">displayName</span></span>|<span data-ttu-id="df7a4-137">字符串</span><span class="sxs-lookup"><span data-stu-id="df7a4-137">String</span></span>|<span data-ttu-id="df7a4-138">MicrosoftTunnelSite 的显示名称</span><span class="sxs-lookup"><span data-stu-id="df7a4-138">The MicrosoftTunnelSite's display name</span></span>|
|<span data-ttu-id="df7a4-139">description</span><span class="sxs-lookup"><span data-stu-id="df7a4-139">description</span></span>|<span data-ttu-id="df7a4-140">字符串</span><span class="sxs-lookup"><span data-stu-id="df7a4-140">String</span></span>|<span data-ttu-id="df7a4-141">MicrosoftTunnelSite 的说明</span><span class="sxs-lookup"><span data-stu-id="df7a4-141">The MicrosoftTunnelSite's description</span></span>|
|<span data-ttu-id="df7a4-142">publicAddress</span><span class="sxs-lookup"><span data-stu-id="df7a4-142">publicAddress</span></span>|<span data-ttu-id="df7a4-143">字符串</span><span class="sxs-lookup"><span data-stu-id="df7a4-143">String</span></span>|<span data-ttu-id="df7a4-144">MicrosoftTunnelSite 的公共域名或 IP 地址</span><span class="sxs-lookup"><span data-stu-id="df7a4-144">The MicrosoftTunnelSite's public domain name or IP address</span></span>|
|<span data-ttu-id="df7a4-145">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="df7a4-145">roleScopeTagIds</span></span>|<span data-ttu-id="df7a4-146">String 集合</span><span class="sxs-lookup"><span data-stu-id="df7a4-146">String collection</span></span>|<span data-ttu-id="df7a4-147">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="df7a4-147">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="df7a4-148">响应</span><span class="sxs-lookup"><span data-stu-id="df7a4-148">Response</span></span>
<span data-ttu-id="df7a4-149">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df7a4-149">If successful, this method returns a `201 Created` response code and a [microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df7a4-150">示例</span><span class="sxs-lookup"><span data-stu-id="df7a4-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="df7a4-151">请求</span><span class="sxs-lookup"><span data-stu-id="df7a4-151">Request</span></span>
<span data-ttu-id="df7a4-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df7a4-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites
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

### <a name="response"></a><span data-ttu-id="df7a4-153">响应</span><span class="sxs-lookup"><span data-stu-id="df7a4-153">Response</span></span>
<span data-ttu-id="df7a4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="df7a4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




