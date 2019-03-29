---
title: 获取 deviceManagementScriptGroupAssignment
description: 读取 deviceManagementScriptGroupAssignment 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76496e2e861e00a559a090985eef88530a03142f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958254"
---
# <a name="get-devicemanagementscriptgroupassignment"></a><span data-ttu-id="9c44e-103">获取 deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="9c44e-103">Get deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="9c44e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9c44e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c44e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c44e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c44e-106">读取[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9c44e-106">Read properties and relationships of the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c44e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9c44e-107">Prerequisites</span></span>
<span data-ttu-id="9c44e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c44e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c44e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c44e-110">Permission type</span></span>|<span data-ttu-id="9c44e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9c44e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c44e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c44e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9c44e-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c44e-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9c44e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c44e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c44e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c44e-115">Not supported.</span></span>|
|<span data-ttu-id="9c44e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c44e-116">Application</span></span>|<span data-ttu-id="9c44e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c44e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c44e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c44e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9c44e-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9c44e-119">Optional query parameters</span></span>
<span data-ttu-id="9c44e-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9c44e-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c44e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c44e-121">Request headers</span></span>
|<span data-ttu-id="9c44e-122">标头</span><span class="sxs-lookup"><span data-stu-id="9c44e-122">Header</span></span>|<span data-ttu-id="9c44e-123">值</span><span class="sxs-lookup"><span data-stu-id="9c44e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c44e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c44e-124">Authorization</span></span>|<span data-ttu-id="9c44e-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9c44e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c44e-126">接受</span><span class="sxs-lookup"><span data-stu-id="9c44e-126">Accept</span></span>|<span data-ttu-id="9c44e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9c44e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c44e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c44e-128">Request body</span></span>
<span data-ttu-id="9c44e-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9c44e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c44e-130">响应</span><span class="sxs-lookup"><span data-stu-id="9c44e-130">Response</span></span>
<span data-ttu-id="9c44e-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9c44e-131">If successful, this method returns a `200 OK` response code and [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c44e-132">示例</span><span class="sxs-lookup"><span data-stu-id="9c44e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c44e-133">请求</span><span class="sxs-lookup"><span data-stu-id="9c44e-133">Request</span></span>
<span data-ttu-id="9c44e-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9c44e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="9c44e-135">响应</span><span class="sxs-lookup"><span data-stu-id="9c44e-135">Response</span></span>
<span data-ttu-id="9c44e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9c44e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 198

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
    "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
    "targetGroupId": "Target Group Id value"
  }
}
```




