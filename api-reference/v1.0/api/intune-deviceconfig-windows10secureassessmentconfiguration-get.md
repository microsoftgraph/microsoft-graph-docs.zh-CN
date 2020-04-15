---
title: 获取 windows10SecureAssessmentConfiguration
description: 读取 windows10SecureAssessmentConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7c1487af01cf17086c2057337d28e91a0421c3dd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442062"
---
# <a name="get-windows10secureassessmentconfiguration"></a><span data-ttu-id="03410-103">获取 windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="03410-103">Get windows10SecureAssessmentConfiguration</span></span>

<span data-ttu-id="03410-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03410-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03410-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03410-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03410-106">读取 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="03410-106">Read properties and relationships of the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03410-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="03410-107">Prerequisites</span></span>
<span data-ttu-id="03410-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03410-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03410-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="03410-110">Permission type</span></span>|<span data-ttu-id="03410-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="03410-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03410-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03410-112">Delegated (work or school account)</span></span>|<span data-ttu-id="03410-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="03410-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="03410-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03410-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03410-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="03410-115">Not supported.</span></span>|
|<span data-ttu-id="03410-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="03410-116">Application</span></span>|<span data-ttu-id="03410-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="03410-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03410-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03410-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="03410-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="03410-119">Optional query parameters</span></span>
<span data-ttu-id="03410-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="03410-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03410-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="03410-121">Request headers</span></span>
|<span data-ttu-id="03410-122">标头</span><span class="sxs-lookup"><span data-stu-id="03410-122">Header</span></span>|<span data-ttu-id="03410-123">值</span><span class="sxs-lookup"><span data-stu-id="03410-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03410-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="03410-124">Authorization</span></span>|<span data-ttu-id="03410-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="03410-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03410-126">接受</span><span class="sxs-lookup"><span data-stu-id="03410-126">Accept</span></span>|<span data-ttu-id="03410-127">application/json</span><span class="sxs-lookup"><span data-stu-id="03410-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03410-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="03410-128">Request body</span></span>
<span data-ttu-id="03410-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="03410-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03410-130">响应</span><span class="sxs-lookup"><span data-stu-id="03410-130">Response</span></span>
<span data-ttu-id="03410-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="03410-131">If successful, this method returns a `200 OK` response code and [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03410-132">示例</span><span class="sxs-lookup"><span data-stu-id="03410-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="03410-133">请求</span><span class="sxs-lookup"><span data-stu-id="03410-133">Request</span></span>
<span data-ttu-id="03410-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03410-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="03410-135">响应</span><span class="sxs-lookup"><span data-stu-id="03410-135">Response</span></span>
<span data-ttu-id="03410-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="03410-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 574

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
    "id": "f60d71be-71be-f60d-be71-0df6be710df6",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "launchUri": "Launch Uri value",
    "configurationAccount": "Configuration Account value",
    "allowPrinting": true,
    "allowScreenCapture": true,
    "allowTextSuggestion": true
  }
}
```






