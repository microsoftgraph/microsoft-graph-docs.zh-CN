---
title: 创建 roleScopeTagAutoAssignment
description: 创建新的 roleScopeTagAutoAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 337d7adaea4b27c6a1c451e463a36f58ab48ee6f
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791677"
---
# <a name="create-rolescopetagautoassignment"></a><span data-ttu-id="f1330-103">创建 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="f1330-103">Create roleScopeTagAutoAssignment</span></span>

<span data-ttu-id="f1330-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1330-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1330-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f1330-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1330-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f1330-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1330-107">创建新的[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f1330-107">Create a new [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1330-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f1330-108">Prerequisites</span></span>
<span data-ttu-id="f1330-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f1330-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f1330-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1330-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1330-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1330-111">Permission type</span></span>|<span data-ttu-id="f1330-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f1330-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1330-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1330-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1330-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1330-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="f1330-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1330-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1330-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1330-116">Not supported.</span></span>|
|<span data-ttu-id="f1330-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1330-117">Application</span></span>|<span data-ttu-id="f1330-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1330-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1330-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1330-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="f1330-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1330-120">Request headers</span></span>
|<span data-ttu-id="f1330-121">标头</span><span class="sxs-lookup"><span data-stu-id="f1330-121">Header</span></span>|<span data-ttu-id="f1330-122">值</span><span class="sxs-lookup"><span data-stu-id="f1330-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1330-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1330-123">Authorization</span></span>|<span data-ttu-id="f1330-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f1330-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1330-125">接受</span><span class="sxs-lookup"><span data-stu-id="f1330-125">Accept</span></span>|<span data-ttu-id="f1330-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1330-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1330-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1330-127">Request body</span></span>
<span data-ttu-id="f1330-128">在请求正文中，提供 roleScopeTagAutoAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1330-128">In the request body, supply a JSON representation for the roleScopeTagAutoAssignment object.</span></span>

<span data-ttu-id="f1330-129">下表显示创建 roleScopeTagAutoAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f1330-129">The following table shows the properties that are required when you create the roleScopeTagAutoAssignment.</span></span>

|<span data-ttu-id="f1330-130">属性</span><span class="sxs-lookup"><span data-stu-id="f1330-130">Property</span></span>|<span data-ttu-id="f1330-131">类型</span><span class="sxs-lookup"><span data-stu-id="f1330-131">Type</span></span>|<span data-ttu-id="f1330-132">说明</span><span class="sxs-lookup"><span data-stu-id="f1330-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1330-133">id</span><span class="sxs-lookup"><span data-stu-id="f1330-133">id</span></span>|<span data-ttu-id="f1330-134">String</span><span class="sxs-lookup"><span data-stu-id="f1330-134">String</span></span>|<span data-ttu-id="f1330-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f1330-135">Key of the entity.</span></span>|
|<span data-ttu-id="f1330-136">target</span><span class="sxs-lookup"><span data-stu-id="f1330-136">target</span></span>|[<span data-ttu-id="f1330-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f1330-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f1330-138">特定角色范围标记的自动分配目标。</span><span class="sxs-lookup"><span data-stu-id="f1330-138">The auto-assignment target for the specific Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="f1330-139">响应</span><span class="sxs-lookup"><span data-stu-id="f1330-139">Response</span></span>
<span data-ttu-id="f1330-140">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f1330-140">If successful, this method returns a `201 Created` response code and a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1330-141">示例</span><span class="sxs-lookup"><span data-stu-id="f1330-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1330-142">请求</span><span class="sxs-lookup"><span data-stu-id="f1330-142">Request</span></span>
<span data-ttu-id="f1330-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f1330-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
Content-type: application/json
Content-length: 321

{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="f1330-144">响应</span><span class="sxs-lookup"><span data-stu-id="f1330-144">Response</span></span>
<span data-ttu-id="f1330-145">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="f1330-145">Here is an example of the response.</span></span> <span data-ttu-id="f1330-146">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="f1330-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f1330-147">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f1330-147">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 370

{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "id": "256e6375-6375-256e-7563-6e2575636e25",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```



