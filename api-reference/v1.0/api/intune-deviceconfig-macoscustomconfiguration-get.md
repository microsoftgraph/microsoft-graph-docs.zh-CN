---
title: 获取 macOSCustomConfiguration
description: 读取 macOSCustomConfiguration 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 768a93bcde5bfe4924236b076b3767295a83fed0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997496"
---
# <a name="get-macoscustomconfiguration"></a><span data-ttu-id="f046c-103">获取 macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="f046c-103">Get macOSCustomConfiguration</span></span>

> <span data-ttu-id="f046c-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f046c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f046c-105">读取 [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f046c-105">Read properties and relationships of the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f046c-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="f046c-106">Prerequisites</span></span>
<span data-ttu-id="f046c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f046c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f046c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f046c-109">Permission type</span></span>|<span data-ttu-id="f046c-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f046c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f046c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f046c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f046c-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f046c-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f046c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f046c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f046c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f046c-114">Not supported.</span></span>|
|<span data-ttu-id="f046c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f046c-115">Application</span></span>|<span data-ttu-id="f046c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f046c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f046c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f046c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f046c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f046c-118">Optional query parameters</span></span>
<span data-ttu-id="f046c-119">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f046c-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f046c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f046c-120">Request headers</span></span>
|<span data-ttu-id="f046c-121">标头</span><span class="sxs-lookup"><span data-stu-id="f046c-121">Header</span></span>|<span data-ttu-id="f046c-122">值</span><span class="sxs-lookup"><span data-stu-id="f046c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f046c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f046c-123">Authorization</span></span>|<span data-ttu-id="f046c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f046c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f046c-125">接受</span><span class="sxs-lookup"><span data-stu-id="f046c-125">Accept</span></span>|<span data-ttu-id="f046c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f046c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f046c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f046c-127">Request body</span></span>
<span data-ttu-id="f046c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f046c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f046c-129">响应</span><span class="sxs-lookup"><span data-stu-id="f046c-129">Response</span></span>
<span data-ttu-id="f046c-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f046c-130">If successful, this method returns a `200 OK` response code and [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f046c-131">示例</span><span class="sxs-lookup"><span data-stu-id="f046c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f046c-132">请求</span><span class="sxs-lookup"><span data-stu-id="f046c-132">Request</span></span>
<span data-ttu-id="f046c-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f046c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f046c-134">响应</span><span class="sxs-lookup"><span data-stu-id="f046c-134">Response</span></span>
<span data-ttu-id="f046c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f046c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 492

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
    "id": "a253835d-835d-a253-5d83-53a25d8353a2",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "payloadName": "Payload Name value",
    "payloadFileName": "Payload File Name value",
    "payload": "cGF5bG9hZA=="
  }
}
```



