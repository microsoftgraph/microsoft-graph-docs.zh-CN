---
title: 创建 deviceManagementResourceAccessProfileAssignment
description: 创建新的 deviceManagementResourceAccessProfileAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1053da56d274206d7f050797350d8948d55fa7b3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301549"
---
# <a name="create-devicemanagementresourceaccessprofileassignment"></a><span data-ttu-id="cbfed-103">创建 deviceManagementResourceAccessProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="cbfed-103">Create deviceManagementResourceAccessProfileAssignment</span></span>

<span data-ttu-id="cbfed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbfed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cbfed-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cbfed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbfed-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cbfed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbfed-107">创建新的 [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cbfed-107">Create a new [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbfed-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cbfed-108">Prerequisites</span></span>
<span data-ttu-id="cbfed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cbfed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbfed-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cbfed-111">Permission type</span></span>|<span data-ttu-id="cbfed-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cbfed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbfed-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cbfed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cbfed-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbfed-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cbfed-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cbfed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbfed-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cbfed-116">Not supported.</span></span>|
|<span data-ttu-id="cbfed-117">Application</span><span class="sxs-lookup"><span data-stu-id="cbfed-117">Application</span></span>|<span data-ttu-id="cbfed-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbfed-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbfed-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cbfed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="cbfed-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cbfed-120">Request headers</span></span>
|<span data-ttu-id="cbfed-121">标头</span><span class="sxs-lookup"><span data-stu-id="cbfed-121">Header</span></span>|<span data-ttu-id="cbfed-122">值</span><span class="sxs-lookup"><span data-stu-id="cbfed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbfed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbfed-123">Authorization</span></span>|<span data-ttu-id="cbfed-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cbfed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbfed-125">接受</span><span class="sxs-lookup"><span data-stu-id="cbfed-125">Accept</span></span>|<span data-ttu-id="cbfed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cbfed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbfed-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cbfed-127">Request body</span></span>
<span data-ttu-id="cbfed-128">在请求正文中，提供 deviceManagementResourceAccessProfileAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cbfed-128">In the request body, supply a JSON representation for the deviceManagementResourceAccessProfileAssignment object.</span></span>

<span data-ttu-id="cbfed-129">下表显示创建 deviceManagementResourceAccessProfileAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cbfed-129">The following table shows the properties that are required when you create the deviceManagementResourceAccessProfileAssignment.</span></span>

|<span data-ttu-id="cbfed-130">属性</span><span class="sxs-lookup"><span data-stu-id="cbfed-130">Property</span></span>|<span data-ttu-id="cbfed-131">类型</span><span class="sxs-lookup"><span data-stu-id="cbfed-131">Type</span></span>|<span data-ttu-id="cbfed-132">说明</span><span class="sxs-lookup"><span data-stu-id="cbfed-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbfed-133">id</span><span class="sxs-lookup"><span data-stu-id="cbfed-133">id</span></span>|<span data-ttu-id="cbfed-134">字符串</span><span class="sxs-lookup"><span data-stu-id="cbfed-134">String</span></span>|<span data-ttu-id="cbfed-135">工作分配的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="cbfed-135">Unique identifier for the Assignments</span></span>|
|<span data-ttu-id="cbfed-136">intent</span><span class="sxs-lookup"><span data-stu-id="cbfed-136">intent</span></span>|[<span data-ttu-id="cbfed-137">deviceManagementResourceAccessProfileIntent</span><span class="sxs-lookup"><span data-stu-id="cbfed-137">deviceManagementResourceAccessProfileIntent</span></span>](../resources/intune-rapolicy-devicemanagementresourceaccessprofileintent.md)|<span data-ttu-id="cbfed-138">资源访问配置文件的分配意图。</span><span class="sxs-lookup"><span data-stu-id="cbfed-138">The assignment intent for the resource access profile.</span></span> <span data-ttu-id="cbfed-139">可取值为：`apply`、`remove`。</span><span class="sxs-lookup"><span data-stu-id="cbfed-139">Possible values are: `apply`, `remove`.</span></span>|
|<span data-ttu-id="cbfed-140">target</span><span class="sxs-lookup"><span data-stu-id="cbfed-140">target</span></span>|[<span data-ttu-id="cbfed-141">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cbfed-141">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="cbfed-142">资源访问配置文件的分配目标。</span><span class="sxs-lookup"><span data-stu-id="cbfed-142">The assignment target for the resource access profile.</span></span>|
|<span data-ttu-id="cbfed-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="cbfed-143">sourceId</span></span>|<span data-ttu-id="cbfed-144">字符串</span><span class="sxs-lookup"><span data-stu-id="cbfed-144">String</span></span>|<span data-ttu-id="cbfed-145">工作分配的源的标识符。</span><span class="sxs-lookup"><span data-stu-id="cbfed-145">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="cbfed-146">响应</span><span class="sxs-lookup"><span data-stu-id="cbfed-146">Response</span></span>
<span data-ttu-id="cbfed-147">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cbfed-147">If successful, this method returns a `201 Created` response code and a [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbfed-148">示例</span><span class="sxs-lookup"><span data-stu-id="cbfed-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbfed-149">请求</span><span class="sxs-lookup"><span data-stu-id="cbfed-149">Request</span></span>
<span data-ttu-id="cbfed-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cbfed-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assignments
Content-type: application/json
Content-length: 399

{
  "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileAssignment",
  "intent": "remove",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="cbfed-151">响应</span><span class="sxs-lookup"><span data-stu-id="cbfed-151">Response</span></span>
<span data-ttu-id="cbfed-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cbfed-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 448

{
  "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileAssignment",
  "id": "4ebb8d4e-8d4e-4ebb-4e8d-bb4e4e8dbb4e",
  "intent": "remove",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "sourceId": "Source Id value"
}
```




