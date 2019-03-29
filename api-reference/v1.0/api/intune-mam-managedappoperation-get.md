---
title: 获取 managedAppOperation
description: 读取 managedAppOperation 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cda432dcaaf5ede81f692eee6c4425299e95bb13
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969300"
---
# <a name="get-managedappoperation"></a><span data-ttu-id="581c7-103">获取 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="581c7-103">Get managedAppOperation</span></span>

> <span data-ttu-id="581c7-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="581c7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="581c7-105">读取 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="581c7-105">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="581c7-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="581c7-106">Prerequisites</span></span>
<span data-ttu-id="581c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="581c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="581c7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="581c7-109">Permission type</span></span>|<span data-ttu-id="581c7-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="581c7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="581c7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="581c7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="581c7-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="581c7-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="581c7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="581c7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="581c7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="581c7-114">Not supported.</span></span>|
|<span data-ttu-id="581c7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="581c7-115">Application</span></span>|<span data-ttu-id="581c7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="581c7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="581c7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="581c7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="581c7-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="581c7-118">Optional query parameters</span></span>
<span data-ttu-id="581c7-119">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="581c7-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="581c7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="581c7-120">Request headers</span></span>
|<span data-ttu-id="581c7-121">标头</span><span class="sxs-lookup"><span data-stu-id="581c7-121">Header</span></span>|<span data-ttu-id="581c7-122">值</span><span class="sxs-lookup"><span data-stu-id="581c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="581c7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="581c7-123">Authorization</span></span>|<span data-ttu-id="581c7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="581c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="581c7-125">接受</span><span class="sxs-lookup"><span data-stu-id="581c7-125">Accept</span></span>|<span data-ttu-id="581c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="581c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="581c7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="581c7-127">Request body</span></span>
<span data-ttu-id="581c7-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="581c7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="581c7-129">响应</span><span class="sxs-lookup"><span data-stu-id="581c7-129">Response</span></span>
<span data-ttu-id="581c7-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="581c7-130">If successful, this method returns a `200 OK` response code and [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="581c7-131">示例</span><span class="sxs-lookup"><span data-stu-id="581c7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="581c7-132">请求</span><span class="sxs-lookup"><span data-stu-id="581c7-132">Request</span></span>
<span data-ttu-id="581c7-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="581c7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

### <a name="response"></a><span data-ttu-id="581c7-134">响应</span><span class="sxs-lookup"><span data-stu-id="581c7-134">Response</span></span>
<span data-ttu-id="581c7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="581c7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 303

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppOperation",
    "displayName": "Display Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "state": "State value",
    "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
    "version": "Version value"
  }
}
```



