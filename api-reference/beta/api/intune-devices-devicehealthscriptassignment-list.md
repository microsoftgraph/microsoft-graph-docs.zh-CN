---
title: 列出 deviceHealthScriptAssignments
description: 列出 deviceHealthScriptAssignment 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 976ba0fef00456f3ebc2524ac68ac4f6aeddf4b6
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087578"
---
# <a name="list-devicehealthscriptassignments"></a><span data-ttu-id="ca8eb-103">列出 deviceHealthScriptAssignments</span><span class="sxs-lookup"><span data-stu-id="ca8eb-103">List deviceHealthScriptAssignments</span></span>

> <span data-ttu-id="ca8eb-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ca8eb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca8eb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca8eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca8eb-106">列出[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ca8eb-106">List properties and relationships of the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca8eb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ca8eb-107">Prerequisites</span></span>
<span data-ttu-id="ca8eb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca8eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca8eb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca8eb-110">Permission type</span></span>|<span data-ttu-id="ca8eb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ca8eb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca8eb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca8eb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca8eb-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca8eb-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ca8eb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca8eb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca8eb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca8eb-115">Not supported.</span></span>|
|<span data-ttu-id="ca8eb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca8eb-116">Application</span></span>|<span data-ttu-id="ca8eb-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca8eb-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca8eb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca8eb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ca8eb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca8eb-119">Request headers</span></span>
|<span data-ttu-id="ca8eb-120">标头</span><span class="sxs-lookup"><span data-stu-id="ca8eb-120">Header</span></span>|<span data-ttu-id="ca8eb-121">值</span><span class="sxs-lookup"><span data-stu-id="ca8eb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca8eb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca8eb-122">Authorization</span></span>|<span data-ttu-id="ca8eb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ca8eb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca8eb-124">接受</span><span class="sxs-lookup"><span data-stu-id="ca8eb-124">Accept</span></span>|<span data-ttu-id="ca8eb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca8eb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca8eb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca8eb-126">Request body</span></span>
<span data-ttu-id="ca8eb-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ca8eb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca8eb-128">响应</span><span class="sxs-lookup"><span data-stu-id="ca8eb-128">Response</span></span>
<span data-ttu-id="ca8eb-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="ca8eb-129">If successful, this method returns a `200 OK` response code and a collection of [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca8eb-130">示例</span><span class="sxs-lookup"><span data-stu-id="ca8eb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca8eb-131">请求</span><span class="sxs-lookup"><span data-stu-id="ca8eb-131">Request</span></span>
<span data-ttu-id="ca8eb-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca8eb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
```

### <a name="response"></a><span data-ttu-id="ca8eb-133">响应</span><span class="sxs-lookup"><span data-stu-id="ca8eb-133">Response</span></span>
<span data-ttu-id="ca8eb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca8eb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 395

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
      "id": "c08c4eb1-4eb1-c08c-b14e-8cc0b14e8cc0",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "runRemediationScript": true,
      "runSchedule": {
        "@odata.type": "microsoft.graph.runSchedule"
      }
    }
  ]
}
```






