---
title: 获取 deviceEnrollmentConfiguration
description: 读取 deviceEnrollmentConfiguration 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 13e9b85868598e72788b29f93f5a104059392ec8
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537027"
---
# <a name="get-deviceenrollmentconfiguration"></a><span data-ttu-id="35980-103">获取 deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="35980-103">Get deviceEnrollmentConfiguration</span></span>

> <span data-ttu-id="35980-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="35980-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35980-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="35980-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35980-106">读取 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="35980-106">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35980-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="35980-107">Prerequisites</span></span>
<span data-ttu-id="35980-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="35980-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35980-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="35980-110">Permission type</span></span>|<span data-ttu-id="35980-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="35980-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35980-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="35980-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="35980-113">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="35980-113">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="35980-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="35980-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="35980-115">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="35980-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="35980-116">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="35980-116">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="35980-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="35980-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35980-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="35980-118">Not supported.</span></span>|
|<span data-ttu-id="35980-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="35980-119">Application</span></span>||
| <span data-ttu-id="35980-120">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="35980-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="35980-121">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="35980-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="35980-122">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="35980-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="35980-123">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="35980-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35980-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="35980-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="35980-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="35980-125">Optional query parameters</span></span>
<span data-ttu-id="35980-126">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="35980-126">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35980-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="35980-127">Request headers</span></span>
|<span data-ttu-id="35980-128">标头</span><span class="sxs-lookup"><span data-stu-id="35980-128">Header</span></span>|<span data-ttu-id="35980-129">值</span><span class="sxs-lookup"><span data-stu-id="35980-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35980-130">授权</span><span class="sxs-lookup"><span data-stu-id="35980-130">Authorization</span></span>|<span data-ttu-id="35980-131">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="35980-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35980-132">接受</span><span class="sxs-lookup"><span data-stu-id="35980-132">Accept</span></span>|<span data-ttu-id="35980-133">application/json</span><span class="sxs-lookup"><span data-stu-id="35980-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35980-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="35980-134">Request body</span></span>
<span data-ttu-id="35980-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="35980-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35980-136">响应</span><span class="sxs-lookup"><span data-stu-id="35980-136">Response</span></span>
<span data-ttu-id="35980-137">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="35980-137">If successful, this method returns a `200 OK` response code and [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35980-138">示例</span><span class="sxs-lookup"><span data-stu-id="35980-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="35980-139">请求</span><span class="sxs-lookup"><span data-stu-id="35980-139">Request</span></span>
<span data-ttu-id="35980-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="35980-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="35980-141">响应</span><span class="sxs-lookup"><span data-stu-id="35980-141">Response</span></span>
<span data-ttu-id="35980-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="35980-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 392

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
    "id": "df13d8b9-d8b9-df13-b9d8-13dfb9d813df",
    "displayName": "Display Name value",
    "description": "Description value",
    "priority": 8,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "version": 7
  }
}
```






