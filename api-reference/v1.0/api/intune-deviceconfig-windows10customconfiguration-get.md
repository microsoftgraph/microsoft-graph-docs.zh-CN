---
title: 获取 windows10CustomConfiguration
description: 读取 windows10CustomConfiguration 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c306cc7216f8f4b7a61c52f5f3cc14c2c76f70da
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365584"
---
# <a name="get-windows10customconfiguration"></a><span data-ttu-id="afecc-103">获取 windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="afecc-103">Get windows10CustomConfiguration</span></span>

> <span data-ttu-id="afecc-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="afecc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afecc-105">读取 [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="afecc-105">Read properties and relationships of the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afecc-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="afecc-106">Prerequisites</span></span>
<span data-ttu-id="afecc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="afecc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afecc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="afecc-109">Permission type</span></span>|<span data-ttu-id="afecc-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="afecc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afecc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="afecc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="afecc-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="afecc-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="afecc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="afecc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afecc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="afecc-114">Not supported.</span></span>|
|<span data-ttu-id="afecc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="afecc-115">Application</span></span>|<span data-ttu-id="afecc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="afecc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="afecc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="afecc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="afecc-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="afecc-118">Optional query parameters</span></span>
<span data-ttu-id="afecc-119">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="afecc-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="afecc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="afecc-120">Request headers</span></span>
|<span data-ttu-id="afecc-121">标头</span><span class="sxs-lookup"><span data-stu-id="afecc-121">Header</span></span>|<span data-ttu-id="afecc-122">值</span><span class="sxs-lookup"><span data-stu-id="afecc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afecc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="afecc-123">Authorization</span></span>|<span data-ttu-id="afecc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="afecc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afecc-125">接受</span><span class="sxs-lookup"><span data-stu-id="afecc-125">Accept</span></span>|<span data-ttu-id="afecc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="afecc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afecc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="afecc-127">Request body</span></span>
<span data-ttu-id="afecc-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="afecc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afecc-129">响应</span><span class="sxs-lookup"><span data-stu-id="afecc-129">Response</span></span>
<span data-ttu-id="afecc-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="afecc-130">If successful, this method returns a `200 OK` response code and [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afecc-131">示例</span><span class="sxs-lookup"><span data-stu-id="afecc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="afecc-132">请求</span><span class="sxs-lookup"><span data-stu-id="afecc-132">Request</span></span>
<span data-ttu-id="afecc-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="afecc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="afecc-134">响应</span><span class="sxs-lookup"><span data-stu-id="afecc-134">Response</span></span>
<span data-ttu-id="afecc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="afecc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 627

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
    "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "omaSettings": [
      {
        "@odata.type": "microsoft.graph.omaSettingInteger",
        "displayName": "Display Name value",
        "description": "Description value",
        "omaUri": "Oma Uri value",
        "value": 5
      }
    ]
  }
}
```




