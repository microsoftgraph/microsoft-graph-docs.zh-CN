---
title: 更新 assignmentFilterEvaluationStatusDetails
description: 更新 assignmentFilterEvaluationStatusDetails 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0cd53ae8b487a89cdb47b2635f075a4558acf6b8
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160221"
---
# <a name="update-assignmentfilterevaluationstatusdetails"></a><span data-ttu-id="d27c6-103">更新 assignmentFilterEvaluationStatusDetails</span><span class="sxs-lookup"><span data-stu-id="d27c6-103">Update assignmentFilterEvaluationStatusDetails</span></span>

<span data-ttu-id="d27c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d27c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d27c6-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d27c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d27c6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d27c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d27c6-107">更新 [assignmentFilterEvaluationStatusDetails 对象](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="d27c6-107">Update the properties of a [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d27c6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d27c6-108">Prerequisites</span></span>
<span data-ttu-id="d27c6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d27c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d27c6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d27c6-111">Permission type</span></span>|<span data-ttu-id="d27c6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d27c6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d27c6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d27c6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d27c6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d27c6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d27c6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d27c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d27c6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d27c6-116">Not supported.</span></span>|
|<span data-ttu-id="d27c6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d27c6-117">Application</span></span>|<span data-ttu-id="d27c6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d27c6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d27c6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d27c6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}/assignmentFilterEvaluationStatusDetails/{assignmentFilterEvaluationStatusDetailsId}
```

## <a name="request-headers"></a><span data-ttu-id="d27c6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d27c6-120">Request headers</span></span>
|<span data-ttu-id="d27c6-121">标头</span><span class="sxs-lookup"><span data-stu-id="d27c6-121">Header</span></span>|<span data-ttu-id="d27c6-122">值</span><span class="sxs-lookup"><span data-stu-id="d27c6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d27c6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d27c6-123">Authorization</span></span>|<span data-ttu-id="d27c6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d27c6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d27c6-125">接受</span><span class="sxs-lookup"><span data-stu-id="d27c6-125">Accept</span></span>|<span data-ttu-id="d27c6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d27c6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d27c6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d27c6-127">Request body</span></span>
<span data-ttu-id="d27c6-128">在请求正文中，提供 [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d27c6-128">In the request body, supply a JSON representation for the [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) object.</span></span>

<span data-ttu-id="d27c6-129">下表显示创建 [assignmentFilterEvaluationStatusDetails 时所需的属性](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)。</span><span class="sxs-lookup"><span data-stu-id="d27c6-129">The following table shows the properties that are required when you create the [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md).</span></span>

|<span data-ttu-id="d27c6-130">属性</span><span class="sxs-lookup"><span data-stu-id="d27c6-130">Property</span></span>|<span data-ttu-id="d27c6-131">类型</span><span class="sxs-lookup"><span data-stu-id="d27c6-131">Type</span></span>|<span data-ttu-id="d27c6-132">说明</span><span class="sxs-lookup"><span data-stu-id="d27c6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d27c6-133">id</span><span class="sxs-lookup"><span data-stu-id="d27c6-133">id</span></span>|<span data-ttu-id="d27c6-134">String</span><span class="sxs-lookup"><span data-stu-id="d27c6-134">String</span></span>|<span data-ttu-id="d27c6-135">AssignmentFilterEvaluationStatusDetails 实体的键。</span><span class="sxs-lookup"><span data-stu-id="d27c6-135">Key of the AssignmentFilterEvaluationStatusDetails entity.</span></span>|
|<span data-ttu-id="d27c6-136">payloadId</span><span class="sxs-lookup"><span data-stu-id="d27c6-136">payloadId</span></span>|<span data-ttu-id="d27c6-137">String</span><span class="sxs-lookup"><span data-stu-id="d27c6-137">String</span></span>|<span data-ttu-id="d27c6-138">已应用筛选器的 PayloadId。</span><span class="sxs-lookup"><span data-stu-id="d27c6-138">PayloadId on which filter has been applied.</span></span>|



## <a name="response"></a><span data-ttu-id="d27c6-139">响应</span><span class="sxs-lookup"><span data-stu-id="d27c6-139">Response</span></span>
<span data-ttu-id="d27c6-140">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d27c6-140">If successful, this method returns a `200 OK` response code and an updated [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d27c6-141">示例</span><span class="sxs-lookup"><span data-stu-id="d27c6-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d27c6-142">请求</span><span class="sxs-lookup"><span data-stu-id="d27c6-142">Request</span></span>
<span data-ttu-id="d27c6-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d27c6-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/assignmentFilterEvaluationStatusDetails/{assignmentFilterEvaluationStatusDetailsId}
Content-type: application/json
Content-length: 117

{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationStatusDetails",
  "payloadId": "Payload Id value"
}
```

### <a name="response"></a><span data-ttu-id="d27c6-144">响应</span><span class="sxs-lookup"><span data-stu-id="d27c6-144">Response</span></span>
<span data-ttu-id="d27c6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d27c6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 166

{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationStatusDetails",
  "id": "820ef068-f068-820e-68f0-0e8268f00e82",
  "payloadId": "Payload Id value"
}
```




