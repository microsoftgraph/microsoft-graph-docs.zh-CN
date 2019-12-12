---
title: 创建 roleScopeTagAutoAssignment
description: 创建新的 roleScopeTagAutoAssignment 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 507b04989f6d5bc431e4aa2439800c127771f33e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955201"
---
# <a name="create-rolescopetagautoassignment"></a><span data-ttu-id="42c81-103">创建 roleScopeTagAutoAssignment</span><span class="sxs-lookup"><span data-stu-id="42c81-103">Create roleScopeTagAutoAssignment</span></span>

> <span data-ttu-id="42c81-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="42c81-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42c81-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="42c81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42c81-106">创建新的[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="42c81-106">Create a new [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42c81-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="42c81-107">Prerequisites</span></span>
<span data-ttu-id="42c81-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="42c81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42c81-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="42c81-110">Permission type</span></span>|<span data-ttu-id="42c81-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="42c81-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42c81-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="42c81-112">Delegated (work or school account)</span></span>|<span data-ttu-id="42c81-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42c81-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="42c81-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="42c81-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42c81-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="42c81-115">Not supported.</span></span>|
|<span data-ttu-id="42c81-116">Application</span><span class="sxs-lookup"><span data-stu-id="42c81-116">Application</span></span>|<span data-ttu-id="42c81-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42c81-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42c81-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="42c81-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="42c81-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="42c81-119">Request headers</span></span>
|<span data-ttu-id="42c81-120">标头</span><span class="sxs-lookup"><span data-stu-id="42c81-120">Header</span></span>|<span data-ttu-id="42c81-121">值</span><span class="sxs-lookup"><span data-stu-id="42c81-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42c81-122">授权</span><span class="sxs-lookup"><span data-stu-id="42c81-122">Authorization</span></span>|<span data-ttu-id="42c81-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="42c81-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42c81-124">接受</span><span class="sxs-lookup"><span data-stu-id="42c81-124">Accept</span></span>|<span data-ttu-id="42c81-125">application/json</span><span class="sxs-lookup"><span data-stu-id="42c81-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42c81-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="42c81-126">Request body</span></span>
<span data-ttu-id="42c81-127">在请求正文中，提供 roleScopeTagAutoAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42c81-127">In the request body, supply a JSON representation for the roleScopeTagAutoAssignment object.</span></span>

<span data-ttu-id="42c81-128">下表显示创建 roleScopeTagAutoAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="42c81-128">The following table shows the properties that are required when you create the roleScopeTagAutoAssignment.</span></span>

|<span data-ttu-id="42c81-129">属性</span><span class="sxs-lookup"><span data-stu-id="42c81-129">Property</span></span>|<span data-ttu-id="42c81-130">类型</span><span class="sxs-lookup"><span data-stu-id="42c81-130">Type</span></span>|<span data-ttu-id="42c81-131">说明</span><span class="sxs-lookup"><span data-stu-id="42c81-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42c81-132">id</span><span class="sxs-lookup"><span data-stu-id="42c81-132">id</span></span>|<span data-ttu-id="42c81-133">字符串</span><span class="sxs-lookup"><span data-stu-id="42c81-133">String</span></span>|<span data-ttu-id="42c81-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="42c81-134">Key of the entity.</span></span>|
|<span data-ttu-id="42c81-135">target</span><span class="sxs-lookup"><span data-stu-id="42c81-135">target</span></span>|[<span data-ttu-id="42c81-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="42c81-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="42c81-137">特定角色范围标记的自动分配目标。</span><span class="sxs-lookup"><span data-stu-id="42c81-137">The auto-assignment target for the specific Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="42c81-138">响应</span><span class="sxs-lookup"><span data-stu-id="42c81-138">Response</span></span>
<span data-ttu-id="42c81-139">如果成功，此方法在响应`201 Created`正文中返回响应代码和[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="42c81-139">If successful, this method returns a `201 Created` response code and a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42c81-140">示例</span><span class="sxs-lookup"><span data-stu-id="42c81-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="42c81-141">请求</span><span class="sxs-lookup"><span data-stu-id="42c81-141">Request</span></span>
<span data-ttu-id="42c81-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="42c81-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="42c81-143">响应</span><span class="sxs-lookup"><span data-stu-id="42c81-143">Response</span></span>
<span data-ttu-id="42c81-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="42c81-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





