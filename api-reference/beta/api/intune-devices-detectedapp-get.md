---
title: 获取 detectedApp
description: 读取 detectedApp 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b182ebe67d481d3f800b9b1e1e76749b9f1055d9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814678"
---
# <a name="get-detectedapp"></a><span data-ttu-id="cceca-103">获取 detectedApp</span><span class="sxs-lookup"><span data-stu-id="cceca-103">Get detectedApp</span></span>

> <span data-ttu-id="cceca-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cceca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cceca-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cceca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cceca-106">读取 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cceca-106">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cceca-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cceca-107">Prerequisites</span></span>
<span data-ttu-id="cceca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cceca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cceca-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cceca-110">Permission type</span></span>|<span data-ttu-id="cceca-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cceca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cceca-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cceca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cceca-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cceca-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="cceca-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cceca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cceca-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cceca-115">Not supported.</span></span>|
|<span data-ttu-id="cceca-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cceca-116">Application</span></span>|<span data-ttu-id="cceca-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cceca-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cceca-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cceca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cceca-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cceca-119">Optional query parameters</span></span>
<span data-ttu-id="cceca-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cceca-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cceca-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="cceca-121">Request headers</span></span>
|<span data-ttu-id="cceca-122">标头</span><span class="sxs-lookup"><span data-stu-id="cceca-122">Header</span></span>|<span data-ttu-id="cceca-123">值</span><span class="sxs-lookup"><span data-stu-id="cceca-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cceca-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cceca-124">Authorization</span></span>|<span data-ttu-id="cceca-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cceca-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cceca-126">接受</span><span class="sxs-lookup"><span data-stu-id="cceca-126">Accept</span></span>|<span data-ttu-id="cceca-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cceca-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cceca-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="cceca-128">Request body</span></span>
<span data-ttu-id="cceca-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cceca-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cceca-130">响应</span><span class="sxs-lookup"><span data-stu-id="cceca-130">Response</span></span>
<span data-ttu-id="cceca-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [detectedApp](../resources/intune-devices-detectedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cceca-131">If successful, this method returns a `200 OK` response code and [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cceca-132">示例</span><span class="sxs-lookup"><span data-stu-id="cceca-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="cceca-133">请求</span><span class="sxs-lookup"><span data-stu-id="cceca-133">Request</span></span>
<span data-ttu-id="cceca-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cceca-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/detectedApps/{detectedAppId}
```

### <a name="response"></a><span data-ttu-id="cceca-135">响应</span><span class="sxs-lookup"><span data-stu-id="cceca-135">Response</span></span>
<span data-ttu-id="cceca-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cceca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "value": {
    "@odata.type": "#microsoft.graph.detectedApp",
    "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
    "displayName": "Display Name value",
    "version": "Version value",
    "sizeInByte": 10,
    "deviceCount": 11
  }
}
```




