---
title: 列出 managedAppStatusRaws
description: 列出 managedAppStatusRaw 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cdbb95f771c28ec9723362e823537b2f2f34f005
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254714"
---
# <a name="list-managedappstatusraws"></a><span data-ttu-id="6dcff-103">列出 managedAppStatusRaws</span><span class="sxs-lookup"><span data-stu-id="6dcff-103">List managedAppStatusRaws</span></span>

> <span data-ttu-id="6dcff-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6dcff-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dcff-105">列出 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6dcff-105">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6dcff-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="6dcff-106">Prerequisites</span></span>
<span data-ttu-id="6dcff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6dcff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6dcff-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6dcff-109">Permission type</span></span>|<span data-ttu-id="6dcff-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6dcff-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dcff-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6dcff-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6dcff-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6dcff-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6dcff-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6dcff-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dcff-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6dcff-114">Not supported.</span></span>|
|<span data-ttu-id="6dcff-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6dcff-115">Application</span></span>|<span data-ttu-id="6dcff-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6dcff-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dcff-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6dcff-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="6dcff-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6dcff-118">Request headers</span></span>
|<span data-ttu-id="6dcff-119">标头</span><span class="sxs-lookup"><span data-stu-id="6dcff-119">Header</span></span>|<span data-ttu-id="6dcff-120">值</span><span class="sxs-lookup"><span data-stu-id="6dcff-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6dcff-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dcff-121">Authorization</span></span>|<span data-ttu-id="6dcff-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6dcff-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6dcff-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6dcff-123">Accept</span></span>|<span data-ttu-id="6dcff-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6dcff-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dcff-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6dcff-125">Request body</span></span>
<span data-ttu-id="6dcff-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6dcff-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dcff-127">响应</span><span class="sxs-lookup"><span data-stu-id="6dcff-127">Response</span></span>
<span data-ttu-id="6dcff-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6dcff-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dcff-129">示例</span><span class="sxs-lookup"><span data-stu-id="6dcff-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="6dcff-130">请求</span><span class="sxs-lookup"><span data-stu-id="6dcff-130">Request</span></span>
<span data-ttu-id="6dcff-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6dcff-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses
```

### <a name="response"></a><span data-ttu-id="6dcff-132">响应</span><span class="sxs-lookup"><span data-stu-id="6dcff-132">Response</span></span>
<span data-ttu-id="6dcff-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6dcff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 307

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppStatusRaw",
      "displayName": "Display Name value",
      "id": "80847581-7581-8084-8175-848081758480",
      "version": "Version value",
      "content": {
        "@odata.type": "microsoft.graph.Json"
      }
    }
  ]
}
```



