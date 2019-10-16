---
title: 创建 policySetAssignment
description: 创建新的 policySetAssignment 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d95a41b843844edf43f430c19685a689d2d73917
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536313"
---
# <a name="create-policysetassignment"></a><span data-ttu-id="a1ffa-103">创建 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="a1ffa-103">Create policySetAssignment</span></span>

> <span data-ttu-id="a1ffa-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a1ffa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1ffa-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1ffa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1ffa-106">创建新的[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a1ffa-106">Create a new [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1ffa-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a1ffa-107">Prerequisites</span></span>
<span data-ttu-id="a1ffa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1ffa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1ffa-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1ffa-110">Permission type</span></span>|<span data-ttu-id="a1ffa-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a1ffa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1ffa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1ffa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1ffa-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1ffa-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1ffa-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1ffa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1ffa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1ffa-115">Not supported.</span></span>|
|<span data-ttu-id="a1ffa-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1ffa-116">Application</span></span>|<span data-ttu-id="a1ffa-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1ffa-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1ffa-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1ffa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a1ffa-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1ffa-119">Request headers</span></span>
|<span data-ttu-id="a1ffa-120">标头</span><span class="sxs-lookup"><span data-stu-id="a1ffa-120">Header</span></span>|<span data-ttu-id="a1ffa-121">值</span><span class="sxs-lookup"><span data-stu-id="a1ffa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1ffa-122">授权</span><span class="sxs-lookup"><span data-stu-id="a1ffa-122">Authorization</span></span>|<span data-ttu-id="a1ffa-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a1ffa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1ffa-124">接受</span><span class="sxs-lookup"><span data-stu-id="a1ffa-124">Accept</span></span>|<span data-ttu-id="a1ffa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1ffa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1ffa-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1ffa-126">Request body</span></span>
<span data-ttu-id="a1ffa-127">在请求正文中，提供 policySetAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1ffa-127">In the request body, supply a JSON representation for the policySetAssignment object.</span></span>

<span data-ttu-id="a1ffa-128">下表显示创建 policySetAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a1ffa-128">The following table shows the properties that are required when you create the policySetAssignment.</span></span>

|<span data-ttu-id="a1ffa-129">属性</span><span class="sxs-lookup"><span data-stu-id="a1ffa-129">Property</span></span>|<span data-ttu-id="a1ffa-130">类型</span><span class="sxs-lookup"><span data-stu-id="a1ffa-130">Type</span></span>|<span data-ttu-id="a1ffa-131">说明</span><span class="sxs-lookup"><span data-stu-id="a1ffa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1ffa-132">id</span><span class="sxs-lookup"><span data-stu-id="a1ffa-132">id</span></span>|<span data-ttu-id="a1ffa-133">字符串</span><span class="sxs-lookup"><span data-stu-id="a1ffa-133">String</span></span>|<span data-ttu-id="a1ffa-134">PolicySetAssignment 的键。</span><span class="sxs-lookup"><span data-stu-id="a1ffa-134">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="a1ffa-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1ffa-135">lastModifiedDateTime</span></span>|<span data-ttu-id="a1ffa-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1ffa-136">DateTimeOffset</span></span>|<span data-ttu-id="a1ffa-137">PolicySetAssignment 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="a1ffa-137">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="a1ffa-138">target</span><span class="sxs-lookup"><span data-stu-id="a1ffa-138">target</span></span>|[<span data-ttu-id="a1ffa-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a1ffa-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a1ffa-140">PolicySetAssignment 的目标组</span><span class="sxs-lookup"><span data-stu-id="a1ffa-140">The target group of PolicySetAssignment</span></span>|



## <a name="response"></a><span data-ttu-id="a1ffa-141">响应</span><span class="sxs-lookup"><span data-stu-id="a1ffa-141">Response</span></span>
<span data-ttu-id="a1ffa-142">如果成功，此方法在响应`201 Created`正文中返回响应代码和[policySetAssignment](../resources/intune-policyset-policysetassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a1ffa-142">If successful, this method returns a `201 Created` response code and a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1ffa-143">示例</span><span class="sxs-lookup"><span data-stu-id="a1ffa-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1ffa-144">请求</span><span class="sxs-lookup"><span data-stu-id="a1ffa-144">Request</span></span>
<span data-ttu-id="a1ffa-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1ffa-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/assignments
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="a1ffa-146">响应</span><span class="sxs-lookup"><span data-stu-id="a1ffa-146">Response</span></span>
<span data-ttu-id="a1ffa-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1ffa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






