---
title: hasPayloadLinks 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 51f83e508e5904ef57c1b7ce7fc70e5de22b9238
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863168"
---
# <a name="haspayloadlinks-action"></a><span data-ttu-id="10287-103">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="10287-103">hasPayloadLinks action</span></span>

<span data-ttu-id="10287-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10287-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10287-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="10287-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10287-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="10287-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10287-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="10287-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10287-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="10287-108">Prerequisites</span></span>
<span data-ttu-id="10287-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="10287-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10287-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="10287-111">Permission type</span></span>|<span data-ttu-id="10287-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="10287-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10287-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10287-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="10287-114">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="10287-114">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="10287-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="10287-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="10287-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10287-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10287-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="10287-117">Not supported.</span></span>|
|<span data-ttu-id="10287-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="10287-118">Application</span></span>||
| <span data-ttu-id="10287-119">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="10287-119">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="10287-120">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="10287-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10287-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10287-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/hasPayloadLinks
```

## <a name="request-headers"></a><span data-ttu-id="10287-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="10287-122">Request headers</span></span>
|<span data-ttu-id="10287-123">标头</span><span class="sxs-lookup"><span data-stu-id="10287-123">Header</span></span>|<span data-ttu-id="10287-124">值</span><span class="sxs-lookup"><span data-stu-id="10287-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10287-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="10287-125">Authorization</span></span>|<span data-ttu-id="10287-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="10287-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10287-127">接受</span><span class="sxs-lookup"><span data-stu-id="10287-127">Accept</span></span>|<span data-ttu-id="10287-128">application/json</span><span class="sxs-lookup"><span data-stu-id="10287-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10287-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="10287-129">Request body</span></span>
<span data-ttu-id="10287-130">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10287-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="10287-131">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="10287-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="10287-132">属性</span><span class="sxs-lookup"><span data-stu-id="10287-132">Property</span></span>|<span data-ttu-id="10287-133">类型</span><span class="sxs-lookup"><span data-stu-id="10287-133">Type</span></span>|<span data-ttu-id="10287-134">说明</span><span class="sxs-lookup"><span data-stu-id="10287-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10287-135">payloadIds</span><span class="sxs-lookup"><span data-stu-id="10287-135">payloadIds</span></span>|<span data-ttu-id="10287-136">String collection</span><span class="sxs-lookup"><span data-stu-id="10287-136">String collection</span></span>|<span data-ttu-id="10287-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="10287-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="10287-138">响应</span><span class="sxs-lookup"><span data-stu-id="10287-138">Response</span></span>
<span data-ttu-id="10287-139">如果成功，此操作在响应正文中返回 响应代码和 `200 OK` [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="10287-139">If successful, this action returns a `200 OK` response code and a [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10287-140">示例</span><span class="sxs-lookup"><span data-stu-id="10287-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="10287-141">请求</span><span class="sxs-lookup"><span data-stu-id="10287-141">Request</span></span>
<span data-ttu-id="10287-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="10287-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/hasPayloadLinks

Content-type: application/json
Content-length: 53

{
  "payloadIds": [
    "Payload Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="10287-143">响应</span><span class="sxs-lookup"><span data-stu-id="10287-143">Response</span></span>
<span data-ttu-id="10287-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="10287-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": [
    {
      "@odata.type": "microsoft.graph.hasPayloadLinkResultItem",
      "payloadId": "Payload Id value",
      "hasLink": true,
      "error": "Error value",
      "sources": [
        "policySets"
      ]
    }
  ]
}
```







