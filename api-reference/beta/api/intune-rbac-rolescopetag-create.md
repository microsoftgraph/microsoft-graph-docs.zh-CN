---
title: 创建 roleScopeTag
description: 创建新的 roleScopeTag 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c17eebbcdff6ee9f466568baa8ace0825c73771d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154234"
---
# <a name="create-rolescopetag"></a><span data-ttu-id="5f94d-103">创建 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="5f94d-103">Create roleScopeTag</span></span>

> <span data-ttu-id="5f94d-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5f94d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f94d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5f94d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f94d-106">创建新的[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5f94d-106">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f94d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5f94d-107">Prerequisites</span></span>
<span data-ttu-id="5f94d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5f94d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5f94d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f94d-110">Permission type</span></span>|<span data-ttu-id="5f94d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5f94d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f94d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f94d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5f94d-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f94d-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="5f94d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f94d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f94d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f94d-115">Not supported.</span></span>|
|<span data-ttu-id="5f94d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f94d-116">Application</span></span>|<span data-ttu-id="5f94d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f94d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f94d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f94d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="5f94d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f94d-119">Request headers</span></span>
|<span data-ttu-id="5f94d-120">标头</span><span class="sxs-lookup"><span data-stu-id="5f94d-120">Header</span></span>|<span data-ttu-id="5f94d-121">值</span><span class="sxs-lookup"><span data-stu-id="5f94d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f94d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f94d-122">Authorization</span></span>|<span data-ttu-id="5f94d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5f94d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f94d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5f94d-124">Accept</span></span>|<span data-ttu-id="5f94d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5f94d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f94d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f94d-126">Request body</span></span>
<span data-ttu-id="5f94d-127">在请求正文中, 提供 roleScopeTag 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f94d-127">In the request body, supply a JSON representation for the roleScopeTag object.</span></span>

<span data-ttu-id="5f94d-128">下表显示创建 roleScopeTag 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5f94d-128">The following table shows the properties that are required when you create the roleScopeTag.</span></span>

|<span data-ttu-id="5f94d-129">属性</span><span class="sxs-lookup"><span data-stu-id="5f94d-129">Property</span></span>|<span data-ttu-id="5f94d-130">类型</span><span class="sxs-lookup"><span data-stu-id="5f94d-130">Type</span></span>|<span data-ttu-id="5f94d-131">说明</span><span class="sxs-lookup"><span data-stu-id="5f94d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f94d-132">id</span><span class="sxs-lookup"><span data-stu-id="5f94d-132">id</span></span>|<span data-ttu-id="5f94d-133">String</span><span class="sxs-lookup"><span data-stu-id="5f94d-133">String</span></span>|<span data-ttu-id="5f94d-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5f94d-134">Key of the entity.</span></span> <span data-ttu-id="5f94d-135">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="5f94d-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="5f94d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5f94d-136">displayName</span></span>|<span data-ttu-id="5f94d-137">String</span><span class="sxs-lookup"><span data-stu-id="5f94d-137">String</span></span>|<span data-ttu-id="5f94d-138">角色范围标记的显示名称或友好名称。</span><span class="sxs-lookup"><span data-stu-id="5f94d-138">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="5f94d-139">说明</span><span class="sxs-lookup"><span data-stu-id="5f94d-139">description</span></span>|<span data-ttu-id="5f94d-140">String</span><span class="sxs-lookup"><span data-stu-id="5f94d-140">String</span></span>|<span data-ttu-id="5f94d-141">角色范围标记的说明。</span><span class="sxs-lookup"><span data-stu-id="5f94d-141">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="5f94d-142">响应</span><span class="sxs-lookup"><span data-stu-id="5f94d-142">Response</span></span>
<span data-ttu-id="5f94d-143">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5f94d-143">If successful, this method returns a `201 Created` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f94d-144">示例</span><span class="sxs-lookup"><span data-stu-id="5f94d-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f94d-145">请求</span><span class="sxs-lookup"><span data-stu-id="5f94d-145">Request</span></span>
<span data-ttu-id="5f94d-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5f94d-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags
Content-type: application/json
Content-length: 133

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="5f94d-147">响应</span><span class="sxs-lookup"><span data-stu-id="5f94d-147">Response</span></span>
<span data-ttu-id="5f94d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5f94d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 182

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
  "displayName": "Display Name value",
  "description": "Description value"
}
```




