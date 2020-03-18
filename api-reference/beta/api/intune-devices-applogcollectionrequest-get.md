---
title: 获取 appLogCollectionRequest
description: 读取 appLogCollectionRequest 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2bc3331dfeca08af705645f1685b7125d04614a7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42763989"
---
# <a name="get-applogcollectionrequest"></a><span data-ttu-id="a217e-103">获取 appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="a217e-103">Get appLogCollectionRequest</span></span>

> <span data-ttu-id="a217e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a217e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a217e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a217e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a217e-106">读取[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a217e-106">Read properties and relationships of the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a217e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a217e-107">Prerequisites</span></span>
<span data-ttu-id="a217e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a217e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a217e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a217e-110">Permission type</span></span>|<span data-ttu-id="a217e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a217e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a217e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a217e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a217e-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a217e-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a217e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a217e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a217e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a217e-115">Not supported.</span></span>|
|<span data-ttu-id="a217e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a217e-116">Application</span></span>|<span data-ttu-id="a217e-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a217e-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a217e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a217e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a217e-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a217e-119">Optional query parameters</span></span>
<span data-ttu-id="a217e-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a217e-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a217e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a217e-121">Request headers</span></span>
|<span data-ttu-id="a217e-122">标头</span><span class="sxs-lookup"><span data-stu-id="a217e-122">Header</span></span>|<span data-ttu-id="a217e-123">值</span><span class="sxs-lookup"><span data-stu-id="a217e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a217e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a217e-124">Authorization</span></span>|<span data-ttu-id="a217e-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a217e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a217e-126">接受</span><span class="sxs-lookup"><span data-stu-id="a217e-126">Accept</span></span>|<span data-ttu-id="a217e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a217e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a217e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a217e-128">Request body</span></span>
<span data-ttu-id="a217e-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a217e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a217e-130">响应</span><span class="sxs-lookup"><span data-stu-id="a217e-130">Response</span></span>
<span data-ttu-id="a217e-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a217e-131">If successful, this method returns a `200 OK` response code and [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a217e-132">示例</span><span class="sxs-lookup"><span data-stu-id="a217e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a217e-133">请求</span><span class="sxs-lookup"><span data-stu-id="a217e-133">Request</span></span>
<span data-ttu-id="a217e-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a217e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

### <a name="response"></a><span data-ttu-id="a217e-135">响应</span><span class="sxs-lookup"><span data-stu-id="a217e-135">Response</span></span>
<span data-ttu-id="a217e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a217e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 341

{
  "value": {
    "@odata.type": "#microsoft.graph.appLogCollectionRequest",
    "id": "cca685ff-85ff-cca6-ff85-a6ccff85a6cc",
    "status": "completed",
    "errorMessage": "Error Message value",
    "customLogFolders": [
      "Custom Log Folders value"
    ],
    "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
  }
}
```




