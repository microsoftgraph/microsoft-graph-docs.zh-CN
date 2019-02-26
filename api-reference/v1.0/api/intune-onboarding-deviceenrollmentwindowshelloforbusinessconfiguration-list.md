---
title: 列出 deviceEnrollmentWindowsHelloForBusinessConfigurations
description: 列出 deviceEnrollmentWindowsHelloForBusinessConfiguration 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a566f17f47852ca2cec6c95306e19f20cb590b2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260058"
---
# <a name="list-deviceenrollmentwindowshelloforbusinessconfigurations"></a><span data-ttu-id="a6df5-103">列出 deviceEnrollmentWindowsHelloForBusinessConfigurations</span><span class="sxs-lookup"><span data-stu-id="a6df5-103">List deviceEnrollmentWindowsHelloForBusinessConfigurations</span></span>

> <span data-ttu-id="a6df5-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6df5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6df5-105">列出 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a6df5-105">List properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6df5-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a6df5-106">Prerequisites</span></span>
<span data-ttu-id="a6df5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a6df5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a6df5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6df5-109">Permission type</span></span>|<span data-ttu-id="a6df5-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a6df5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6df5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6df5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a6df5-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6df5-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a6df5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6df5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6df5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6df5-114">Not supported.</span></span>|
|<span data-ttu-id="a6df5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6df5-115">Application</span></span>|<span data-ttu-id="a6df5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6df5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6df5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6df5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a6df5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6df5-118">Request headers</span></span>
|<span data-ttu-id="a6df5-119">标头</span><span class="sxs-lookup"><span data-stu-id="a6df5-119">Header</span></span>|<span data-ttu-id="a6df5-120">值</span><span class="sxs-lookup"><span data-stu-id="a6df5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6df5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6df5-121">Authorization</span></span>|<span data-ttu-id="a6df5-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a6df5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6df5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a6df5-123">Accept</span></span>|<span data-ttu-id="a6df5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a6df5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6df5-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6df5-125">Request body</span></span>
<span data-ttu-id="a6df5-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a6df5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6df5-127">响应</span><span class="sxs-lookup"><span data-stu-id="a6df5-127">Response</span></span>
<span data-ttu-id="a6df5-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a6df5-128">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6df5-129">示例</span><span class="sxs-lookup"><span data-stu-id="a6df5-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6df5-130">请求</span><span class="sxs-lookup"><span data-stu-id="a6df5-130">Request</span></span>
<span data-ttu-id="a6df5-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a6df5-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="a6df5-132">响应</span><span class="sxs-lookup"><span data-stu-id="a6df5-132">Response</span></span>
<span data-ttu-id="a6df5-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a6df5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 914

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
      "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "pinMinimumLength": 0,
      "pinMaximumLength": 0,
      "pinUppercaseCharactersUsage": "required",
      "pinLowercaseCharactersUsage": "required",
      "pinSpecialCharactersUsage": "required",
      "state": "enabled",
      "securityDeviceRequired": true,
      "unlockWithBiometricsEnabled": true,
      "remotePassportEnabled": true,
      "pinPreviousBlockCount": 5,
      "pinExpirationInDays": 3,
      "enhancedBiometricsState": "enabled"
    }
  ]
}
```



