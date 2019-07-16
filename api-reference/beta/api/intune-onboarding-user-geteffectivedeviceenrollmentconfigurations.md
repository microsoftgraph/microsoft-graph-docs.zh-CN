---
title: getEffectiveDeviceEnrollmentConfigurations 函数
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 28c0f774192f3fde33c654047d10f67ad7cffdcd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725910"
---
# <a name="geteffectivedeviceenrollmentconfigurations-function"></a><span data-ttu-id="64873-103">getEffectiveDeviceEnrollmentConfigurations 函数</span><span class="sxs-lookup"><span data-stu-id="64873-103">getEffectiveDeviceEnrollmentConfigurations function</span></span>

> <span data-ttu-id="64873-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="64873-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64873-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="64873-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64873-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="64873-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64873-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="64873-107">Prerequisites</span></span>
<span data-ttu-id="64873-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64873-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64873-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="64873-110">Permission type</span></span>|<span data-ttu-id="64873-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="64873-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64873-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64873-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64873-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="64873-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="64873-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64873-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64873-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="64873-115">Not supported.</span></span>|
|<span data-ttu-id="64873-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="64873-116">Application</span></span>|<span data-ttu-id="64873-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="64873-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64873-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64873-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="64873-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="64873-119">Request headers</span></span>
|<span data-ttu-id="64873-120">标头</span><span class="sxs-lookup"><span data-stu-id="64873-120">Header</span></span>|<span data-ttu-id="64873-121">值</span><span class="sxs-lookup"><span data-stu-id="64873-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64873-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="64873-122">Authorization</span></span>|<span data-ttu-id="64873-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="64873-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64873-124">接受</span><span class="sxs-lookup"><span data-stu-id="64873-124">Accept</span></span>|<span data-ttu-id="64873-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64873-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64873-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="64873-126">Request body</span></span>
<span data-ttu-id="64873-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="64873-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64873-128">响应</span><span class="sxs-lookup"><span data-stu-id="64873-128">Response</span></span>
<span data-ttu-id="64873-129">如果成功, 此函数会在`200 OK`响应正文中返回响应代码和[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)集合。</span><span class="sxs-lookup"><span data-stu-id="64873-129">If successful, this function returns a `200 OK` response code and a [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64873-130">示例</span><span class="sxs-lookup"><span data-stu-id="64873-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="64873-131">请求</span><span class="sxs-lookup"><span data-stu-id="64873-131">Request</span></span>
<span data-ttu-id="64873-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="64873-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="64873-133">响应</span><span class="sxs-lookup"><span data-stu-id="64873-133">Response</span></span>
<span data-ttu-id="64873-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="64873-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





