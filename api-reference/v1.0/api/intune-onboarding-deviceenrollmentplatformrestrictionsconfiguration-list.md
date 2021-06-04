---
title: 列出 deviceEnrollmentPlatformRestrictionsConfigurations
description: 列出 deviceEnrollmentPlatformRestrictionsConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f1b1c5e77818a57bd0de2ea0817ebb17d09c3095
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52744678"
---
# <a name="list-deviceenrollmentplatformrestrictionsconfigurations"></a><span data-ttu-id="10a78-103">列出 deviceEnrollmentPlatformRestrictionsConfigurations</span><span class="sxs-lookup"><span data-stu-id="10a78-103">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>

<span data-ttu-id="10a78-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10a78-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10a78-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="10a78-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10a78-106">列出 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="10a78-106">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10a78-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="10a78-107">Prerequisites</span></span>
<span data-ttu-id="10a78-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="10a78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10a78-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="10a78-110">Permission type</span></span>|<span data-ttu-id="10a78-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="10a78-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10a78-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10a78-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10a78-113">DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10a78-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="10a78-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10a78-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10a78-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="10a78-115">Not supported.</span></span>|
|<span data-ttu-id="10a78-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="10a78-116">Application</span></span>|<span data-ttu-id="10a78-117">DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10a78-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10a78-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10a78-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="10a78-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="10a78-119">Request headers</span></span>
|<span data-ttu-id="10a78-120">标头</span><span class="sxs-lookup"><span data-stu-id="10a78-120">Header</span></span>|<span data-ttu-id="10a78-121">值</span><span class="sxs-lookup"><span data-stu-id="10a78-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10a78-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="10a78-122">Authorization</span></span>|<span data-ttu-id="10a78-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="10a78-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10a78-124">接受</span><span class="sxs-lookup"><span data-stu-id="10a78-124">Accept</span></span>|<span data-ttu-id="10a78-125">application/json</span><span class="sxs-lookup"><span data-stu-id="10a78-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10a78-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="10a78-126">Request body</span></span>
<span data-ttu-id="10a78-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="10a78-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10a78-128">响应</span><span class="sxs-lookup"><span data-stu-id="10a78-128">Response</span></span>
<span data-ttu-id="10a78-129">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="10a78-129">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10a78-130">示例</span><span class="sxs-lookup"><span data-stu-id="10a78-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="10a78-131">请求</span><span class="sxs-lookup"><span data-stu-id="10a78-131">Request</span></span>
<span data-ttu-id="10a78-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="10a78-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="10a78-133">响应</span><span class="sxs-lookup"><span data-stu-id="10a78-133">Response</span></span>
<span data-ttu-id="10a78-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="10a78-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2027

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
      "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "iosRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      },
      "windowsRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      },
      "windowsMobileRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      },
      "androidRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      },
      "macOSRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      }
    }
  ]
}
```




