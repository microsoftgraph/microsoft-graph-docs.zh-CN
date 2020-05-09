---
title: createCopy 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e25371a5efb1a9cc342bb6122b464d304848b4ba
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177245"
---
# <a name="createcopy-action"></a><span data-ttu-id="5f682-103">createCopy 操作</span><span class="sxs-lookup"><span data-stu-id="5f682-103">createCopy action</span></span>

<span data-ttu-id="5f682-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f682-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f682-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5f682-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f682-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5f682-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f682-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5f682-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f682-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5f682-108">Prerequisites</span></span>
<span data-ttu-id="5f682-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5f682-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f682-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f682-111">Permission type</span></span>|<span data-ttu-id="5f682-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5f682-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f682-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f682-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5f682-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f682-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5f682-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f682-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f682-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f682-116">Not supported.</span></span>|
|<span data-ttu-id="5f682-117">Application</span><span class="sxs-lookup"><span data-stu-id="5f682-117">Application</span></span>|<span data-ttu-id="5f682-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f682-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f682-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f682-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/createCopy
```

## <a name="request-headers"></a><span data-ttu-id="5f682-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f682-120">Request headers</span></span>
|<span data-ttu-id="5f682-121">标头</span><span class="sxs-lookup"><span data-stu-id="5f682-121">Header</span></span>|<span data-ttu-id="5f682-122">值</span><span class="sxs-lookup"><span data-stu-id="5f682-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f682-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f682-123">Authorization</span></span>|<span data-ttu-id="5f682-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5f682-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f682-125">接受</span><span class="sxs-lookup"><span data-stu-id="5f682-125">Accept</span></span>|<span data-ttu-id="5f682-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5f682-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f682-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f682-127">Request body</span></span>
<span data-ttu-id="5f682-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f682-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5f682-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="5f682-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5f682-130">属性</span><span class="sxs-lookup"><span data-stu-id="5f682-130">Property</span></span>|<span data-ttu-id="5f682-131">类型</span><span class="sxs-lookup"><span data-stu-id="5f682-131">Type</span></span>|<span data-ttu-id="5f682-132">说明</span><span class="sxs-lookup"><span data-stu-id="5f682-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f682-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5f682-133">displayName</span></span>|<span data-ttu-id="5f682-134">String</span><span class="sxs-lookup"><span data-stu-id="5f682-134">String</span></span>|<span data-ttu-id="5f682-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5f682-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5f682-136">响应</span><span class="sxs-lookup"><span data-stu-id="5f682-136">Response</span></span>
<span data-ttu-id="5f682-137">如果成功，此操作会在`200 OK`响应正文中返回响应代码和[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) 。</span><span class="sxs-lookup"><span data-stu-id="5f682-137">If successful, this action returns a `200 OK` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f682-138">示例</span><span class="sxs-lookup"><span data-stu-id="5f682-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f682-139">请求</span><span class="sxs-lookup"><span data-stu-id="5f682-139">Request</span></span>
<span data-ttu-id="5f682-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5f682-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/createCopy

Content-type: application/json
Content-length: 43

{
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="5f682-141">响应</span><span class="sxs-lookup"><span data-stu-id="5f682-141">Response</span></span>
<span data-ttu-id="5f682-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5f682-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 418

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementIntent",
    "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
    "displayName": "Display Name value",
    "description": "Description value",
    "isAssigned": true,
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "templateId": "Template Id value",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```



