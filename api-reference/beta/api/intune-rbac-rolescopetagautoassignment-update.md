---
title: 更新 roleScopeTagAutoAssignment
description: 更新 roleScopeTagAutoAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0860d28f77fcdadec1537e57ce1852ae20c8863a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49304467"
---
# <a name="update-rolescopetagautoassignment"></a><span data-ttu-id="8c500-103">更新 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="8c500-103">Update roleScopeTagAutoAssignment</span></span>

<span data-ttu-id="8c500-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c500-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c500-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8c500-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c500-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c500-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c500-107">更新 [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8c500-107">Update the properties of a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c500-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8c500-108">Prerequisites</span></span>
<span data-ttu-id="8c500-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c500-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c500-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c500-111">Permission type</span></span>|<span data-ttu-id="8c500-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8c500-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c500-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c500-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c500-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c500-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="8c500-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c500-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c500-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c500-116">Not supported.</span></span>|
|<span data-ttu-id="8c500-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c500-117">Application</span></span>|<span data-ttu-id="8c500-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c500-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c500-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c500-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="8c500-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c500-120">Request headers</span></span>
|<span data-ttu-id="8c500-121">标头</span><span class="sxs-lookup"><span data-stu-id="8c500-121">Header</span></span>|<span data-ttu-id="8c500-122">值</span><span class="sxs-lookup"><span data-stu-id="8c500-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c500-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c500-123">Authorization</span></span>|<span data-ttu-id="8c500-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8c500-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c500-125">接受</span><span class="sxs-lookup"><span data-stu-id="8c500-125">Accept</span></span>|<span data-ttu-id="8c500-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c500-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c500-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c500-127">Request body</span></span>
<span data-ttu-id="8c500-128">在请求正文中，提供 [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c500-128">In the request body, supply a JSON representation for the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

<span data-ttu-id="8c500-129">下表显示创建 [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8c500-129">The following table shows the properties that are required when you create the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span></span>

|<span data-ttu-id="8c500-130">属性</span><span class="sxs-lookup"><span data-stu-id="8c500-130">Property</span></span>|<span data-ttu-id="8c500-131">类型</span><span class="sxs-lookup"><span data-stu-id="8c500-131">Type</span></span>|<span data-ttu-id="8c500-132">说明</span><span class="sxs-lookup"><span data-stu-id="8c500-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c500-133">id</span><span class="sxs-lookup"><span data-stu-id="8c500-133">id</span></span>|<span data-ttu-id="8c500-134">字符串</span><span class="sxs-lookup"><span data-stu-id="8c500-134">String</span></span>|<span data-ttu-id="8c500-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8c500-135">Key of the entity.</span></span>|
|<span data-ttu-id="8c500-136">target</span><span class="sxs-lookup"><span data-stu-id="8c500-136">target</span></span>|[<span data-ttu-id="8c500-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8c500-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8c500-138">特定角色范围标记的自动分配目标。</span><span class="sxs-lookup"><span data-stu-id="8c500-138">The auto-assignment target for the specific Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="8c500-139">响应</span><span class="sxs-lookup"><span data-stu-id="8c500-139">Response</span></span>
<span data-ttu-id="8c500-140">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8c500-140">If successful, this method returns a `200 OK` response code and an updated [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c500-141">示例</span><span class="sxs-lookup"><span data-stu-id="8c500-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c500-142">请求</span><span class="sxs-lookup"><span data-stu-id="8c500-142">Request</span></span>
<span data-ttu-id="8c500-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8c500-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments/{roleScopeTagAutoAssignmentId}
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

### <a name="response"></a><span data-ttu-id="8c500-144">响应</span><span class="sxs-lookup"><span data-stu-id="8c500-144">Response</span></span>
<span data-ttu-id="8c500-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8c500-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




