---
title: 更新 roleScopeTag
description: 更新 roleScopeTag 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6b05ba0be4e91bd9f4cb39ae316048f1f85194ab
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404811"
---
# <a name="update-rolescopetag"></a><span data-ttu-id="5f985-103">更新 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="5f985-103">Update roleScopeTag</span></span>

> <span data-ttu-id="5f985-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="5f985-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5f985-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5f985-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f985-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5f985-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f985-107">更新[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5f985-107">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f985-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5f985-108">Prerequisites</span></span>
<span data-ttu-id="5f985-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5f985-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5f985-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f985-111">Permission type</span></span>|<span data-ttu-id="5f985-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5f985-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f985-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f985-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5f985-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f985-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="5f985-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f985-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f985-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f985-116">Not supported.</span></span>|
|<span data-ttu-id="5f985-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f985-117">Application</span></span>|<span data-ttu-id="5f985-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f985-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f985-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f985-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleScopeTags/{roleScopeTagId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="request-headers"></a><span data-ttu-id="5f985-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f985-120">Request headers</span></span>
|<span data-ttu-id="5f985-121">标头</span><span class="sxs-lookup"><span data-stu-id="5f985-121">Header</span></span>|<span data-ttu-id="5f985-122">值</span><span class="sxs-lookup"><span data-stu-id="5f985-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f985-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f985-123">Authorization</span></span>|<span data-ttu-id="5f985-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5f985-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f985-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5f985-125">Accept</span></span>|<span data-ttu-id="5f985-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5f985-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f985-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f985-127">Request body</span></span>
<span data-ttu-id="5f985-128">在请求正文中，提供[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f985-128">In the request body, supply a JSON representation for the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

<span data-ttu-id="5f985-129">下表显示时创建[roleScopeTag](../resources/intune-rbac-rolescopetag.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5f985-129">The following table shows the properties that are required when you create the [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>

|<span data-ttu-id="5f985-130">属性</span><span class="sxs-lookup"><span data-stu-id="5f985-130">Property</span></span>|<span data-ttu-id="5f985-131">类型</span><span class="sxs-lookup"><span data-stu-id="5f985-131">Type</span></span>|<span data-ttu-id="5f985-132">说明</span><span class="sxs-lookup"><span data-stu-id="5f985-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f985-133">id</span><span class="sxs-lookup"><span data-stu-id="5f985-133">id</span></span>|<span data-ttu-id="5f985-134">String</span><span class="sxs-lookup"><span data-stu-id="5f985-134">String</span></span>|<span data-ttu-id="5f985-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5f985-135">Key of the entity.</span></span> <span data-ttu-id="5f985-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="5f985-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="5f985-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5f985-137">displayName</span></span>|<span data-ttu-id="5f985-138">String</span><span class="sxs-lookup"><span data-stu-id="5f985-138">String</span></span>|<span data-ttu-id="5f985-139">显示或角色作用域标记的友好名称。</span><span class="sxs-lookup"><span data-stu-id="5f985-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="5f985-140">说明</span><span class="sxs-lookup"><span data-stu-id="5f985-140">description</span></span>|<span data-ttu-id="5f985-141">String</span><span class="sxs-lookup"><span data-stu-id="5f985-141">String</span></span>|<span data-ttu-id="5f985-142">角色作用域标记的说明。</span><span class="sxs-lookup"><span data-stu-id="5f985-142">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="5f985-143">响应</span><span class="sxs-lookup"><span data-stu-id="5f985-143">Response</span></span>
<span data-ttu-id="5f985-144">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5f985-144">If successful, this method returns a `200 OK` response code and an updated [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f985-145">示例</span><span class="sxs-lookup"><span data-stu-id="5f985-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f985-146">请求</span><span class="sxs-lookup"><span data-stu-id="5f985-146">Request</span></span>
<span data-ttu-id="5f985-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5f985-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}
Content-type: application/json
Content-length: 133

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="5f985-148">响应</span><span class="sxs-lookup"><span data-stu-id="5f985-148">Response</span></span>
<span data-ttu-id="5f985-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5f985-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 182

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
  "displayName": "Display Name value",
  "description": "Description value"
}
```




