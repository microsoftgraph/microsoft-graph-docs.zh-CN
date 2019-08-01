---
title: 获取 deviceEnrollmentLimitConfiguration
description: 读取 deviceEnrollmentLimitConfiguration 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 188e231f2bdc06cfb15ccae13804a197bd8269dd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017999"
---
# <a name="get-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="31bc1-103">获取 deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="31bc1-103">Get deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="31bc1-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="31bc1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31bc1-105">读取 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="31bc1-105">Read properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31bc1-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="31bc1-106">Prerequisites</span></span>
<span data-ttu-id="31bc1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="31bc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31bc1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="31bc1-109">Permission type</span></span>|<span data-ttu-id="31bc1-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="31bc1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31bc1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31bc1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="31bc1-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="31bc1-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="31bc1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31bc1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31bc1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="31bc1-114">Not supported.</span></span>|
|<span data-ttu-id="31bc1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="31bc1-115">Application</span></span>|<span data-ttu-id="31bc1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="31bc1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31bc1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31bc1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="31bc1-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="31bc1-118">Optional query parameters</span></span>
<span data-ttu-id="31bc1-119">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="31bc1-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31bc1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="31bc1-120">Request headers</span></span>
|<span data-ttu-id="31bc1-121">标头</span><span class="sxs-lookup"><span data-stu-id="31bc1-121">Header</span></span>|<span data-ttu-id="31bc1-122">值</span><span class="sxs-lookup"><span data-stu-id="31bc1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31bc1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="31bc1-123">Authorization</span></span>|<span data-ttu-id="31bc1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="31bc1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31bc1-125">接受</span><span class="sxs-lookup"><span data-stu-id="31bc1-125">Accept</span></span>|<span data-ttu-id="31bc1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31bc1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31bc1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="31bc1-127">Request body</span></span>
<span data-ttu-id="31bc1-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="31bc1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31bc1-129">响应</span><span class="sxs-lookup"><span data-stu-id="31bc1-129">Response</span></span>
<span data-ttu-id="31bc1-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="31bc1-130">If successful, this method returns a `200 OK` response code and [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31bc1-131">示例</span><span class="sxs-lookup"><span data-stu-id="31bc1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="31bc1-132">请求</span><span class="sxs-lookup"><span data-stu-id="31bc1-132">Request</span></span>
<span data-ttu-id="31bc1-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="31bc1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="31bc1-134">响应</span><span class="sxs-lookup"><span data-stu-id="31bc1-134">Response</span></span>
<span data-ttu-id="31bc1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="31bc1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 414

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
    "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
    "displayName": "Display Name value",
    "description": "Description value",
    "priority": 8,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "version": 7,
    "limit": 5
  }
}
```



