---
title: 更新 roleScopeTagAutoAssignment
description: 更新 roleScopeTagAutoAssignment 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0b177e224c3e0392517a66a964a0a05216c7c8fd
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955152"
---
# <a name="update-rolescopetagautoassignment"></a><span data-ttu-id="abff4-103">更新 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="abff4-103">Update roleScopeTagAutoAssignment</span></span>

> <span data-ttu-id="abff4-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="abff4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abff4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="abff4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abff4-106">更新[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="abff4-106">Update the properties of a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abff4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="abff4-107">Prerequisites</span></span>
<span data-ttu-id="abff4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="abff4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abff4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="abff4-110">Permission type</span></span>|<span data-ttu-id="abff4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="abff4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abff4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="abff4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="abff4-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abff4-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="abff4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="abff4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abff4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="abff4-115">Not supported.</span></span>|
|<span data-ttu-id="abff4-116">Application</span><span class="sxs-lookup"><span data-stu-id="abff4-116">Application</span></span>|<span data-ttu-id="abff4-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abff4-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="abff4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="abff4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="abff4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="abff4-119">Request headers</span></span>
|<span data-ttu-id="abff4-120">标头</span><span class="sxs-lookup"><span data-stu-id="abff4-120">Header</span></span>|<span data-ttu-id="abff4-121">值</span><span class="sxs-lookup"><span data-stu-id="abff4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abff4-122">授权</span><span class="sxs-lookup"><span data-stu-id="abff4-122">Authorization</span></span>|<span data-ttu-id="abff4-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="abff4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abff4-124">接受</span><span class="sxs-lookup"><span data-stu-id="abff4-124">Accept</span></span>|<span data-ttu-id="abff4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="abff4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abff4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="abff4-126">Request body</span></span>
<span data-ttu-id="abff4-127">在请求正文中，提供[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="abff4-127">In the request body, supply a JSON representation for the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

<span data-ttu-id="abff4-128">下表显示创建[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="abff4-128">The following table shows the properties that are required when you create the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span></span>

|<span data-ttu-id="abff4-129">属性</span><span class="sxs-lookup"><span data-stu-id="abff4-129">Property</span></span>|<span data-ttu-id="abff4-130">类型</span><span class="sxs-lookup"><span data-stu-id="abff4-130">Type</span></span>|<span data-ttu-id="abff4-131">说明</span><span class="sxs-lookup"><span data-stu-id="abff4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abff4-132">id</span><span class="sxs-lookup"><span data-stu-id="abff4-132">id</span></span>|<span data-ttu-id="abff4-133">字符串</span><span class="sxs-lookup"><span data-stu-id="abff4-133">String</span></span>|<span data-ttu-id="abff4-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="abff4-134">Key of the entity.</span></span>|
|<span data-ttu-id="abff4-135">target</span><span class="sxs-lookup"><span data-stu-id="abff4-135">target</span></span>|[<span data-ttu-id="abff4-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="abff4-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="abff4-137">特定角色范围标记的自动分配目标。</span><span class="sxs-lookup"><span data-stu-id="abff4-137">The auto-assignment target for the specific Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="abff4-138">响应</span><span class="sxs-lookup"><span data-stu-id="abff4-138">Response</span></span>
<span data-ttu-id="abff4-139">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="abff4-139">If successful, this method returns a `200 OK` response code and an updated [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abff4-140">示例</span><span class="sxs-lookup"><span data-stu-id="abff4-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="abff4-141">请求</span><span class="sxs-lookup"><span data-stu-id="abff4-141">Request</span></span>
<span data-ttu-id="abff4-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="abff4-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
Content-type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="abff4-143">响应</span><span class="sxs-lookup"><span data-stu-id="abff4-143">Response</span></span>
<span data-ttu-id="abff4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="abff4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "id": "256e6375-6375-256e-7563-6e2575636e25",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





