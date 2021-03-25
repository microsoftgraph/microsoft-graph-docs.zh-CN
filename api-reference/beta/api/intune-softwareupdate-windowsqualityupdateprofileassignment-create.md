---
title: 创建 windowsQualityUpdateProfileAssignment
description: 创建新的 windowsQualityUpdateProfileAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b4c1c7feb40af06d8baefcfbc7642c828114e208
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156168"
---
# <a name="create-windowsqualityupdateprofileassignment"></a><span data-ttu-id="1d9f6-103">创建 windowsQualityUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="1d9f6-103">Create windowsQualityUpdateProfileAssignment</span></span>

<span data-ttu-id="1d9f6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d9f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d9f6-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1d9f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d9f6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1d9f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d9f6-107">创建新的 [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1d9f6-107">Create a new [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d9f6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1d9f6-108">Prerequisites</span></span>
<span data-ttu-id="1d9f6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1d9f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d9f6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1d9f6-111">Permission type</span></span>|<span data-ttu-id="1d9f6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1d9f6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d9f6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1d9f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d9f6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d9f6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1d9f6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1d9f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d9f6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1d9f6-116">Not supported.</span></span>|
|<span data-ttu-id="1d9f6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1d9f6-117">Application</span></span>|<span data-ttu-id="1d9f6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d9f6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d9f6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d9f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1d9f6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1d9f6-120">Request headers</span></span>
|<span data-ttu-id="1d9f6-121">标头</span><span class="sxs-lookup"><span data-stu-id="1d9f6-121">Header</span></span>|<span data-ttu-id="1d9f6-122">值</span><span class="sxs-lookup"><span data-stu-id="1d9f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d9f6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d9f6-123">Authorization</span></span>|<span data-ttu-id="1d9f6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1d9f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d9f6-125">接受</span><span class="sxs-lookup"><span data-stu-id="1d9f6-125">Accept</span></span>|<span data-ttu-id="1d9f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d9f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d9f6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1d9f6-127">Request body</span></span>
<span data-ttu-id="1d9f6-128">在请求正文中，提供 windowsQualityUpdateProfileAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d9f6-128">In the request body, supply a JSON representation for the windowsQualityUpdateProfileAssignment object.</span></span>

<span data-ttu-id="1d9f6-129">下表显示创建 windowsQualityUpdateProfileAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1d9f6-129">The following table shows the properties that are required when you create the windowsQualityUpdateProfileAssignment.</span></span>

|<span data-ttu-id="1d9f6-130">属性</span><span class="sxs-lookup"><span data-stu-id="1d9f6-130">Property</span></span>|<span data-ttu-id="1d9f6-131">类型</span><span class="sxs-lookup"><span data-stu-id="1d9f6-131">Type</span></span>|<span data-ttu-id="1d9f6-132">说明</span><span class="sxs-lookup"><span data-stu-id="1d9f6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d9f6-133">id</span><span class="sxs-lookup"><span data-stu-id="1d9f6-133">id</span></span>|<span data-ttu-id="1d9f6-134">String</span><span class="sxs-lookup"><span data-stu-id="1d9f6-134">String</span></span>|<span data-ttu-id="1d9f6-135">实体的标识符</span><span class="sxs-lookup"><span data-stu-id="1d9f6-135">The Identifier of the entity</span></span>|
|<span data-ttu-id="1d9f6-136">target</span><span class="sxs-lookup"><span data-stu-id="1d9f6-136">target</span></span>|[<span data-ttu-id="1d9f6-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1d9f6-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1d9f6-138">功能更新配置文件分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="1d9f6-138">The assignment target that the feature update profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="1d9f6-139">响应</span><span class="sxs-lookup"><span data-stu-id="1d9f6-139">Response</span></span>
<span data-ttu-id="1d9f6-140">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1d9f6-140">If successful, this method returns a `201 Created` response code and a [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d9f6-141">示例</span><span class="sxs-lookup"><span data-stu-id="1d9f6-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d9f6-142">请求</span><span class="sxs-lookup"><span data-stu-id="1d9f6-142">Request</span></span>
<span data-ttu-id="1d9f6-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1d9f6-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}/assignments
Content-type: application/json
Content-length: 344

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="1d9f6-144">响应</span><span class="sxs-lookup"><span data-stu-id="1d9f6-144">Response</span></span>
<span data-ttu-id="1d9f6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1d9f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 393

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfileAssignment",
  "id": "0c3a8422-8422-0c3a-2284-3a0c22843a0c",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```




