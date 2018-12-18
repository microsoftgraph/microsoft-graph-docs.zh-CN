---
title: 列出 deviceInstallStates
description: 列出 deviceInstallState 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: 94c4039e2605ab6139623cfac50343aac5b0b925
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350783"
---
# <a name="list-deviceinstallstates"></a><span data-ttu-id="d941e-103">列出 deviceInstallStates</span><span class="sxs-lookup"><span data-stu-id="d941e-103">List deviceInstallStates</span></span>

> <span data-ttu-id="d941e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d941e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d941e-105">列出 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d941e-105">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d941e-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="d941e-106">Prerequisites</span></span>
<span data-ttu-id="d941e-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d941e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d941e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d941e-109">Permission type</span></span>|<span data-ttu-id="d941e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d941e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d941e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d941e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d941e-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d941e-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d941e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d941e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d941e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d941e-114">Not supported.</span></span>|
|<span data-ttu-id="d941e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d941e-115">Application</span></span>|<span data-ttu-id="d941e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d941e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d941e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d941e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="d941e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d941e-118">Request headers</span></span>
|<span data-ttu-id="d941e-119">标头</span><span class="sxs-lookup"><span data-stu-id="d941e-119">Header</span></span>|<span data-ttu-id="d941e-120">值</span><span class="sxs-lookup"><span data-stu-id="d941e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d941e-121">授权</span><span class="sxs-lookup"><span data-stu-id="d941e-121">Authorization</span></span>|<span data-ttu-id="d941e-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d941e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d941e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d941e-123">Accept</span></span>|<span data-ttu-id="d941e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d941e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d941e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d941e-125">Request body</span></span>
<span data-ttu-id="d941e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d941e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d941e-127">响应</span><span class="sxs-lookup"><span data-stu-id="d941e-127">Response</span></span>
<span data-ttu-id="d941e-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceInstallState](../resources/intune-books-deviceinstallstate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d941e-128">If successful, this method returns a `200 OK` response code and a collection of [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d941e-129">示例</span><span class="sxs-lookup"><span data-stu-id="d941e-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d941e-130">请求</span><span class="sxs-lookup"><span data-stu-id="d941e-130">Request</span></span>
<span data-ttu-id="d941e-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d941e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="d941e-132">响应</span><span class="sxs-lookup"><span data-stu-id="d941e-132">Response</span></span>
<span data-ttu-id="d941e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d941e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



