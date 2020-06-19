---
title: 更新 intuneBrandingProfileAssignment
description: 更新 intuneBrandingProfileAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 718a2e538b619a4138ef64987009bd5f6415851a
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791207"
---
# <a name="update-intunebrandingprofileassignment"></a><span data-ttu-id="52e13-103">更新 intuneBrandingProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="52e13-103">Update intuneBrandingProfileAssignment</span></span>

<span data-ttu-id="52e13-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52e13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52e13-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="52e13-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52e13-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="52e13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52e13-107">更新[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="52e13-107">Update the properties of a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52e13-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="52e13-108">Prerequisites</span></span>
<span data-ttu-id="52e13-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="52e13-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="52e13-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52e13-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52e13-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="52e13-111">Permission type</span></span>|<span data-ttu-id="52e13-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="52e13-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52e13-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="52e13-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52e13-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52e13-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="52e13-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="52e13-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52e13-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="52e13-116">Not supported.</span></span>|
|<span data-ttu-id="52e13-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="52e13-117">Application</span></span>|<span data-ttu-id="52e13-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52e13-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52e13-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="52e13-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="52e13-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="52e13-120">Request headers</span></span>
|<span data-ttu-id="52e13-121">标头</span><span class="sxs-lookup"><span data-stu-id="52e13-121">Header</span></span>|<span data-ttu-id="52e13-122">值</span><span class="sxs-lookup"><span data-stu-id="52e13-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52e13-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="52e13-123">Authorization</span></span>|<span data-ttu-id="52e13-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="52e13-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52e13-125">接受</span><span class="sxs-lookup"><span data-stu-id="52e13-125">Accept</span></span>|<span data-ttu-id="52e13-126">application/json</span><span class="sxs-lookup"><span data-stu-id="52e13-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52e13-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="52e13-127">Request body</span></span>
<span data-ttu-id="52e13-128">在请求正文中，提供[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52e13-128">In the request body, supply a JSON representation for the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

<span data-ttu-id="52e13-129">下表显示创建[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="52e13-129">The following table shows the properties that are required when you create the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span></span>

|<span data-ttu-id="52e13-130">属性</span><span class="sxs-lookup"><span data-stu-id="52e13-130">Property</span></span>|<span data-ttu-id="52e13-131">类型</span><span class="sxs-lookup"><span data-stu-id="52e13-131">Type</span></span>|<span data-ttu-id="52e13-132">说明</span><span class="sxs-lookup"><span data-stu-id="52e13-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52e13-133">id</span><span class="sxs-lookup"><span data-stu-id="52e13-133">id</span></span>|<span data-ttu-id="52e13-134">String</span><span class="sxs-lookup"><span data-stu-id="52e13-134">String</span></span>|<span data-ttu-id="52e13-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="52e13-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="52e13-136">target</span><span class="sxs-lookup"><span data-stu-id="52e13-136">target</span></span>|[<span data-ttu-id="52e13-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="52e13-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="52e13-138">为品牌配置文件分配的工作分配目标。</span><span class="sxs-lookup"><span data-stu-id="52e13-138">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="52e13-139">响应</span><span class="sxs-lookup"><span data-stu-id="52e13-139">Response</span></span>
<span data-ttu-id="52e13-140">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="52e13-140">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52e13-141">示例</span><span class="sxs-lookup"><span data-stu-id="52e13-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="52e13-142">请求</span><span class="sxs-lookup"><span data-stu-id="52e13-142">Request</span></span>
<span data-ttu-id="52e13-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="52e13-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
Content-type: application/json
Content-length: 326

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="52e13-144">响应</span><span class="sxs-lookup"><span data-stu-id="52e13-144">Response</span></span>
<span data-ttu-id="52e13-145">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="52e13-145">Here is an example of the response.</span></span> <span data-ttu-id="52e13-146">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="52e13-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="52e13-147">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="52e13-147">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 375

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```



