---
title: 创建 roleScopeTagAutoAssignment
description: 创建新的 roleScopeTagAutoAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 400a1db04487936d1558b677f7363228b44fb6ca
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178050"
---
# <a name="create-rolescopetagautoassignment"></a><span data-ttu-id="17f33-103">创建 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="17f33-103">Create roleScopeTagAutoAssignment</span></span>

<span data-ttu-id="17f33-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17f33-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17f33-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="17f33-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17f33-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="17f33-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17f33-107">创建新的[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="17f33-107">Create a new [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17f33-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="17f33-108">Prerequisites</span></span>
<span data-ttu-id="17f33-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17f33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17f33-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="17f33-111">Permission type</span></span>|<span data-ttu-id="17f33-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="17f33-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17f33-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17f33-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17f33-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17f33-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="17f33-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17f33-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17f33-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="17f33-116">Not supported.</span></span>|
|<span data-ttu-id="17f33-117">Application</span><span class="sxs-lookup"><span data-stu-id="17f33-117">Application</span></span>|<span data-ttu-id="17f33-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17f33-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17f33-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17f33-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="17f33-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="17f33-120">Request headers</span></span>
|<span data-ttu-id="17f33-121">标头</span><span class="sxs-lookup"><span data-stu-id="17f33-121">Header</span></span>|<span data-ttu-id="17f33-122">值</span><span class="sxs-lookup"><span data-stu-id="17f33-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17f33-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="17f33-123">Authorization</span></span>|<span data-ttu-id="17f33-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="17f33-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17f33-125">接受</span><span class="sxs-lookup"><span data-stu-id="17f33-125">Accept</span></span>|<span data-ttu-id="17f33-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17f33-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17f33-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="17f33-127">Request body</span></span>
<span data-ttu-id="17f33-128">在请求正文中，提供 roleScopeTagAutoAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17f33-128">In the request body, supply a JSON representation for the roleScopeTagAutoAssignment object.</span></span>

<span data-ttu-id="17f33-129">下表显示创建 roleScopeTagAutoAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="17f33-129">The following table shows the properties that are required when you create the roleScopeTagAutoAssignment.</span></span>

|<span data-ttu-id="17f33-130">属性</span><span class="sxs-lookup"><span data-stu-id="17f33-130">Property</span></span>|<span data-ttu-id="17f33-131">类型</span><span class="sxs-lookup"><span data-stu-id="17f33-131">Type</span></span>|<span data-ttu-id="17f33-132">说明</span><span class="sxs-lookup"><span data-stu-id="17f33-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17f33-133">id</span><span class="sxs-lookup"><span data-stu-id="17f33-133">id</span></span>|<span data-ttu-id="17f33-134">字符串</span><span class="sxs-lookup"><span data-stu-id="17f33-134">String</span></span>|<span data-ttu-id="17f33-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="17f33-135">Key of the entity.</span></span>|
|<span data-ttu-id="17f33-136">target</span><span class="sxs-lookup"><span data-stu-id="17f33-136">target</span></span>|[<span data-ttu-id="17f33-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="17f33-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="17f33-138">特定角色范围标记的自动分配目标。</span><span class="sxs-lookup"><span data-stu-id="17f33-138">The auto-assignment target for the specific Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="17f33-139">响应</span><span class="sxs-lookup"><span data-stu-id="17f33-139">Response</span></span>
<span data-ttu-id="17f33-140">如果成功，此方法在响应`201 Created`正文中返回响应代码和[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="17f33-140">If successful, this method returns a `201 Created` response code and a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17f33-141">示例</span><span class="sxs-lookup"><span data-stu-id="17f33-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="17f33-142">请求</span><span class="sxs-lookup"><span data-stu-id="17f33-142">Request</span></span>
<span data-ttu-id="17f33-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="17f33-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
Content-type: application/json
Content-length: 154

{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="17f33-144">响应</span><span class="sxs-lookup"><span data-stu-id="17f33-144">Response</span></span>
<span data-ttu-id="17f33-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="17f33-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 203

{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "id": "256e6375-6375-256e-7563-6e2575636e25",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  }
}
```



