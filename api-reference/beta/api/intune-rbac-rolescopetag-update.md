---
title: 更新 roleScopeTag
description: 更新 roleScopeTag 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1dd417be2450f7cc956f6e6c4c7c39f9f748be2d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955124"
---
# <a name="update-rolescopetag"></a><span data-ttu-id="979a3-103">更新 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="979a3-103">Update roleScopeTag</span></span>

> <span data-ttu-id="979a3-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="979a3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="979a3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="979a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="979a3-106">更新[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="979a3-106">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="979a3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="979a3-107">Prerequisites</span></span>
<span data-ttu-id="979a3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="979a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="979a3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="979a3-110">Permission type</span></span>|<span data-ttu-id="979a3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="979a3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="979a3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="979a3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="979a3-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="979a3-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="979a3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="979a3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="979a3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="979a3-115">Not supported.</span></span>|
|<span data-ttu-id="979a3-116">Application</span><span class="sxs-lookup"><span data-stu-id="979a3-116">Application</span></span>|<span data-ttu-id="979a3-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="979a3-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="979a3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="979a3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleScopeTags/{roleScopeTagId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="request-headers"></a><span data-ttu-id="979a3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="979a3-119">Request headers</span></span>
|<span data-ttu-id="979a3-120">标头</span><span class="sxs-lookup"><span data-stu-id="979a3-120">Header</span></span>|<span data-ttu-id="979a3-121">值</span><span class="sxs-lookup"><span data-stu-id="979a3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="979a3-122">授权</span><span class="sxs-lookup"><span data-stu-id="979a3-122">Authorization</span></span>|<span data-ttu-id="979a3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="979a3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="979a3-124">接受</span><span class="sxs-lookup"><span data-stu-id="979a3-124">Accept</span></span>|<span data-ttu-id="979a3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="979a3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="979a3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="979a3-126">Request body</span></span>
<span data-ttu-id="979a3-127">在请求正文中，提供[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="979a3-127">In the request body, supply a JSON representation for the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

<span data-ttu-id="979a3-128">下表显示创建[roleScopeTag](../resources/intune-rbac-rolescopetag.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="979a3-128">The following table shows the properties that are required when you create the [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>

|<span data-ttu-id="979a3-129">属性</span><span class="sxs-lookup"><span data-stu-id="979a3-129">Property</span></span>|<span data-ttu-id="979a3-130">类型</span><span class="sxs-lookup"><span data-stu-id="979a3-130">Type</span></span>|<span data-ttu-id="979a3-131">说明</span><span class="sxs-lookup"><span data-stu-id="979a3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="979a3-132">id</span><span class="sxs-lookup"><span data-stu-id="979a3-132">id</span></span>|<span data-ttu-id="979a3-133">字符串</span><span class="sxs-lookup"><span data-stu-id="979a3-133">String</span></span>|<span data-ttu-id="979a3-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="979a3-134">Key of the entity.</span></span> <span data-ttu-id="979a3-135">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="979a3-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="979a3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="979a3-136">displayName</span></span>|<span data-ttu-id="979a3-137">String</span><span class="sxs-lookup"><span data-stu-id="979a3-137">String</span></span>|<span data-ttu-id="979a3-138">角色范围标记的显示名称或友好名称。</span><span class="sxs-lookup"><span data-stu-id="979a3-138">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="979a3-139">说明</span><span class="sxs-lookup"><span data-stu-id="979a3-139">description</span></span>|<span data-ttu-id="979a3-140">String</span><span class="sxs-lookup"><span data-stu-id="979a3-140">String</span></span>|<span data-ttu-id="979a3-141">角色范围标记的说明。</span><span class="sxs-lookup"><span data-stu-id="979a3-141">Description of the Role Scope Tag.</span></span>|
|<span data-ttu-id="979a3-142">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="979a3-142">isBuiltIn</span></span>|<span data-ttu-id="979a3-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="979a3-143">Boolean</span></span>|<span data-ttu-id="979a3-144">角色范围标记的说明。</span><span class="sxs-lookup"><span data-stu-id="979a3-144">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="979a3-145">响应</span><span class="sxs-lookup"><span data-stu-id="979a3-145">Response</span></span>
<span data-ttu-id="979a3-146">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象。</span><span class="sxs-lookup"><span data-stu-id="979a3-146">If successful, this method returns a `200 OK` response code and an updated [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="979a3-147">示例</span><span class="sxs-lookup"><span data-stu-id="979a3-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="979a3-148">请求</span><span class="sxs-lookup"><span data-stu-id="979a3-148">Request</span></span>
<span data-ttu-id="979a3-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="979a3-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}
Content-type: application/json
Content-length: 155

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "displayName": "Display Name value",
  "description": "Description value",
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="979a3-150">响应</span><span class="sxs-lookup"><span data-stu-id="979a3-150">Response</span></span>
<span data-ttu-id="979a3-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="979a3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





