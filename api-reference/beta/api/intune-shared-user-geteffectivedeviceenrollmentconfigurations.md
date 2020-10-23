---
title: getEffectiveDeviceEnrollmentConfigurations 函数
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8b613834d06427f1687b839a79c2c24f14630c82
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728618"
---
# <a name="geteffectivedeviceenrollmentconfigurations-function"></a><span data-ttu-id="382ba-103">getEffectiveDeviceEnrollmentConfigurations 函数</span><span class="sxs-lookup"><span data-stu-id="382ba-103">getEffectiveDeviceEnrollmentConfigurations function</span></span>

<span data-ttu-id="382ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="382ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="382ba-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="382ba-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="382ba-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="382ba-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="382ba-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="382ba-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="382ba-108">尚未记录</span><span class="sxs-lookup"><span data-stu-id="382ba-108">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="382ba-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="382ba-109">Prerequisites</span></span>

<span data-ttu-id="382ba-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="382ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="382ba-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="382ba-112">Permission type</span></span>|<span data-ttu-id="382ba-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="382ba-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="382ba-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="382ba-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="382ba-115">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="382ba-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="382ba-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="382ba-116">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="382ba-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="382ba-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="382ba-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="382ba-118">Not supported.</span></span>|
|<span data-ttu-id="382ba-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="382ba-119">Application</span></span>||
| <span data-ttu-id="382ba-120">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="382ba-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="382ba-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="382ba-121">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="382ba-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="382ba-122">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="382ba-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="382ba-123">Request headers</span></span>

|<span data-ttu-id="382ba-124">标头</span><span class="sxs-lookup"><span data-stu-id="382ba-124">Header</span></span>|<span data-ttu-id="382ba-125">值</span><span class="sxs-lookup"><span data-stu-id="382ba-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="382ba-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="382ba-126">Authorization</span></span>|<span data-ttu-id="382ba-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="382ba-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="382ba-128">接受</span><span class="sxs-lookup"><span data-stu-id="382ba-128">Accept</span></span>|<span data-ttu-id="382ba-129">application/json</span><span class="sxs-lookup"><span data-stu-id="382ba-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="382ba-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="382ba-130">Request body</span></span>

<span data-ttu-id="382ba-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="382ba-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="382ba-132">响应</span><span class="sxs-lookup"><span data-stu-id="382ba-132">Response</span></span>

<span data-ttu-id="382ba-133">如果成功，此函数会 `200 OK` 在响应正文中返回响应代码和 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="382ba-133">If successful, this function returns a `200 OK` response code and a [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="382ba-134">示例</span><span class="sxs-lookup"><span data-stu-id="382ba-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="382ba-135">请求</span><span class="sxs-lookup"><span data-stu-id="382ba-135">Request</span></span>

<span data-ttu-id="382ba-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="382ba-136">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="382ba-137">响应</span><span class="sxs-lookup"><span data-stu-id="382ba-137">Response</span></span>

<span data-ttu-id="382ba-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="382ba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 422

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
      "id": "df13d8b9-d8b9-df13-b9d8-13dfb9d813df",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7
    }
  ]
}
```











