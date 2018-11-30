---
title: 更新 roleScopeTag
description: 更新 roleScopeTag 对象的属性。
ms.openlocfilehash: d18f4f47be9aab01b1221e9ce7736878bb059bed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047993"
---
# <a name="update-rolescopetag"></a><span data-ttu-id="2f817-103">更新 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="2f817-103">Update roleScopeTag</span></span>

> <span data-ttu-id="2f817-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2f817-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f817-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2f817-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2f817-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2f817-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f817-107">更新[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2f817-107">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2f817-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2f817-108">Prerequisites</span></span>
<span data-ttu-id="2f817-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="2f817-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f817-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f817-111">Permission type</span></span>|<span data-ttu-id="2f817-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2f817-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f817-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f817-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f817-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f817-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="2f817-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f817-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f817-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f817-116">Not supported.</span></span>|
|<span data-ttu-id="2f817-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f817-117">Application</span></span>|<span data-ttu-id="2f817-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f817-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f817-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f817-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleScopeTags/{roleScopeTagId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="request-headers"></a><span data-ttu-id="2f817-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f817-120">Request headers</span></span>
|<span data-ttu-id="2f817-121">标头</span><span class="sxs-lookup"><span data-stu-id="2f817-121">Header</span></span>|<span data-ttu-id="2f817-122">值</span><span class="sxs-lookup"><span data-stu-id="2f817-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f817-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f817-123">Authorization</span></span>|<span data-ttu-id="2f817-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2f817-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f817-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2f817-125">Accept</span></span>|<span data-ttu-id="2f817-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f817-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f817-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f817-127">Request body</span></span>
<span data-ttu-id="2f817-128">在请求正文中，提供[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f817-128">In the request body, supply a JSON representation for the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

<span data-ttu-id="2f817-129">下表显示时创建[roleScopeTag](../resources/intune-rbac-rolescopetag.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2f817-129">The following table shows the properties that are required when you create the [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>

|<span data-ttu-id="2f817-130">属性</span><span class="sxs-lookup"><span data-stu-id="2f817-130">Property</span></span>|<span data-ttu-id="2f817-131">类型</span><span class="sxs-lookup"><span data-stu-id="2f817-131">Type</span></span>|<span data-ttu-id="2f817-132">说明</span><span class="sxs-lookup"><span data-stu-id="2f817-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f817-133">id</span><span class="sxs-lookup"><span data-stu-id="2f817-133">id</span></span>|<span data-ttu-id="2f817-134">String</span><span class="sxs-lookup"><span data-stu-id="2f817-134">String</span></span>|<span data-ttu-id="2f817-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2f817-135">Key of the entity.</span></span> <span data-ttu-id="2f817-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="2f817-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="2f817-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2f817-137">displayName</span></span>|<span data-ttu-id="2f817-138">字符串</span><span class="sxs-lookup"><span data-stu-id="2f817-138">String</span></span>|<span data-ttu-id="2f817-139">显示或角色作用域标记的友好名称。</span><span class="sxs-lookup"><span data-stu-id="2f817-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="2f817-140">说明</span><span class="sxs-lookup"><span data-stu-id="2f817-140">description</span></span>|<span data-ttu-id="2f817-141">字符串</span><span class="sxs-lookup"><span data-stu-id="2f817-141">String</span></span>|<span data-ttu-id="2f817-142">角色作用域标记的说明。</span><span class="sxs-lookup"><span data-stu-id="2f817-142">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="2f817-143">响应</span><span class="sxs-lookup"><span data-stu-id="2f817-143">Response</span></span>
<span data-ttu-id="2f817-144">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2f817-144">If successful, this method returns a `200 OK` response code and an updated [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f817-145">示例</span><span class="sxs-lookup"><span data-stu-id="2f817-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="2f817-146">请求</span><span class="sxs-lookup"><span data-stu-id="2f817-146">Request</span></span>
<span data-ttu-id="2f817-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f817-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="2f817-148">响应</span><span class="sxs-lookup"><span data-stu-id="2f817-148">Response</span></span>
<span data-ttu-id="2f817-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2f817-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





