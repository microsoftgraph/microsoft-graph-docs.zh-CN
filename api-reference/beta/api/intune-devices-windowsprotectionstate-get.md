---
title: 获取 windowsProtectionState
description: 读取属性和 windowsProtectionState 对象的关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 323e2ab2f0ff0c089c2dcc304fa62c31857ae31b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881194"
---
# <a name="get-windowsprotectionstate"></a><span data-ttu-id="29229-103">获取 windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="29229-103">Get windowsProtectionState</span></span>

> <span data-ttu-id="29229-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="29229-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29229-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="29229-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29229-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="29229-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29229-107">读取属性和[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="29229-107">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="29229-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="29229-108">Prerequisites</span></span>
<span data-ttu-id="29229-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="29229-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29229-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="29229-111">Permission type</span></span>|<span data-ttu-id="29229-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="29229-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29229-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29229-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29229-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="29229-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="29229-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29229-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29229-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="29229-116">Not supported.</span></span>|
|<span data-ttu-id="29229-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="29229-117">Application</span></span>|<span data-ttu-id="29229-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="29229-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29229-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29229-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="optional-query-parameters"></a><span data-ttu-id="29229-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="29229-120">Optional query parameters</span></span>
<span data-ttu-id="29229-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="29229-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="29229-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="29229-122">Request headers</span></span>
|<span data-ttu-id="29229-123">标头</span><span class="sxs-lookup"><span data-stu-id="29229-123">Header</span></span>|<span data-ttu-id="29229-124">值</span><span class="sxs-lookup"><span data-stu-id="29229-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29229-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="29229-125">Authorization</span></span>|<span data-ttu-id="29229-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="29229-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29229-127">Accept</span><span class="sxs-lookup"><span data-stu-id="29229-127">Accept</span></span>|<span data-ttu-id="29229-128">application/json</span><span class="sxs-lookup"><span data-stu-id="29229-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29229-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="29229-129">Request body</span></span>
<span data-ttu-id="29229-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="29229-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29229-131">响应</span><span class="sxs-lookup"><span data-stu-id="29229-131">Response</span></span>
<span data-ttu-id="29229-132">如果成功，此方法返回`200 OK`响应正文中的响应代码和[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="29229-132">If successful, this method returns a `200 OK` response code and [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29229-133">示例</span><span class="sxs-lookup"><span data-stu-id="29229-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="29229-134">请求</span><span class="sxs-lookup"><span data-stu-id="29229-134">Request</span></span>
<span data-ttu-id="29229-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="29229-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
```

### <a name="response"></a><span data-ttu-id="29229-136">响应</span><span class="sxs-lookup"><span data-stu-id="29229-136">Response</span></span>
<span data-ttu-id="29229-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="29229-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 971

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsProtectionState",
    "id": "1ac6ea5a-ea5a-1ac6-5aea-c61a5aeac61a",
    "malwareProtectionEnabled": true,
    "deviceState": "fullScanPending",
    "realTimeProtectionEnabled": true,
    "networkInspectionSystemEnabled": true,
    "quickScanOverdue": true,
    "fullScanOverdue": true,
    "signatureUpdateOverdue": true,
    "rebootRequired": true,
    "fullScanRequired": true,
    "engineVersion": "Engine Version value",
    "signatureVersion": "Signature Version value",
    "antiMalwareVersion": "Anti Malware Version value",
    "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
    "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
    "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
    "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
  }
}
```





