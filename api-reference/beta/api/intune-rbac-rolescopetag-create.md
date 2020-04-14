---
title: 创建 roleScopeTag
description: 创建新的 roleScopeTag 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a705d41ce2e10a07dfb43e86dd662adbce3f837c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43360630"
---
# <a name="create-rolescopetag"></a><span data-ttu-id="d3c32-103">创建 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="d3c32-103">Create roleScopeTag</span></span>

<span data-ttu-id="d3c32-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3c32-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3c32-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d3c32-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3c32-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3c32-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3c32-107">创建新的[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d3c32-107">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3c32-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d3c32-108">Prerequisites</span></span>
<span data-ttu-id="d3c32-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3c32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3c32-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3c32-111">Permission type</span></span>|<span data-ttu-id="d3c32-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d3c32-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3c32-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3c32-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3c32-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3c32-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="d3c32-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3c32-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3c32-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3c32-116">Not supported.</span></span>|
|<span data-ttu-id="d3c32-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3c32-117">Application</span></span>|<span data-ttu-id="d3c32-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3c32-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3c32-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3c32-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="d3c32-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3c32-120">Request headers</span></span>
|<span data-ttu-id="d3c32-121">标头</span><span class="sxs-lookup"><span data-stu-id="d3c32-121">Header</span></span>|<span data-ttu-id="d3c32-122">值</span><span class="sxs-lookup"><span data-stu-id="d3c32-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3c32-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3c32-123">Authorization</span></span>|<span data-ttu-id="d3c32-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d3c32-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3c32-125">接受</span><span class="sxs-lookup"><span data-stu-id="d3c32-125">Accept</span></span>|<span data-ttu-id="d3c32-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3c32-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3c32-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3c32-127">Request body</span></span>
<span data-ttu-id="d3c32-128">在请求正文中，提供 roleScopeTag 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3c32-128">In the request body, supply a JSON representation for the roleScopeTag object.</span></span>

<span data-ttu-id="d3c32-129">下表显示创建 roleScopeTag 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d3c32-129">The following table shows the properties that are required when you create the roleScopeTag.</span></span>

|<span data-ttu-id="d3c32-130">属性</span><span class="sxs-lookup"><span data-stu-id="d3c32-130">Property</span></span>|<span data-ttu-id="d3c32-131">类型</span><span class="sxs-lookup"><span data-stu-id="d3c32-131">Type</span></span>|<span data-ttu-id="d3c32-132">说明</span><span class="sxs-lookup"><span data-stu-id="d3c32-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3c32-133">id</span><span class="sxs-lookup"><span data-stu-id="d3c32-133">id</span></span>|<span data-ttu-id="d3c32-134">字符串</span><span class="sxs-lookup"><span data-stu-id="d3c32-134">String</span></span>|<span data-ttu-id="d3c32-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d3c32-135">Key of the entity.</span></span> <span data-ttu-id="d3c32-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="d3c32-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="d3c32-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d3c32-137">displayName</span></span>|<span data-ttu-id="d3c32-138">String</span><span class="sxs-lookup"><span data-stu-id="d3c32-138">String</span></span>|<span data-ttu-id="d3c32-139">角色范围标记的显示名称或友好名称。</span><span class="sxs-lookup"><span data-stu-id="d3c32-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="d3c32-140">description</span><span class="sxs-lookup"><span data-stu-id="d3c32-140">description</span></span>|<span data-ttu-id="d3c32-141">String</span><span class="sxs-lookup"><span data-stu-id="d3c32-141">String</span></span>|<span data-ttu-id="d3c32-142">角色范围标记的说明。</span><span class="sxs-lookup"><span data-stu-id="d3c32-142">Description of the Role Scope Tag.</span></span>|
|<span data-ttu-id="d3c32-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="d3c32-143">isBuiltIn</span></span>|<span data-ttu-id="d3c32-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3c32-144">Boolean</span></span>|<span data-ttu-id="d3c32-145">角色范围标记的说明。</span><span class="sxs-lookup"><span data-stu-id="d3c32-145">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="d3c32-146">响应</span><span class="sxs-lookup"><span data-stu-id="d3c32-146">Response</span></span>
<span data-ttu-id="d3c32-147">如果成功，此方法在响应`201 Created`正文中返回响应代码和[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d3c32-147">If successful, this method returns a `201 Created` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3c32-148">示例</span><span class="sxs-lookup"><span data-stu-id="d3c32-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3c32-149">请求</span><span class="sxs-lookup"><span data-stu-id="d3c32-149">Request</span></span>
<span data-ttu-id="d3c32-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d3c32-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags
Content-type: application/json
Content-length: 155

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "displayName": "Display Name value",
  "description": "Description value",
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="d3c32-151">响应</span><span class="sxs-lookup"><span data-stu-id="d3c32-151">Response</span></span>
<span data-ttu-id="d3c32-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d3c32-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 204

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
  "displayName": "Display Name value",
  "description": "Description value",
  "isBuiltIn": true
}
```



