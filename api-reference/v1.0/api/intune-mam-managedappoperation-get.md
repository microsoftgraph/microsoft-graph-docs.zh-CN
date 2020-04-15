---
title: 获取 managedAppOperation
description: 读取 managedAppOperation 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f49f37b29197603c521fce03d1286c48397aeb4b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43399078"
---
# <a name="get-managedappoperation"></a><span data-ttu-id="10894-103">获取 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="10894-103">Get managedAppOperation</span></span>

<span data-ttu-id="10894-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10894-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10894-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="10894-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10894-106">读取 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="10894-106">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10894-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="10894-107">Prerequisites</span></span>
<span data-ttu-id="10894-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="10894-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10894-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="10894-110">Permission type</span></span>|<span data-ttu-id="10894-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="10894-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10894-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10894-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10894-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="10894-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="10894-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10894-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10894-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="10894-115">Not supported.</span></span>|
|<span data-ttu-id="10894-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="10894-116">Application</span></span>|<span data-ttu-id="10894-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="10894-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10894-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10894-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10894-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="10894-119">Optional query parameters</span></span>
<span data-ttu-id="10894-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="10894-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10894-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="10894-121">Request headers</span></span>
|<span data-ttu-id="10894-122">标头</span><span class="sxs-lookup"><span data-stu-id="10894-122">Header</span></span>|<span data-ttu-id="10894-123">值</span><span class="sxs-lookup"><span data-stu-id="10894-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10894-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="10894-124">Authorization</span></span>|<span data-ttu-id="10894-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="10894-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10894-126">接受</span><span class="sxs-lookup"><span data-stu-id="10894-126">Accept</span></span>|<span data-ttu-id="10894-127">application/json</span><span class="sxs-lookup"><span data-stu-id="10894-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10894-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="10894-128">Request body</span></span>
<span data-ttu-id="10894-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="10894-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10894-130">响应</span><span class="sxs-lookup"><span data-stu-id="10894-130">Response</span></span>
<span data-ttu-id="10894-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="10894-131">If successful, this method returns a `200 OK` response code and [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10894-132">示例</span><span class="sxs-lookup"><span data-stu-id="10894-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="10894-133">请求</span><span class="sxs-lookup"><span data-stu-id="10894-133">Request</span></span>
<span data-ttu-id="10894-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="10894-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

### <a name="response"></a><span data-ttu-id="10894-135">响应</span><span class="sxs-lookup"><span data-stu-id="10894-135">Response</span></span>
<span data-ttu-id="10894-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="10894-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






