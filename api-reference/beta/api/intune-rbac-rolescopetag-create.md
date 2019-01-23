---
title: 创建 roleScopeTag
description: 创建新的 roleScopeTag 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 61476fa106661baa179ff5344b8e4ac891b5a3b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422192"
---
# <a name="create-rolescopetag"></a><span data-ttu-id="29e2b-103">创建 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="29e2b-103">Create roleScopeTag</span></span>

> <span data-ttu-id="29e2b-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="29e2b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="29e2b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="29e2b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29e2b-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="29e2b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29e2b-107">创建新的[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象。</span><span class="sxs-lookup"><span data-stu-id="29e2b-107">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29e2b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="29e2b-108">Prerequisites</span></span>
<span data-ttu-id="29e2b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="29e2b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="29e2b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="29e2b-111">Permission type</span></span>|<span data-ttu-id="29e2b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="29e2b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29e2b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29e2b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29e2b-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29e2b-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="29e2b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29e2b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29e2b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="29e2b-116">Not supported.</span></span>|
|<span data-ttu-id="29e2b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="29e2b-117">Application</span></span>|<span data-ttu-id="29e2b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="29e2b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29e2b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29e2b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="29e2b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="29e2b-120">Request headers</span></span>
|<span data-ttu-id="29e2b-121">标头</span><span class="sxs-lookup"><span data-stu-id="29e2b-121">Header</span></span>|<span data-ttu-id="29e2b-122">值</span><span class="sxs-lookup"><span data-stu-id="29e2b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29e2b-123">授权</span><span class="sxs-lookup"><span data-stu-id="29e2b-123">Authorization</span></span>|<span data-ttu-id="29e2b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="29e2b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29e2b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="29e2b-125">Accept</span></span>|<span data-ttu-id="29e2b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29e2b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29e2b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="29e2b-127">Request body</span></span>
<span data-ttu-id="29e2b-128">在请求正文中，提供 roleScopeTag 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29e2b-128">In the request body, supply a JSON representation for the roleScopeTag object.</span></span>

<span data-ttu-id="29e2b-129">下表显示时创建 roleScopeTag 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="29e2b-129">The following table shows the properties that are required when you create the roleScopeTag.</span></span>

|<span data-ttu-id="29e2b-130">属性</span><span class="sxs-lookup"><span data-stu-id="29e2b-130">Property</span></span>|<span data-ttu-id="29e2b-131">类型</span><span class="sxs-lookup"><span data-stu-id="29e2b-131">Type</span></span>|<span data-ttu-id="29e2b-132">说明</span><span class="sxs-lookup"><span data-stu-id="29e2b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29e2b-133">id</span><span class="sxs-lookup"><span data-stu-id="29e2b-133">id</span></span>|<span data-ttu-id="29e2b-134">String</span><span class="sxs-lookup"><span data-stu-id="29e2b-134">String</span></span>|<span data-ttu-id="29e2b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="29e2b-135">Key of the entity.</span></span> <span data-ttu-id="29e2b-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="29e2b-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="29e2b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="29e2b-137">displayName</span></span>|<span data-ttu-id="29e2b-138">String</span><span class="sxs-lookup"><span data-stu-id="29e2b-138">String</span></span>|<span data-ttu-id="29e2b-139">显示或角色作用域标记的友好名称。</span><span class="sxs-lookup"><span data-stu-id="29e2b-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="29e2b-140">说明</span><span class="sxs-lookup"><span data-stu-id="29e2b-140">description</span></span>|<span data-ttu-id="29e2b-141">String</span><span class="sxs-lookup"><span data-stu-id="29e2b-141">String</span></span>|<span data-ttu-id="29e2b-142">角色作用域标记的说明。</span><span class="sxs-lookup"><span data-stu-id="29e2b-142">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="29e2b-143">响应</span><span class="sxs-lookup"><span data-stu-id="29e2b-143">Response</span></span>
<span data-ttu-id="29e2b-144">如果成功，此方法返回`201 Created`响应代码和响应正文中的[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象。</span><span class="sxs-lookup"><span data-stu-id="29e2b-144">If successful, this method returns a `201 Created` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29e2b-145">示例</span><span class="sxs-lookup"><span data-stu-id="29e2b-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="29e2b-146">请求</span><span class="sxs-lookup"><span data-stu-id="29e2b-146">Request</span></span>
<span data-ttu-id="29e2b-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="29e2b-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="29e2b-148">响应</span><span class="sxs-lookup"><span data-stu-id="29e2b-148">Response</span></span>
<span data-ttu-id="29e2b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="29e2b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




