---
title: getEffectiveDeviceEnrollmentConfigurations 函数
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ee8eb2ff3a15d234d05ed28a13f600e7e47e4d53
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971708"
---
# <a name="geteffectivedeviceenrollmentconfigurations-function"></a><span data-ttu-id="b24d7-103">getEffectiveDeviceEnrollmentConfigurations 函数</span><span class="sxs-lookup"><span data-stu-id="b24d7-103">getEffectiveDeviceEnrollmentConfigurations function</span></span>

> <span data-ttu-id="b24d7-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b24d7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b24d7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b24d7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b24d7-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b24d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b24d7-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b24d7-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b24d7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b24d7-108">Prerequisites</span></span>

<span data-ttu-id="b24d7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b24d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b24d7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b24d7-111">Permission type</span></span>|<span data-ttu-id="b24d7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b24d7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b24d7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b24d7-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b24d7-114">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="b24d7-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b24d7-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b24d7-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b24d7-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b24d7-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b24d7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b24d7-117">Not supported.</span></span>|
|<span data-ttu-id="b24d7-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b24d7-118">Application</span></span>|<span data-ttu-id="b24d7-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="b24d7-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b24d7-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b24d7-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b24d7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b24d7-121">Request headers</span></span>

|<span data-ttu-id="b24d7-122">标头</span><span class="sxs-lookup"><span data-stu-id="b24d7-122">Header</span></span>|<span data-ttu-id="b24d7-123">值</span><span class="sxs-lookup"><span data-stu-id="b24d7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b24d7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b24d7-124">Authorization</span></span>|<span data-ttu-id="b24d7-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b24d7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b24d7-126">接受</span><span class="sxs-lookup"><span data-stu-id="b24d7-126">Accept</span></span>|<span data-ttu-id="b24d7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b24d7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b24d7-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b24d7-128">Request body</span></span>

<span data-ttu-id="b24d7-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b24d7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b24d7-130">响应</span><span class="sxs-lookup"><span data-stu-id="b24d7-130">Response</span></span>

<span data-ttu-id="b24d7-131">如果成功, 此函数会在`200 OK`响应正文中返回响应代码和[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)集合。</span><span class="sxs-lookup"><span data-stu-id="b24d7-131">If successful, this function returns a `200 OK` response code and a [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b24d7-132">示例</span><span class="sxs-lookup"><span data-stu-id="b24d7-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b24d7-133">请求</span><span class="sxs-lookup"><span data-stu-id="b24d7-133">Request</span></span>

<span data-ttu-id="b24d7-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b24d7-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="b24d7-135">响应</span><span class="sxs-lookup"><span data-stu-id="b24d7-135">Response</span></span>

<span data-ttu-id="b24d7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b24d7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



