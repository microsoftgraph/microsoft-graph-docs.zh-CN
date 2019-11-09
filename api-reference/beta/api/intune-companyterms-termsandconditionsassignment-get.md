---
title: 获取 termsAndConditionsAssignment
description: 读取 termsAndConditionsAssignment 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e9166dfe1243f5e262771407fbc620b706e55344
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085062"
---
# <a name="get-termsandconditionsassignment"></a><span data-ttu-id="4acbb-103">获取 termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="4acbb-103">Get termsAndConditionsAssignment</span></span>

> <span data-ttu-id="4acbb-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4acbb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4acbb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4acbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4acbb-106">读取 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4acbb-106">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4acbb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4acbb-107">Prerequisites</span></span>
<span data-ttu-id="4acbb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4acbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4acbb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4acbb-110">Permission type</span></span>|<span data-ttu-id="4acbb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4acbb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4acbb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4acbb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4acbb-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4acbb-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="4acbb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4acbb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4acbb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4acbb-115">Not supported.</span></span>|
|<span data-ttu-id="4acbb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4acbb-116">Application</span></span>|<span data-ttu-id="4acbb-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4acbb-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4acbb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4acbb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4acbb-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4acbb-119">Optional query parameters</span></span>
<span data-ttu-id="4acbb-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4acbb-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4acbb-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4acbb-121">Request headers</span></span>
|<span data-ttu-id="4acbb-122">标头</span><span class="sxs-lookup"><span data-stu-id="4acbb-122">Header</span></span>|<span data-ttu-id="4acbb-123">值</span><span class="sxs-lookup"><span data-stu-id="4acbb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4acbb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4acbb-124">Authorization</span></span>|<span data-ttu-id="4acbb-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4acbb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4acbb-126">接受</span><span class="sxs-lookup"><span data-stu-id="4acbb-126">Accept</span></span>|<span data-ttu-id="4acbb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4acbb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4acbb-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4acbb-128">Request body</span></span>
<span data-ttu-id="4acbb-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4acbb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4acbb-130">响应</span><span class="sxs-lookup"><span data-stu-id="4acbb-130">Response</span></span>
<span data-ttu-id="4acbb-131">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4acbb-131">If successful, this method returns a `200 OK` response code and [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4acbb-132">示例</span><span class="sxs-lookup"><span data-stu-id="4acbb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4acbb-133">请求</span><span class="sxs-lookup"><span data-stu-id="4acbb-133">Request</span></span>
<span data-ttu-id="4acbb-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4acbb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

### <a name="response"></a><span data-ttu-id="4acbb-135">响应</span><span class="sxs-lookup"><span data-stu-id="4acbb-135">Response</span></span>
<span data-ttu-id="4acbb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4acbb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 246

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
    "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```






