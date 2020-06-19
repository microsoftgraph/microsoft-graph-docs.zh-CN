---
title: 更新 windowsFeatureUpdateProfileAssignment
description: 更新 windowsFeatureUpdateProfileAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 97a6cf5562c92498769f81a262e3fb290c689b4b
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791277"
---
# <a name="update-windowsfeatureupdateprofileassignment"></a><span data-ttu-id="41259-103">更新 windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="41259-103">Update windowsFeatureUpdateProfileAssignment</span></span>

<span data-ttu-id="41259-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41259-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41259-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="41259-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41259-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="41259-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41259-107">更新[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="41259-107">Update the properties of a [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41259-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="41259-108">Prerequisites</span></span>
<span data-ttu-id="41259-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="41259-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="41259-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41259-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41259-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="41259-111">Permission type</span></span>|<span data-ttu-id="41259-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="41259-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41259-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41259-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41259-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41259-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41259-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41259-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41259-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="41259-116">Not supported.</span></span>|
|<span data-ttu-id="41259-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="41259-117">Application</span></span>|<span data-ttu-id="41259-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41259-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41259-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41259-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments/{windowsFeatureUpdateProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="41259-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="41259-120">Request headers</span></span>
|<span data-ttu-id="41259-121">标头</span><span class="sxs-lookup"><span data-stu-id="41259-121">Header</span></span>|<span data-ttu-id="41259-122">值</span><span class="sxs-lookup"><span data-stu-id="41259-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41259-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="41259-123">Authorization</span></span>|<span data-ttu-id="41259-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="41259-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41259-125">接受</span><span class="sxs-lookup"><span data-stu-id="41259-125">Accept</span></span>|<span data-ttu-id="41259-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41259-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41259-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="41259-127">Request body</span></span>
<span data-ttu-id="41259-128">在请求正文中，提供[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41259-128">In the request body, supply a JSON representation for the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>

<span data-ttu-id="41259-129">下表显示创建[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="41259-129">The following table shows the properties that are required when you create the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md).</span></span>

|<span data-ttu-id="41259-130">属性</span><span class="sxs-lookup"><span data-stu-id="41259-130">Property</span></span>|<span data-ttu-id="41259-131">类型</span><span class="sxs-lookup"><span data-stu-id="41259-131">Type</span></span>|<span data-ttu-id="41259-132">说明</span><span class="sxs-lookup"><span data-stu-id="41259-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41259-133">id</span><span class="sxs-lookup"><span data-stu-id="41259-133">id</span></span>|<span data-ttu-id="41259-134">String</span><span class="sxs-lookup"><span data-stu-id="41259-134">String</span></span>|<span data-ttu-id="41259-135">实体的标识符</span><span class="sxs-lookup"><span data-stu-id="41259-135">The Identifier of the entity</span></span>|
|<span data-ttu-id="41259-136">target</span><span class="sxs-lookup"><span data-stu-id="41259-136">target</span></span>|[<span data-ttu-id="41259-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="41259-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="41259-138">将功能更新配置文件分配到的工作分配目标。</span><span class="sxs-lookup"><span data-stu-id="41259-138">The assignment target that the feature update profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="41259-139">响应</span><span class="sxs-lookup"><span data-stu-id="41259-139">Response</span></span>
<span data-ttu-id="41259-140">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="41259-140">If successful, this method returns a `200 OK` response code and an updated [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41259-141">示例</span><span class="sxs-lookup"><span data-stu-id="41259-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="41259-142">请求</span><span class="sxs-lookup"><span data-stu-id="41259-142">Request</span></span>
<span data-ttu-id="41259-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41259-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments/{windowsFeatureUpdateProfileAssignmentId}
Content-type: application/json
Content-length: 344

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="41259-144">响应</span><span class="sxs-lookup"><span data-stu-id="41259-144">Response</span></span>
<span data-ttu-id="41259-145">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="41259-145">Here is an example of the response.</span></span> <span data-ttu-id="41259-146">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="41259-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="41259-147">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="41259-147">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 393

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
  "id": "567a744f-744f-567a-4f74-7a564f747a56",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```



