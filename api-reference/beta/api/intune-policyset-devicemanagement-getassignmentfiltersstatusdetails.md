---
title: getAssignmentFiltersStatusDetails 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2538cc410dbe3b80ea1b2e26c5fe3c4c9bedafca
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148671"
---
# <a name="getassignmentfiltersstatusdetails-action"></a><span data-ttu-id="df7c6-103">getAssignmentFiltersStatusDetails 操作</span><span class="sxs-lookup"><span data-stu-id="df7c6-103">getAssignmentFiltersStatusDetails action</span></span>

<span data-ttu-id="df7c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df7c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df7c6-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="df7c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df7c6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df7c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df7c6-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="df7c6-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df7c6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="df7c6-108">Prerequisites</span></span>
<span data-ttu-id="df7c6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df7c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df7c6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="df7c6-111">Permission type</span></span>|<span data-ttu-id="df7c6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="df7c6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df7c6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df7c6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df7c6-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df7c6-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="df7c6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df7c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df7c6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="df7c6-116">Not supported.</span></span>|
|<span data-ttu-id="df7c6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="df7c6-117">Application</span></span>|<span data-ttu-id="df7c6-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df7c6-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df7c6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df7c6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/getAssignmentFiltersStatusDetails
```

## <a name="request-headers"></a><span data-ttu-id="df7c6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="df7c6-120">Request headers</span></span>
|<span data-ttu-id="df7c6-121">标头</span><span class="sxs-lookup"><span data-stu-id="df7c6-121">Header</span></span>|<span data-ttu-id="df7c6-122">值</span><span class="sxs-lookup"><span data-stu-id="df7c6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df7c6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df7c6-123">Authorization</span></span>|<span data-ttu-id="df7c6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="df7c6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df7c6-125">接受</span><span class="sxs-lookup"><span data-stu-id="df7c6-125">Accept</span></span>|<span data-ttu-id="df7c6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df7c6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df7c6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="df7c6-127">Request body</span></span>
<span data-ttu-id="df7c6-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df7c6-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="df7c6-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="df7c6-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="df7c6-130">属性</span><span class="sxs-lookup"><span data-stu-id="df7c6-130">Property</span></span>|<span data-ttu-id="df7c6-131">类型</span><span class="sxs-lookup"><span data-stu-id="df7c6-131">Type</span></span>|<span data-ttu-id="df7c6-132">说明</span><span class="sxs-lookup"><span data-stu-id="df7c6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df7c6-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="df7c6-133">managedDeviceId</span></span>|<span data-ttu-id="df7c6-134">String</span><span class="sxs-lookup"><span data-stu-id="df7c6-134">String</span></span>|<span data-ttu-id="df7c6-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="df7c6-135">Not yet documented</span></span>|
|<span data-ttu-id="df7c6-136">payloadId</span><span class="sxs-lookup"><span data-stu-id="df7c6-136">payloadId</span></span>|<span data-ttu-id="df7c6-137">String</span><span class="sxs-lookup"><span data-stu-id="df7c6-137">String</span></span>|<span data-ttu-id="df7c6-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="df7c6-138">Not yet documented</span></span>|
|<span data-ttu-id="df7c6-139">userId</span><span class="sxs-lookup"><span data-stu-id="df7c6-139">userId</span></span>|<span data-ttu-id="df7c6-140">String</span><span class="sxs-lookup"><span data-stu-id="df7c6-140">String</span></span>|<span data-ttu-id="df7c6-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="df7c6-141">Not yet documented</span></span>|
|<span data-ttu-id="df7c6-142">assignmentFilterIds</span><span class="sxs-lookup"><span data-stu-id="df7c6-142">assignmentFilterIds</span></span>|<span data-ttu-id="df7c6-143">String collection</span><span class="sxs-lookup"><span data-stu-id="df7c6-143">String collection</span></span>|<span data-ttu-id="df7c6-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="df7c6-144">Not yet documented</span></span>|
|<span data-ttu-id="df7c6-145">top</span><span class="sxs-lookup"><span data-stu-id="df7c6-145">top</span></span>|<span data-ttu-id="df7c6-146">Int32</span><span class="sxs-lookup"><span data-stu-id="df7c6-146">Int32</span></span>|<span data-ttu-id="df7c6-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="df7c6-147">Not yet documented</span></span>|
|<span data-ttu-id="df7c6-148">skip</span><span class="sxs-lookup"><span data-stu-id="df7c6-148">skip</span></span>|<span data-ttu-id="df7c6-149">Int32</span><span class="sxs-lookup"><span data-stu-id="df7c6-149">Int32</span></span>|<span data-ttu-id="df7c6-150">尚未记录</span><span class="sxs-lookup"><span data-stu-id="df7c6-150">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="df7c6-151">响应</span><span class="sxs-lookup"><span data-stu-id="df7c6-151">Response</span></span>
<span data-ttu-id="df7c6-152">如果成功，此操作在响应正文中返回 响应代码和 `200 OK` [assignmentFilterStatusDetails。](../resources/intune-policyset-assignmentfilterstatusdetails.md)</span><span class="sxs-lookup"><span data-stu-id="df7c6-152">If successful, this action returns a `200 OK` response code and a [assignmentFilterStatusDetails](../resources/intune-policyset-assignmentfilterstatusdetails.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df7c6-153">示例</span><span class="sxs-lookup"><span data-stu-id="df7c6-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="df7c6-154">请求</span><span class="sxs-lookup"><span data-stu-id="df7c6-154">Request</span></span>
<span data-ttu-id="df7c6-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df7c6-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/getAssignmentFiltersStatusDetails

Content-type: application/json
Content-length: 214

{
  "managedDeviceId": "Managed Device Id value",
  "payloadId": "Payload Id value",
  "userId": "User Id value",
  "assignmentFilterIds": [
    "Assignment Filter Ids value"
  ],
  "top": 3,
  "skip": 4
}
```

### <a name="response"></a><span data-ttu-id="df7c6-156">响应</span><span class="sxs-lookup"><span data-stu-id="df7c6-156">Response</span></span>
<span data-ttu-id="df7c6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="df7c6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1216

{
  "value": {
    "@odata.type": "microsoft.graph.assignmentFilterStatusDetails",
    "managedDeviceId": "Managed Device Id value",
    "payloadId": "Payload Id value",
    "userId": "User Id value",
    "deviceProperties": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "evalutionSummaries": [
      {
        "@odata.type": "microsoft.graph.assignmentFilterEvaluationSummary",
        "assignmentFilterId": "Assignment Filter Id value",
        "assignmentFilterLastModifiedDateTime": "2017-01-01T00:02:50.0900701-08:00",
        "assignmentFilterDisplayName": "Assignment Filter Display Name value",
        "assignmentFilterPlatform": "androidForWork",
        "evaluationResult": "match",
        "evaluationDateTime": "2016-12-31T23:58:01.2047675-08:00",
        "assignmentFilterType": "include",
        "assignmentFilterTypeAndEvaluationResults": [
          {
            "@odata.type": "microsoft.graph.assignmentFilterTypeAndEvaluationResult",
            "assignmentFilterType": "include",
            "evaluationResult": "match"
          }
        ]
      }
    ]
  }
}
```




