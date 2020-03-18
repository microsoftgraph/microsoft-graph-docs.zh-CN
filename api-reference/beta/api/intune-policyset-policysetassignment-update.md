---
title: 更新 policySetAssignment
description: 更新 policySetAssignment 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 70f679df2c85caecf9286952bfadb6ddbf6f1c17
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802074"
---
# <a name="update-policysetassignment"></a><span data-ttu-id="82ed2-103">更新 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="82ed2-103">Update policySetAssignment</span></span>

> <span data-ttu-id="82ed2-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="82ed2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82ed2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="82ed2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82ed2-106">更新[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="82ed2-106">Update the properties of a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82ed2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="82ed2-107">Prerequisites</span></span>
<span data-ttu-id="82ed2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82ed2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82ed2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="82ed2-110">Permission type</span></span>|<span data-ttu-id="82ed2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="82ed2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82ed2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82ed2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82ed2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82ed2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82ed2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82ed2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82ed2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="82ed2-115">Not supported.</span></span>|
|<span data-ttu-id="82ed2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="82ed2-116">Application</span></span>|<span data-ttu-id="82ed2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82ed2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82ed2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82ed2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/assignments/{policySetAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="82ed2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="82ed2-119">Request headers</span></span>
|<span data-ttu-id="82ed2-120">标头</span><span class="sxs-lookup"><span data-stu-id="82ed2-120">Header</span></span>|<span data-ttu-id="82ed2-121">值</span><span class="sxs-lookup"><span data-stu-id="82ed2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82ed2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82ed2-122">Authorization</span></span>|<span data-ttu-id="82ed2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="82ed2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82ed2-124">接受</span><span class="sxs-lookup"><span data-stu-id="82ed2-124">Accept</span></span>|<span data-ttu-id="82ed2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82ed2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82ed2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="82ed2-126">Request body</span></span>
<span data-ttu-id="82ed2-127">在请求正文中，提供[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82ed2-127">In the request body, supply a JSON representation for the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

<span data-ttu-id="82ed2-128">下表显示创建[policySetAssignment](../resources/intune-policyset-policysetassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="82ed2-128">The following table shows the properties that are required when you create the [policySetAssignment](../resources/intune-policyset-policysetassignment.md).</span></span>

|<span data-ttu-id="82ed2-129">属性</span><span class="sxs-lookup"><span data-stu-id="82ed2-129">Property</span></span>|<span data-ttu-id="82ed2-130">类型</span><span class="sxs-lookup"><span data-stu-id="82ed2-130">Type</span></span>|<span data-ttu-id="82ed2-131">说明</span><span class="sxs-lookup"><span data-stu-id="82ed2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82ed2-132">id</span><span class="sxs-lookup"><span data-stu-id="82ed2-132">id</span></span>|<span data-ttu-id="82ed2-133">String</span><span class="sxs-lookup"><span data-stu-id="82ed2-133">String</span></span>|<span data-ttu-id="82ed2-134">PolicySetAssignment 的键。</span><span class="sxs-lookup"><span data-stu-id="82ed2-134">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="82ed2-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82ed2-135">lastModifiedDateTime</span></span>|<span data-ttu-id="82ed2-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82ed2-136">DateTimeOffset</span></span>|<span data-ttu-id="82ed2-137">PolicySetAssignment 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="82ed2-137">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="82ed2-138">target</span><span class="sxs-lookup"><span data-stu-id="82ed2-138">target</span></span>|[<span data-ttu-id="82ed2-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="82ed2-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="82ed2-140">PolicySetAssignment 的目标组</span><span class="sxs-lookup"><span data-stu-id="82ed2-140">The target group of PolicySetAssignment</span></span>|



## <a name="response"></a><span data-ttu-id="82ed2-141">响应</span><span class="sxs-lookup"><span data-stu-id="82ed2-141">Response</span></span>
<span data-ttu-id="82ed2-142">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="82ed2-142">If successful, this method returns a `200 OK` response code and an updated [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82ed2-143">示例</span><span class="sxs-lookup"><span data-stu-id="82ed2-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="82ed2-144">请求</span><span class="sxs-lookup"><span data-stu-id="82ed2-144">Request</span></span>
<span data-ttu-id="82ed2-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="82ed2-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="82ed2-146">响应</span><span class="sxs-lookup"><span data-stu-id="82ed2-146">Response</span></span>
<span data-ttu-id="82ed2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="82ed2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




