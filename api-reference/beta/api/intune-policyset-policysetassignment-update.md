---
title: 更新 policySetAssignment
description: 更新 policySetAssignment 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c3d2f0f5824e45dd76b5fbda46c5e7702105390a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536292"
---
# <a name="update-policysetassignment"></a><span data-ttu-id="d81df-103">更新 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="d81df-103">Update policySetAssignment</span></span>

> <span data-ttu-id="d81df-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d81df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d81df-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d81df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d81df-106">更新[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d81df-106">Update the properties of a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d81df-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d81df-107">Prerequisites</span></span>
<span data-ttu-id="d81df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d81df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d81df-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d81df-110">Permission type</span></span>|<span data-ttu-id="d81df-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d81df-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d81df-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d81df-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d81df-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d81df-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d81df-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d81df-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d81df-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d81df-115">Not supported.</span></span>|
|<span data-ttu-id="d81df-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d81df-116">Application</span></span>|<span data-ttu-id="d81df-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d81df-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d81df-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d81df-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/assignments/{policySetAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d81df-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d81df-119">Request headers</span></span>
|<span data-ttu-id="d81df-120">标头</span><span class="sxs-lookup"><span data-stu-id="d81df-120">Header</span></span>|<span data-ttu-id="d81df-121">值</span><span class="sxs-lookup"><span data-stu-id="d81df-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d81df-122">授权</span><span class="sxs-lookup"><span data-stu-id="d81df-122">Authorization</span></span>|<span data-ttu-id="d81df-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d81df-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d81df-124">接受</span><span class="sxs-lookup"><span data-stu-id="d81df-124">Accept</span></span>|<span data-ttu-id="d81df-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d81df-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d81df-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d81df-126">Request body</span></span>
<span data-ttu-id="d81df-127">在请求正文中，提供[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d81df-127">In the request body, supply a JSON representation for the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

<span data-ttu-id="d81df-128">下表显示创建[policySetAssignment](../resources/intune-policyset-policysetassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d81df-128">The following table shows the properties that are required when you create the [policySetAssignment](../resources/intune-policyset-policysetassignment.md).</span></span>

|<span data-ttu-id="d81df-129">属性</span><span class="sxs-lookup"><span data-stu-id="d81df-129">Property</span></span>|<span data-ttu-id="d81df-130">类型</span><span class="sxs-lookup"><span data-stu-id="d81df-130">Type</span></span>|<span data-ttu-id="d81df-131">说明</span><span class="sxs-lookup"><span data-stu-id="d81df-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d81df-132">id</span><span class="sxs-lookup"><span data-stu-id="d81df-132">id</span></span>|<span data-ttu-id="d81df-133">字符串</span><span class="sxs-lookup"><span data-stu-id="d81df-133">String</span></span>|<span data-ttu-id="d81df-134">PolicySetAssignment 的键。</span><span class="sxs-lookup"><span data-stu-id="d81df-134">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="d81df-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d81df-135">lastModifiedDateTime</span></span>|<span data-ttu-id="d81df-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d81df-136">DateTimeOffset</span></span>|<span data-ttu-id="d81df-137">PolicySetAssignment 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="d81df-137">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="d81df-138">target</span><span class="sxs-lookup"><span data-stu-id="d81df-138">target</span></span>|[<span data-ttu-id="d81df-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d81df-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d81df-140">PolicySetAssignment 的目标组</span><span class="sxs-lookup"><span data-stu-id="d81df-140">The target group of PolicySetAssignment</span></span>|



## <a name="response"></a><span data-ttu-id="d81df-141">响应</span><span class="sxs-lookup"><span data-stu-id="d81df-141">Response</span></span>
<span data-ttu-id="d81df-142">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d81df-142">If successful, this method returns a `200 OK` response code and an updated [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d81df-143">示例</span><span class="sxs-lookup"><span data-stu-id="d81df-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="d81df-144">请求</span><span class="sxs-lookup"><span data-stu-id="d81df-144">Request</span></span>
<span data-ttu-id="d81df-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d81df-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/assignments/{policySetAssignmentId}
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="d81df-146">响应</span><span class="sxs-lookup"><span data-stu-id="d81df-146">Response</span></span>
<span data-ttu-id="d81df-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d81df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "id": "0a8e7d40-7d40-0a8e-407d-8e0a407d8e0a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```






