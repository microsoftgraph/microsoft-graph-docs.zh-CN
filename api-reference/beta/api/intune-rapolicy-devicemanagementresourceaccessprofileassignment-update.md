---
title: 更新 deviceManagementResourceAccessProfileAssignment
description: 更新 deviceManagementResourceAccessProfileAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1cc09d3d66ba27ae440688a7a18bbfdc3bbd1246
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161990"
---
# <a name="update-devicemanagementresourceaccessprofileassignment"></a><span data-ttu-id="5b909-103">更新 deviceManagementResourceAccessProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="5b909-103">Update deviceManagementResourceAccessProfileAssignment</span></span>

<span data-ttu-id="5b909-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b909-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b909-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5b909-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b909-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5b909-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b909-107">更新 [deviceManagementResourceAccessProfileAssignment 对象](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="5b909-107">Update the properties of a [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b909-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5b909-108">Prerequisites</span></span>
<span data-ttu-id="5b909-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5b909-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b909-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b909-111">Permission type</span></span>|<span data-ttu-id="5b909-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5b909-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b909-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b909-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b909-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b909-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5b909-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b909-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b909-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b909-116">Not supported.</span></span>|
|<span data-ttu-id="5b909-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b909-117">Application</span></span>|<span data-ttu-id="5b909-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b909-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b909-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b909-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assignments/{deviceManagementResourceAccessProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="5b909-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b909-120">Request headers</span></span>
|<span data-ttu-id="5b909-121">标头</span><span class="sxs-lookup"><span data-stu-id="5b909-121">Header</span></span>|<span data-ttu-id="5b909-122">值</span><span class="sxs-lookup"><span data-stu-id="5b909-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b909-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b909-123">Authorization</span></span>|<span data-ttu-id="5b909-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5b909-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b909-125">接受</span><span class="sxs-lookup"><span data-stu-id="5b909-125">Accept</span></span>|<span data-ttu-id="5b909-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b909-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b909-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b909-127">Request body</span></span>
<span data-ttu-id="5b909-128">在请求正文中，提供 [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b909-128">In the request body, supply a JSON representation for the [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object.</span></span>

<span data-ttu-id="5b909-129">下表显示创建 [deviceManagementResourceAccessProfileAssignment 时所需的属性](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="5b909-129">The following table shows the properties that are required when you create the [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md).</span></span>

|<span data-ttu-id="5b909-130">属性</span><span class="sxs-lookup"><span data-stu-id="5b909-130">Property</span></span>|<span data-ttu-id="5b909-131">类型</span><span class="sxs-lookup"><span data-stu-id="5b909-131">Type</span></span>|<span data-ttu-id="5b909-132">说明</span><span class="sxs-lookup"><span data-stu-id="5b909-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b909-133">id</span><span class="sxs-lookup"><span data-stu-id="5b909-133">id</span></span>|<span data-ttu-id="5b909-134">String</span><span class="sxs-lookup"><span data-stu-id="5b909-134">String</span></span>|<span data-ttu-id="5b909-135">工作分配的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="5b909-135">Unique identifier for the Assignments</span></span>|
|<span data-ttu-id="5b909-136">intent</span><span class="sxs-lookup"><span data-stu-id="5b909-136">intent</span></span>|[<span data-ttu-id="5b909-137">deviceManagementResourceAccessProfileIntent</span><span class="sxs-lookup"><span data-stu-id="5b909-137">deviceManagementResourceAccessProfileIntent</span></span>](../resources/intune-rapolicy-devicemanagementresourceaccessprofileintent.md)|<span data-ttu-id="5b909-138">资源访问配置文件的分配意图。</span><span class="sxs-lookup"><span data-stu-id="5b909-138">The assignment intent for the resource access profile.</span></span> <span data-ttu-id="5b909-139">可取值为：`apply`、`remove`。</span><span class="sxs-lookup"><span data-stu-id="5b909-139">Possible values are: `apply`, `remove`.</span></span>|
|<span data-ttu-id="5b909-140">target</span><span class="sxs-lookup"><span data-stu-id="5b909-140">target</span></span>|[<span data-ttu-id="5b909-141">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5b909-141">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5b909-142">资源访问配置文件的分配目标。</span><span class="sxs-lookup"><span data-stu-id="5b909-142">The assignment target for the resource access profile.</span></span>|
|<span data-ttu-id="5b909-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="5b909-143">sourceId</span></span>|<span data-ttu-id="5b909-144">String</span><span class="sxs-lookup"><span data-stu-id="5b909-144">String</span></span>|<span data-ttu-id="5b909-145">工作分配的源的标识符。</span><span class="sxs-lookup"><span data-stu-id="5b909-145">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="5b909-146">响应</span><span class="sxs-lookup"><span data-stu-id="5b909-146">Response</span></span>
<span data-ttu-id="5b909-147">如果成功，此方法在响应正文中返回响应代码和更新 `200 OK` [的 deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5b909-147">If successful, this method returns a `200 OK` response code and an updated [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b909-148">示例</span><span class="sxs-lookup"><span data-stu-id="5b909-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b909-149">请求</span><span class="sxs-lookup"><span data-stu-id="5b909-149">Request</span></span>
<span data-ttu-id="5b909-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5b909-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assignments/{deviceManagementResourceAccessProfileAssignmentId}
Content-type: application/json
Content-length: 463

{
  "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileAssignment",
  "intent": "remove",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  },
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="5b909-151">响应</span><span class="sxs-lookup"><span data-stu-id="5b909-151">Response</span></span>
<span data-ttu-id="5b909-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5b909-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileAssignment",
  "id": "4ebb8d4e-8d4e-4ebb-4e8d-bb4e4e8dbb4e",
  "intent": "remove",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  },
  "sourceId": "Source Id value"
}
```




