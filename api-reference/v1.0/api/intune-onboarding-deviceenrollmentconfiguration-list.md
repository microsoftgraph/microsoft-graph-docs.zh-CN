---
title: 列出 deviceEnrollmentConfigurations
description: 列出 deviceEnrollmentConfiguration 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 871032421bd18eab0a622df0449804fa1da82e3f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018062"
---
# <a name="list-deviceenrollmentconfigurations"></a><span data-ttu-id="29b54-103">列出 deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="29b54-103">List deviceEnrollmentConfigurations</span></span>

> <span data-ttu-id="29b54-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="29b54-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29b54-105">列出 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="29b54-105">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29b54-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="29b54-106">Prerequisites</span></span>
<span data-ttu-id="29b54-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29b54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29b54-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="29b54-109">Permission type</span></span>|<span data-ttu-id="29b54-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="29b54-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29b54-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29b54-111">Delegated (work or school account)</span></span>|<span data-ttu-id="29b54-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="29b54-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="29b54-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29b54-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29b54-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="29b54-114">Not supported.</span></span>|
|<span data-ttu-id="29b54-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="29b54-115">Application</span></span>|<span data-ttu-id="29b54-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="29b54-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29b54-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29b54-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="29b54-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="29b54-118">Request headers</span></span>
|<span data-ttu-id="29b54-119">标头</span><span class="sxs-lookup"><span data-stu-id="29b54-119">Header</span></span>|<span data-ttu-id="29b54-120">值</span><span class="sxs-lookup"><span data-stu-id="29b54-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29b54-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="29b54-121">Authorization</span></span>|<span data-ttu-id="29b54-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="29b54-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29b54-123">接受</span><span class="sxs-lookup"><span data-stu-id="29b54-123">Accept</span></span>|<span data-ttu-id="29b54-124">application/json</span><span class="sxs-lookup"><span data-stu-id="29b54-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29b54-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="29b54-125">Request body</span></span>
<span data-ttu-id="29b54-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="29b54-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29b54-127">响应</span><span class="sxs-lookup"><span data-stu-id="29b54-127">Response</span></span>
<span data-ttu-id="29b54-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="29b54-128">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29b54-129">示例</span><span class="sxs-lookup"><span data-stu-id="29b54-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="29b54-130">请求</span><span class="sxs-lookup"><span data-stu-id="29b54-130">Request</span></span>
<span data-ttu-id="29b54-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="29b54-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="29b54-132">响应</span><span class="sxs-lookup"><span data-stu-id="29b54-132">Response</span></span>
<span data-ttu-id="29b54-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="29b54-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



