---
title: 获取 securityBaselineDeviceState
description: 读取 securityBaselineDeviceState 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 81b744bd82a4af560ee9a6ed489245d9baa98511
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43381078"
---
# <a name="get-securitybaselinedevicestate"></a><span data-ttu-id="f65c8-103">获取 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="f65c8-103">Get securityBaselineDeviceState</span></span>

<span data-ttu-id="f65c8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f65c8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f65c8-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f65c8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f65c8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f65c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f65c8-107">读取[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f65c8-107">Read properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f65c8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f65c8-108">Prerequisites</span></span>
<span data-ttu-id="f65c8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f65c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f65c8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f65c8-111">Permission type</span></span>|<span data-ttu-id="f65c8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f65c8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f65c8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f65c8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f65c8-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f65c8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f65c8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f65c8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f65c8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f65c8-116">Not supported.</span></span>|
|<span data-ttu-id="f65c8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f65c8-117">Application</span></span>|<span data-ttu-id="f65c8-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f65c8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f65c8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f65c8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates/{securityBaselineDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f65c8-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f65c8-120">Optional query parameters</span></span>
<span data-ttu-id="f65c8-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f65c8-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f65c8-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f65c8-122">Request headers</span></span>
|<span data-ttu-id="f65c8-123">标头</span><span class="sxs-lookup"><span data-stu-id="f65c8-123">Header</span></span>|<span data-ttu-id="f65c8-124">值</span><span class="sxs-lookup"><span data-stu-id="f65c8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f65c8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f65c8-125">Authorization</span></span>|<span data-ttu-id="f65c8-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f65c8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f65c8-127">接受</span><span class="sxs-lookup"><span data-stu-id="f65c8-127">Accept</span></span>|<span data-ttu-id="f65c8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f65c8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f65c8-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f65c8-129">Request body</span></span>
<span data-ttu-id="f65c8-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f65c8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f65c8-131">响应</span><span class="sxs-lookup"><span data-stu-id="f65c8-131">Response</span></span>
<span data-ttu-id="f65c8-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f65c8-132">If successful, this method returns a `200 OK` response code and [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f65c8-133">示例</span><span class="sxs-lookup"><span data-stu-id="f65c8-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f65c8-134">请求</span><span class="sxs-lookup"><span data-stu-id="f65c8-134">Request</span></span>
<span data-ttu-id="f65c8-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f65c8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates/{securityBaselineDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="f65c8-136">响应</span><span class="sxs-lookup"><span data-stu-id="f65c8-136">Response</span></span>
<span data-ttu-id="f65c8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f65c8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 392

{
  "value": {
    "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
    "id": "182749bf-49bf-1827-bf49-2718bf492718",
    "managedDeviceId": "Managed Device Id value",
    "deviceDisplayName": "Device Display Name value",
    "userPrincipalName": "User Principal Name value",
    "state": "secure",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
  }
}
```



