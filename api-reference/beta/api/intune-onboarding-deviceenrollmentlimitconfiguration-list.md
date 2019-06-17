---
title: 列出 deviceEnrollmentLimitConfigurations
description: 列出 deviceEnrollmentLimitConfiguration 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d136e92aa9ec5191669f79355c2d9a0fc8a20824
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981264"
---
# <a name="list-deviceenrollmentlimitconfigurations"></a><span data-ttu-id="b2cfc-103">列出 deviceEnrollmentLimitConfigurations</span><span class="sxs-lookup"><span data-stu-id="b2cfc-103">List deviceEnrollmentLimitConfigurations</span></span>

> <span data-ttu-id="b2cfc-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b2cfc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2cfc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b2cfc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2cfc-106">列出 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b2cfc-106">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2cfc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b2cfc-107">Prerequisites</span></span>
<span data-ttu-id="b2cfc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2cfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2cfc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2cfc-110">Permission type</span></span>|<span data-ttu-id="b2cfc-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b2cfc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2cfc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2cfc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2cfc-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2cfc-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b2cfc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2cfc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2cfc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2cfc-115">Not supported.</span></span>|
|<span data-ttu-id="b2cfc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2cfc-116">Application</span></span>|<span data-ttu-id="b2cfc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2cfc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2cfc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2cfc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b2cfc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2cfc-119">Request headers</span></span>
|<span data-ttu-id="b2cfc-120">标头</span><span class="sxs-lookup"><span data-stu-id="b2cfc-120">Header</span></span>|<span data-ttu-id="b2cfc-121">值</span><span class="sxs-lookup"><span data-stu-id="b2cfc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2cfc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2cfc-122">Authorization</span></span>|<span data-ttu-id="b2cfc-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b2cfc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2cfc-124">接受</span><span class="sxs-lookup"><span data-stu-id="b2cfc-124">Accept</span></span>|<span data-ttu-id="b2cfc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2cfc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2cfc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2cfc-126">Request body</span></span>
<span data-ttu-id="b2cfc-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b2cfc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2cfc-128">响应</span><span class="sxs-lookup"><span data-stu-id="b2cfc-128">Response</span></span>
<span data-ttu-id="b2cfc-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b2cfc-129">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentLimitConfiguration](../resources/intune-onboarding-deviceenrollmentlimitconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2cfc-130">示例</span><span class="sxs-lookup"><span data-stu-id="b2cfc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2cfc-131">请求</span><span class="sxs-lookup"><span data-stu-id="b2cfc-131">Request</span></span>
<span data-ttu-id="b2cfc-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b2cfc-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="b2cfc-133">响应</span><span class="sxs-lookup"><span data-stu-id="b2cfc-133">Response</span></span>
<span data-ttu-id="b2cfc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b2cfc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 446

{
  "value": [
    {
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
  ]
}
```





