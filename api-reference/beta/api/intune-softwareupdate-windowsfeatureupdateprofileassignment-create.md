---
title: 创建 windowsFeatureUpdateProfileAssignment
description: 创建新的 windowsFeatureUpdateProfileAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 04f74ec382f1266bfceb9bbb438f655b9f464543
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457603"
---
# <a name="create-windowsfeatureupdateprofileassignment"></a><span data-ttu-id="b83c5-103">创建 windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="b83c5-103">Create windowsFeatureUpdateProfileAssignment</span></span>

<span data-ttu-id="b83c5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b83c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b83c5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b83c5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b83c5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b83c5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b83c5-107">创建新的[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b83c5-107">Create a new [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b83c5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b83c5-108">Prerequisites</span></span>
<span data-ttu-id="b83c5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b83c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b83c5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b83c5-111">Permission type</span></span>|<span data-ttu-id="b83c5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b83c5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b83c5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b83c5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b83c5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b83c5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b83c5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b83c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b83c5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b83c5-116">Not supported.</span></span>|
|<span data-ttu-id="b83c5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b83c5-117">Application</span></span>|<span data-ttu-id="b83c5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b83c5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b83c5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b83c5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b83c5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b83c5-120">Request headers</span></span>
|<span data-ttu-id="b83c5-121">标头</span><span class="sxs-lookup"><span data-stu-id="b83c5-121">Header</span></span>|<span data-ttu-id="b83c5-122">值</span><span class="sxs-lookup"><span data-stu-id="b83c5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b83c5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b83c5-123">Authorization</span></span>|<span data-ttu-id="b83c5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b83c5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b83c5-125">接受</span><span class="sxs-lookup"><span data-stu-id="b83c5-125">Accept</span></span>|<span data-ttu-id="b83c5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b83c5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b83c5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b83c5-127">Request body</span></span>
<span data-ttu-id="b83c5-128">在请求正文中，提供 windowsFeatureUpdateProfileAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b83c5-128">In the request body, supply a JSON representation for the windowsFeatureUpdateProfileAssignment object.</span></span>

<span data-ttu-id="b83c5-129">下表显示创建 windowsFeatureUpdateProfileAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b83c5-129">The following table shows the properties that are required when you create the windowsFeatureUpdateProfileAssignment.</span></span>

|<span data-ttu-id="b83c5-130">属性</span><span class="sxs-lookup"><span data-stu-id="b83c5-130">Property</span></span>|<span data-ttu-id="b83c5-131">类型</span><span class="sxs-lookup"><span data-stu-id="b83c5-131">Type</span></span>|<span data-ttu-id="b83c5-132">说明</span><span class="sxs-lookup"><span data-stu-id="b83c5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b83c5-133">id</span><span class="sxs-lookup"><span data-stu-id="b83c5-133">id</span></span>|<span data-ttu-id="b83c5-134">String</span><span class="sxs-lookup"><span data-stu-id="b83c5-134">String</span></span>|<span data-ttu-id="b83c5-135">实体的标识符</span><span class="sxs-lookup"><span data-stu-id="b83c5-135">The Identifier of the entity</span></span>|
|<span data-ttu-id="b83c5-136">target</span><span class="sxs-lookup"><span data-stu-id="b83c5-136">target</span></span>|[<span data-ttu-id="b83c5-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b83c5-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b83c5-138">将功能更新配置文件分配到的工作分配目标。</span><span class="sxs-lookup"><span data-stu-id="b83c5-138">The assignment target that the feature update profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="b83c5-139">响应</span><span class="sxs-lookup"><span data-stu-id="b83c5-139">Response</span></span>
<span data-ttu-id="b83c5-140">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b83c5-140">If successful, this method returns a `201 Created` response code and a [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b83c5-141">示例</span><span class="sxs-lookup"><span data-stu-id="b83c5-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="b83c5-142">请求</span><span class="sxs-lookup"><span data-stu-id="b83c5-142">Request</span></span>
<span data-ttu-id="b83c5-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b83c5-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments
Content-type: application/json
Content-length: 177

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="b83c5-144">响应</span><span class="sxs-lookup"><span data-stu-id="b83c5-144">Response</span></span>
<span data-ttu-id="b83c5-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b83c5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 226

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
  "id": "567a744f-744f-567a-4f74-7a564f747a56",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



