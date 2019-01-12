---
title: 创建 roleScopeTag
description: 创建新的 roleScopeTag 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 314e9c6fb05f51efb6e2af6ad62faf25974fe3b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915156"
---
# <a name="create-rolescopetag"></a><span data-ttu-id="6d64c-103">创建 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="6d64c-103">Create roleScopeTag</span></span>

> <span data-ttu-id="6d64c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6d64c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d64c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6d64c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6d64c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6d64c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d64c-107">创建新的[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6d64c-107">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6d64c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6d64c-108">Prerequisites</span></span>
<span data-ttu-id="6d64c-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="6d64c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d64c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d64c-111">Permission type</span></span>|<span data-ttu-id="6d64c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6d64c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d64c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d64c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6d64c-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d64c-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="6d64c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6d64c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d64c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d64c-116">Not supported.</span></span>|
|<span data-ttu-id="6d64c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d64c-117">Application</span></span>|<span data-ttu-id="6d64c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d64c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d64c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d64c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="6d64c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6d64c-120">Request headers</span></span>
|<span data-ttu-id="6d64c-121">标头</span><span class="sxs-lookup"><span data-stu-id="6d64c-121">Header</span></span>|<span data-ttu-id="6d64c-122">值</span><span class="sxs-lookup"><span data-stu-id="6d64c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d64c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d64c-123">Authorization</span></span>|<span data-ttu-id="6d64c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6d64c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d64c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6d64c-125">Accept</span></span>|<span data-ttu-id="6d64c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d64c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d64c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d64c-127">Request body</span></span>
<span data-ttu-id="6d64c-128">在请求正文中，提供 roleScopeTag 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d64c-128">In the request body, supply a JSON representation for the roleScopeTag object.</span></span>

<span data-ttu-id="6d64c-129">下表显示时创建 roleScopeTag 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6d64c-129">The following table shows the properties that are required when you create the roleScopeTag.</span></span>

|<span data-ttu-id="6d64c-130">属性</span><span class="sxs-lookup"><span data-stu-id="6d64c-130">Property</span></span>|<span data-ttu-id="6d64c-131">类型</span><span class="sxs-lookup"><span data-stu-id="6d64c-131">Type</span></span>|<span data-ttu-id="6d64c-132">说明</span><span class="sxs-lookup"><span data-stu-id="6d64c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d64c-133">id</span><span class="sxs-lookup"><span data-stu-id="6d64c-133">id</span></span>|<span data-ttu-id="6d64c-134">String</span><span class="sxs-lookup"><span data-stu-id="6d64c-134">String</span></span>|<span data-ttu-id="6d64c-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6d64c-135">Key of the entity.</span></span> <span data-ttu-id="6d64c-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="6d64c-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="6d64c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="6d64c-137">displayName</span></span>|<span data-ttu-id="6d64c-138">字符串</span><span class="sxs-lookup"><span data-stu-id="6d64c-138">String</span></span>|<span data-ttu-id="6d64c-139">显示或角色作用域标记的友好名称。</span><span class="sxs-lookup"><span data-stu-id="6d64c-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="6d64c-140">说明</span><span class="sxs-lookup"><span data-stu-id="6d64c-140">description</span></span>|<span data-ttu-id="6d64c-141">字符串</span><span class="sxs-lookup"><span data-stu-id="6d64c-141">String</span></span>|<span data-ttu-id="6d64c-142">角色作用域标记的说明。</span><span class="sxs-lookup"><span data-stu-id="6d64c-142">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="6d64c-143">响应</span><span class="sxs-lookup"><span data-stu-id="6d64c-143">Response</span></span>
<span data-ttu-id="6d64c-144">如果成功，此方法返回`201 Created`响应代码和响应正文中的[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6d64c-144">If successful, this method returns a `201 Created` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d64c-145">示例</span><span class="sxs-lookup"><span data-stu-id="6d64c-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="6d64c-146">请求</span><span class="sxs-lookup"><span data-stu-id="6d64c-146">Request</span></span>
<span data-ttu-id="6d64c-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6d64c-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6d64c-148">响应</span><span class="sxs-lookup"><span data-stu-id="6d64c-148">Response</span></span>
<span data-ttu-id="6d64c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6d64c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





