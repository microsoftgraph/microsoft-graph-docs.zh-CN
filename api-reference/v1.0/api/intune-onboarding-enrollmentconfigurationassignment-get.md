---
title: 获取 enrollmentConfigurationAssignment
description: 读取 enrollmentConfigurationAssignment 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f79c814635505c1ebeb4498f7c6c15ef11a778f2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854920"
---
# <a name="get-enrollmentconfigurationassignment"></a><span data-ttu-id="687be-103">获取 enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="687be-103">Get enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="687be-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="687be-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="687be-105">读取 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="687be-105">Read properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="687be-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="687be-106">Prerequisites</span></span>
<span data-ttu-id="687be-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="687be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="687be-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="687be-109">Permission type</span></span>|<span data-ttu-id="687be-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="687be-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="687be-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="687be-111">Delegated (work or school account)</span></span>|<span data-ttu-id="687be-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="687be-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="687be-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="687be-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="687be-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="687be-114">Not supported.</span></span>|
|<span data-ttu-id="687be-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="687be-115">Application</span></span>|<span data-ttu-id="687be-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="687be-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="687be-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="687be-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="687be-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="687be-118">Optional query parameters</span></span>
<span data-ttu-id="687be-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="687be-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="687be-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="687be-120">Request headers</span></span>
|<span data-ttu-id="687be-121">标头</span><span class="sxs-lookup"><span data-stu-id="687be-121">Header</span></span>|<span data-ttu-id="687be-122">值</span><span class="sxs-lookup"><span data-stu-id="687be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="687be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="687be-123">Authorization</span></span>|<span data-ttu-id="687be-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="687be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="687be-125">Accept</span><span class="sxs-lookup"><span data-stu-id="687be-125">Accept</span></span>|<span data-ttu-id="687be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="687be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="687be-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="687be-127">Request body</span></span>
<span data-ttu-id="687be-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="687be-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="687be-129">响应</span><span class="sxs-lookup"><span data-stu-id="687be-129">Response</span></span>
<span data-ttu-id="687be-130">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="687be-130">If successful, this method returns a `200 OK` response code and [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="687be-131">示例</span><span class="sxs-lookup"><span data-stu-id="687be-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="687be-132">请求</span><span class="sxs-lookup"><span data-stu-id="687be-132">Request</span></span>
<span data-ttu-id="687be-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="687be-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="687be-134">响应</span><span class="sxs-lookup"><span data-stu-id="687be-134">Response</span></span>
<span data-ttu-id="687be-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="687be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "value": {
    "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
    "id": "705b021c-021c-705b-1c02-5b701c025b70",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```



