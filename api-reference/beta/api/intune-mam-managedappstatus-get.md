---
title: 获取 managedAppStatus
description: 读取 managedAppStatus 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3fc7f984f5b1d62839472d06a9f4d2da6a99ce77
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37193057"
---
# <a name="get-managedappstatus"></a><span data-ttu-id="1e761-103">获取 managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="1e761-103">Get managedAppStatus</span></span>

> <span data-ttu-id="1e761-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1e761-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e761-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1e761-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e761-106">读取 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1e761-106">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e761-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1e761-107">Prerequisites</span></span>
<span data-ttu-id="1e761-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e761-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e761-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e761-110">Permission type</span></span>|<span data-ttu-id="1e761-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1e761-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e761-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e761-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e761-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e761-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1e761-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e761-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e761-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e761-115">Not supported.</span></span>|
|<span data-ttu-id="1e761-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e761-116">Application</span></span>|<span data-ttu-id="1e761-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e761-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e761-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e761-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1e761-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1e761-119">Optional query parameters</span></span>
<span data-ttu-id="1e761-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1e761-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e761-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e761-121">Request headers</span></span>
|<span data-ttu-id="1e761-122">标头</span><span class="sxs-lookup"><span data-stu-id="1e761-122">Header</span></span>|<span data-ttu-id="1e761-123">值</span><span class="sxs-lookup"><span data-stu-id="1e761-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e761-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e761-124">Authorization</span></span>|<span data-ttu-id="1e761-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1e761-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e761-126">接受</span><span class="sxs-lookup"><span data-stu-id="1e761-126">Accept</span></span>|<span data-ttu-id="1e761-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1e761-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e761-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e761-128">Request body</span></span>
<span data-ttu-id="1e761-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1e761-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e761-130">响应</span><span class="sxs-lookup"><span data-stu-id="1e761-130">Response</span></span>
<span data-ttu-id="1e761-131">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1e761-131">If successful, this method returns a `200 OK` response code and [managedAppStatus](../resources/intune-mam-managedappstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e761-132">示例</span><span class="sxs-lookup"><span data-stu-id="1e761-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e761-133">请求</span><span class="sxs-lookup"><span data-stu-id="1e761-133">Request</span></span>
<span data-ttu-id="1e761-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e761-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

### <a name="response"></a><span data-ttu-id="1e761-135">响应</span><span class="sxs-lookup"><span data-stu-id="1e761-135">Response</span></span>
<span data-ttu-id="1e761-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1e761-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 205

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppStatus",
    "displayName": "Display Name value",
    "id": "ad1f7541-7541-ad1f-4175-1fad41751fad",
    "version": "Version value"
  }
}
```




