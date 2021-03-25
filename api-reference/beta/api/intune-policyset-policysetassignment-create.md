---
title: 创建 policySetAssignment
description: 创建新的 policySetAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 66cc853d9fc34a2de3a155e6a0dd6ddce2f5f815
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152374"
---
# <a name="create-policysetassignment"></a><span data-ttu-id="665bd-103">创建 policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="665bd-103">Create policySetAssignment</span></span>

<span data-ttu-id="665bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="665bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="665bd-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="665bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="665bd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="665bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="665bd-107">创建新的 [policySetAssignment](../resources/intune-policyset-policysetassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="665bd-107">Create a new [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="665bd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="665bd-108">Prerequisites</span></span>
<span data-ttu-id="665bd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="665bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="665bd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="665bd-111">Permission type</span></span>|<span data-ttu-id="665bd-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="665bd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="665bd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="665bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="665bd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="665bd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="665bd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="665bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="665bd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="665bd-116">Not supported.</span></span>|
|<span data-ttu-id="665bd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="665bd-117">Application</span></span>|<span data-ttu-id="665bd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="665bd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="665bd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="665bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="665bd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="665bd-120">Request headers</span></span>
|<span data-ttu-id="665bd-121">标头</span><span class="sxs-lookup"><span data-stu-id="665bd-121">Header</span></span>|<span data-ttu-id="665bd-122">值</span><span class="sxs-lookup"><span data-stu-id="665bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="665bd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="665bd-123">Authorization</span></span>|<span data-ttu-id="665bd-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="665bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="665bd-125">接受</span><span class="sxs-lookup"><span data-stu-id="665bd-125">Accept</span></span>|<span data-ttu-id="665bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="665bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="665bd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="665bd-127">Request body</span></span>
<span data-ttu-id="665bd-128">在请求正文中，提供 policySetAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="665bd-128">In the request body, supply a JSON representation for the policySetAssignment object.</span></span>

<span data-ttu-id="665bd-129">下表显示创建 policySetAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="665bd-129">The following table shows the properties that are required when you create the policySetAssignment.</span></span>

|<span data-ttu-id="665bd-130">属性</span><span class="sxs-lookup"><span data-stu-id="665bd-130">Property</span></span>|<span data-ttu-id="665bd-131">类型</span><span class="sxs-lookup"><span data-stu-id="665bd-131">Type</span></span>|<span data-ttu-id="665bd-132">说明</span><span class="sxs-lookup"><span data-stu-id="665bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="665bd-133">id</span><span class="sxs-lookup"><span data-stu-id="665bd-133">id</span></span>|<span data-ttu-id="665bd-134">String</span><span class="sxs-lookup"><span data-stu-id="665bd-134">String</span></span>|<span data-ttu-id="665bd-135">PolicySetAssignment 的键。</span><span class="sxs-lookup"><span data-stu-id="665bd-135">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="665bd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="665bd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="665bd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="665bd-137">DateTimeOffset</span></span>|<span data-ttu-id="665bd-138">PolicySetAssignment 的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="665bd-138">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="665bd-139">target</span><span class="sxs-lookup"><span data-stu-id="665bd-139">target</span></span>|[<span data-ttu-id="665bd-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="665bd-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="665bd-141">PolicySetAssignment 的目标组</span><span class="sxs-lookup"><span data-stu-id="665bd-141">The target group of PolicySetAssignment</span></span>|



## <a name="response"></a><span data-ttu-id="665bd-142">响应</span><span class="sxs-lookup"><span data-stu-id="665bd-142">Response</span></span>
<span data-ttu-id="665bd-143">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [policySetAssignment](../resources/intune-policyset-policysetassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="665bd-143">If successful, this method returns a `201 Created` response code and a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="665bd-144">示例</span><span class="sxs-lookup"><span data-stu-id="665bd-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="665bd-145">请求</span><span class="sxs-lookup"><span data-stu-id="665bd-145">Request</span></span>
<span data-ttu-id="665bd-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="665bd-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/assignments
Content-type: application/json
Content-length: 378

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="665bd-147">响应</span><span class="sxs-lookup"><span data-stu-id="665bd-147">Response</span></span>
<span data-ttu-id="665bd-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="665bd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 491

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "id": "0a8e7d40-7d40-0a8e-407d-8e0a407d8e0a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```




