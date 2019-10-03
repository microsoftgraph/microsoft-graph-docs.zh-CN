---
title: 列出 deviceConfigurationDeviceStatuses
description: 列出 deviceConfigurationDeviceStatus 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bbeb2b99aec3760f0970d8b984c7a791ec159be7
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368699"
---
# <a name="list-deviceconfigurationdevicestatuses"></a><span data-ttu-id="809a2-103">列出 deviceConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="809a2-103">List deviceConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="809a2-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="809a2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="809a2-105">列出 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="809a2-105">List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="809a2-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="809a2-106">Prerequisites</span></span>
<span data-ttu-id="809a2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="809a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="809a2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="809a2-109">Permission type</span></span>|<span data-ttu-id="809a2-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="809a2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="809a2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="809a2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="809a2-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="809a2-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="809a2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="809a2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="809a2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="809a2-114">Not supported.</span></span>|
|<span data-ttu-id="809a2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="809a2-115">Application</span></span>|<span data-ttu-id="809a2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="809a2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="809a2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="809a2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="809a2-118">请求头</span><span class="sxs-lookup"><span data-stu-id="809a2-118">Request headers</span></span>
|<span data-ttu-id="809a2-119">标头</span><span class="sxs-lookup"><span data-stu-id="809a2-119">Header</span></span>|<span data-ttu-id="809a2-120">值</span><span class="sxs-lookup"><span data-stu-id="809a2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="809a2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="809a2-121">Authorization</span></span>|<span data-ttu-id="809a2-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="809a2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="809a2-123">接受</span><span class="sxs-lookup"><span data-stu-id="809a2-123">Accept</span></span>|<span data-ttu-id="809a2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="809a2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="809a2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="809a2-125">Request body</span></span>
<span data-ttu-id="809a2-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="809a2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="809a2-127">响应</span><span class="sxs-lookup"><span data-stu-id="809a2-127">Response</span></span>
<span data-ttu-id="809a2-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="809a2-128">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="809a2-129">示例</span><span class="sxs-lookup"><span data-stu-id="809a2-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="809a2-130">请求</span><span class="sxs-lookup"><span data-stu-id="809a2-130">Request</span></span>
<span data-ttu-id="809a2-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="809a2-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="809a2-132">响应</span><span class="sxs-lookup"><span data-stu-id="809a2-132">Response</span></span>
<span data-ttu-id="809a2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="809a2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 547

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
      "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




