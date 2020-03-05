---
title: 列出 deviceInstallStates
description: 列出 deviceInstallState 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 51d385c6b96959b6cf963b4627d6ff965188dc76
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450382"
---
# <a name="list-deviceinstallstates"></a><span data-ttu-id="24486-103">列出 deviceInstallStates</span><span class="sxs-lookup"><span data-stu-id="24486-103">List deviceInstallStates</span></span>

<span data-ttu-id="24486-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="24486-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24486-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="24486-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24486-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="24486-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24486-107">列出 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="24486-107">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24486-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="24486-108">Prerequisites</span></span>
<span data-ttu-id="24486-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24486-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24486-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="24486-111">Permission type</span></span>|<span data-ttu-id="24486-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="24486-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24486-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24486-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24486-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="24486-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="24486-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24486-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24486-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="24486-116">Not supported.</span></span>|
|<span data-ttu-id="24486-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="24486-117">Application</span></span>|<span data-ttu-id="24486-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="24486-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24486-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24486-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="24486-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="24486-120">Request headers</span></span>
|<span data-ttu-id="24486-121">标头</span><span class="sxs-lookup"><span data-stu-id="24486-121">Header</span></span>|<span data-ttu-id="24486-122">值</span><span class="sxs-lookup"><span data-stu-id="24486-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24486-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="24486-123">Authorization</span></span>|<span data-ttu-id="24486-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="24486-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24486-125">接受</span><span class="sxs-lookup"><span data-stu-id="24486-125">Accept</span></span>|<span data-ttu-id="24486-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24486-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24486-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="24486-127">Request body</span></span>
<span data-ttu-id="24486-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="24486-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24486-129">响应</span><span class="sxs-lookup"><span data-stu-id="24486-129">Response</span></span>
<span data-ttu-id="24486-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="24486-130">If successful, this method returns a `200 OK` response code and a collection of [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24486-131">示例</span><span class="sxs-lookup"><span data-stu-id="24486-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="24486-132">请求</span><span class="sxs-lookup"><span data-stu-id="24486-132">Request</span></span>
<span data-ttu-id="24486-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="24486-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="24486-134">响应</span><span class="sxs-lookup"><span data-stu-id="24486-134">Response</span></span>
<span data-ttu-id="24486-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="24486-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 496

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceInstallState",
      "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
      "deviceName": "Device Name value",
      "deviceId": "Device Id value",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "installState": "installed",
      "errorCode": "Error Code value",
      "osVersion": "Os Version value",
      "osDescription": "Os Description value",
      "userName": "User Name value"
    }
  ]
}
```





