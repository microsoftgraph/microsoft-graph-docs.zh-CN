---
title: 获取 deviceManagementIntent
description: 读取 deviceManagementIntent 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c4f03b7d5764fa0dc5b2c635774bb1c21537c6de
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37180977"
---
# <a name="get-devicemanagementintent"></a><span data-ttu-id="62102-103">获取 deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="62102-103">Get deviceManagementIntent</span></span>

> <span data-ttu-id="62102-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="62102-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62102-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="62102-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62102-106">读取[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="62102-106">Read properties and relationships of the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62102-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="62102-107">Prerequisites</span></span>
<span data-ttu-id="62102-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62102-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62102-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="62102-110">Permission type</span></span>|<span data-ttu-id="62102-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="62102-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62102-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62102-112">Delegated (work or school account)</span></span>|<span data-ttu-id="62102-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="62102-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="62102-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62102-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62102-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="62102-115">Not supported.</span></span>|
|<span data-ttu-id="62102-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="62102-116">Application</span></span>|<span data-ttu-id="62102-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="62102-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="62102-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62102-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="62102-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="62102-119">Optional query parameters</span></span>
<span data-ttu-id="62102-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="62102-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="62102-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="62102-121">Request headers</span></span>
|<span data-ttu-id="62102-122">标头</span><span class="sxs-lookup"><span data-stu-id="62102-122">Header</span></span>|<span data-ttu-id="62102-123">值</span><span class="sxs-lookup"><span data-stu-id="62102-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62102-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="62102-124">Authorization</span></span>|<span data-ttu-id="62102-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="62102-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62102-126">接受</span><span class="sxs-lookup"><span data-stu-id="62102-126">Accept</span></span>|<span data-ttu-id="62102-127">application/json</span><span class="sxs-lookup"><span data-stu-id="62102-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62102-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="62102-128">Request body</span></span>
<span data-ttu-id="62102-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="62102-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62102-130">响应</span><span class="sxs-lookup"><span data-stu-id="62102-130">Response</span></span>
<span data-ttu-id="62102-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="62102-131">If successful, this method returns a `200 OK` response code and [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62102-132">示例</span><span class="sxs-lookup"><span data-stu-id="62102-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="62102-133">请求</span><span class="sxs-lookup"><span data-stu-id="62102-133">Request</span></span>
<span data-ttu-id="62102-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="62102-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}
```

### <a name="response"></a><span data-ttu-id="62102-135">响应</span><span class="sxs-lookup"><span data-stu-id="62102-135">Response</span></span>
<span data-ttu-id="62102-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="62102-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




