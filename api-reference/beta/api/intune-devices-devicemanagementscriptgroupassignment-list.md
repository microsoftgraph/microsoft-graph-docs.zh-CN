---
title: 列出 deviceManagementScriptGroupAssignments
description: 列出 deviceManagementScriptGroupAssignment 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 44cd62b0a0c4a2e7fb9f032679c615336b09489d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173932"
---
# <a name="list-devicemanagementscriptgroupassignments"></a><span data-ttu-id="3cb40-103">列出 deviceManagementScriptGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="3cb40-103">List deviceManagementScriptGroupAssignments</span></span>

> <span data-ttu-id="3cb40-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3cb40-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3cb40-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3cb40-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cb40-106">列出[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3cb40-106">List properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3cb40-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3cb40-107">Prerequisites</span></span>
<span data-ttu-id="3cb40-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3cb40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3cb40-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3cb40-110">Permission type</span></span>|<span data-ttu-id="3cb40-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3cb40-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cb40-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3cb40-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3cb40-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="3cb40-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="3cb40-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3cb40-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cb40-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3cb40-115">Not supported.</span></span>|
|<span data-ttu-id="3cb40-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3cb40-116">Application</span></span>|<span data-ttu-id="3cb40-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3cb40-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cb40-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3cb40-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="3cb40-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3cb40-119">Request headers</span></span>
|<span data-ttu-id="3cb40-120">标头</span><span class="sxs-lookup"><span data-stu-id="3cb40-120">Header</span></span>|<span data-ttu-id="3cb40-121">值</span><span class="sxs-lookup"><span data-stu-id="3cb40-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3cb40-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cb40-122">Authorization</span></span>|<span data-ttu-id="3cb40-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3cb40-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3cb40-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3cb40-124">Accept</span></span>|<span data-ttu-id="3cb40-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3cb40-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cb40-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3cb40-126">Request body</span></span>
<span data-ttu-id="3cb40-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3cb40-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cb40-128">响应</span><span class="sxs-lookup"><span data-stu-id="3cb40-128">Response</span></span>
<span data-ttu-id="3cb40-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="3cb40-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cb40-130">示例</span><span class="sxs-lookup"><span data-stu-id="3cb40-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3cb40-131">请求</span><span class="sxs-lookup"><span data-stu-id="3cb40-131">Request</span></span>
<span data-ttu-id="3cb40-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3cb40-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="3cb40-133">响应</span><span class="sxs-lookup"><span data-stu-id="3cb40-133">Response</span></span>
<span data-ttu-id="3cb40-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3cb40-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 218

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
      "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
      "targetGroupId": "Target Group Id value"
    }
  ]
}
```




