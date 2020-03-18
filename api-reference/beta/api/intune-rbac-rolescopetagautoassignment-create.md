---
title: 创建 roleScopeTagAutoAssignment
description: 创建新的 roleScopeTagAutoAssignment 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 46f6e41fb9cdd461ad5fcfe6cd55552618f004ed
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801556"
---
# <a name="create-rolescopetagautoassignment"></a><span data-ttu-id="593da-103">创建 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="593da-103">Create roleScopeTagAutoAssignment</span></span>

> <span data-ttu-id="593da-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="593da-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="593da-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="593da-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="593da-106">创建新的[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="593da-106">Create a new [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="593da-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="593da-107">Prerequisites</span></span>
<span data-ttu-id="593da-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="593da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="593da-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="593da-110">Permission type</span></span>|<span data-ttu-id="593da-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="593da-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="593da-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="593da-112">Delegated (work or school account)</span></span>|<span data-ttu-id="593da-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="593da-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="593da-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="593da-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="593da-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="593da-115">Not supported.</span></span>|
|<span data-ttu-id="593da-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="593da-116">Application</span></span>|<span data-ttu-id="593da-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="593da-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="593da-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="593da-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="593da-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="593da-119">Request headers</span></span>
|<span data-ttu-id="593da-120">标头</span><span class="sxs-lookup"><span data-stu-id="593da-120">Header</span></span>|<span data-ttu-id="593da-121">值</span><span class="sxs-lookup"><span data-stu-id="593da-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="593da-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="593da-122">Authorization</span></span>|<span data-ttu-id="593da-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="593da-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="593da-124">接受</span><span class="sxs-lookup"><span data-stu-id="593da-124">Accept</span></span>|<span data-ttu-id="593da-125">application/json</span><span class="sxs-lookup"><span data-stu-id="593da-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="593da-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="593da-126">Request body</span></span>
<span data-ttu-id="593da-127">在请求正文中，提供 roleScopeTagAutoAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="593da-127">In the request body, supply a JSON representation for the roleScopeTagAutoAssignment object.</span></span>

<span data-ttu-id="593da-128">下表显示创建 roleScopeTagAutoAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="593da-128">The following table shows the properties that are required when you create the roleScopeTagAutoAssignment.</span></span>

|<span data-ttu-id="593da-129">属性</span><span class="sxs-lookup"><span data-stu-id="593da-129">Property</span></span>|<span data-ttu-id="593da-130">类型</span><span class="sxs-lookup"><span data-stu-id="593da-130">Type</span></span>|<span data-ttu-id="593da-131">说明</span><span class="sxs-lookup"><span data-stu-id="593da-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="593da-132">id</span><span class="sxs-lookup"><span data-stu-id="593da-132">id</span></span>|<span data-ttu-id="593da-133">String</span><span class="sxs-lookup"><span data-stu-id="593da-133">String</span></span>|<span data-ttu-id="593da-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="593da-134">Key of the entity.</span></span>|
|<span data-ttu-id="593da-135">target</span><span class="sxs-lookup"><span data-stu-id="593da-135">target</span></span>|[<span data-ttu-id="593da-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="593da-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="593da-137">特定角色范围标记的自动分配目标。</span><span class="sxs-lookup"><span data-stu-id="593da-137">The auto-assignment target for the specific Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="593da-138">响应</span><span class="sxs-lookup"><span data-stu-id="593da-138">Response</span></span>
<span data-ttu-id="593da-139">如果成功，此方法在响应`201 Created`正文中返回响应代码和[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="593da-139">If successful, this method returns a `201 Created` response code and a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="593da-140">示例</span><span class="sxs-lookup"><span data-stu-id="593da-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="593da-141">请求</span><span class="sxs-lookup"><span data-stu-id="593da-141">Request</span></span>
<span data-ttu-id="593da-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="593da-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
Content-type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="593da-143">响应</span><span class="sxs-lookup"><span data-stu-id="593da-143">Response</span></span>
<span data-ttu-id="593da-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="593da-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




