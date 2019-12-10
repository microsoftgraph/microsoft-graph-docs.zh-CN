---
title: 列出 deviceEnrollmentConfigurations
description: 列出 deviceEnrollmentConfiguration 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3323599ba9731a109b3dd6841fbc90179b5cf48a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940017"
---
# <a name="list-deviceenrollmentconfigurations"></a><span data-ttu-id="1d21d-103">列出 deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="1d21d-103">List deviceEnrollmentConfigurations</span></span>

> <span data-ttu-id="1d21d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1d21d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d21d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1d21d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d21d-106">列出 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1d21d-106">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d21d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1d21d-107">Prerequisites</span></span>
<span data-ttu-id="1d21d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1d21d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d21d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1d21d-110">Permission type</span></span>|<span data-ttu-id="1d21d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1d21d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d21d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1d21d-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1d21d-113">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="1d21d-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="1d21d-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d21d-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="1d21d-115">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="1d21d-115">&nbsp; &nbsp; **Policy Set**</span></span>| <span data-ttu-id="1d21d-116">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d21d-116">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="1d21d-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1d21d-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d21d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d21d-118">Not supported.</span></span>|
|<span data-ttu-id="1d21d-119">Application</span><span class="sxs-lookup"><span data-stu-id="1d21d-119">Application</span></span>||
| <span data-ttu-id="1d21d-120">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="1d21d-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="1d21d-121">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d21d-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="1d21d-122">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="1d21d-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="1d21d-123">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d21d-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d21d-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d21d-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1d21d-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="1d21d-125">Request headers</span></span>
|<span data-ttu-id="1d21d-126">标头</span><span class="sxs-lookup"><span data-stu-id="1d21d-126">Header</span></span>|<span data-ttu-id="1d21d-127">值</span><span class="sxs-lookup"><span data-stu-id="1d21d-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d21d-128">授权</span><span class="sxs-lookup"><span data-stu-id="1d21d-128">Authorization</span></span>|<span data-ttu-id="1d21d-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1d21d-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d21d-130">接受</span><span class="sxs-lookup"><span data-stu-id="1d21d-130">Accept</span></span>|<span data-ttu-id="1d21d-131">application/json</span><span class="sxs-lookup"><span data-stu-id="1d21d-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d21d-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="1d21d-132">Request body</span></span>
<span data-ttu-id="1d21d-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1d21d-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d21d-134">响应</span><span class="sxs-lookup"><span data-stu-id="1d21d-134">Response</span></span>
<span data-ttu-id="1d21d-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1d21d-135">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d21d-136">示例</span><span class="sxs-lookup"><span data-stu-id="1d21d-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d21d-137">请求</span><span class="sxs-lookup"><span data-stu-id="1d21d-137">Request</span></span>
<span data-ttu-id="1d21d-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1d21d-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="1d21d-139">响应</span><span class="sxs-lookup"><span data-stu-id="1d21d-139">Response</span></span>
<span data-ttu-id="1d21d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1d21d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








