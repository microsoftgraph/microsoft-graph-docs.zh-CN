---
title: 创建 roleDefinition
description: 创建新的 roleDefinition 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 27dc878346645c5b7d2e35ebc7fc468afa043a7c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966746"
---
# <a name="create-roledefinition"></a><span data-ttu-id="bb339-103">创建 roleDefinition</span><span class="sxs-lookup"><span data-stu-id="bb339-103">Create roleDefinition</span></span>

> <span data-ttu-id="bb339-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bb339-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb339-105">创建新的 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bb339-105">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bb339-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="bb339-106">Prerequisites</span></span>
<span data-ttu-id="bb339-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="bb339-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb339-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb339-109">Permission type</span></span>|<span data-ttu-id="bb339-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bb339-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb339-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb339-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bb339-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb339-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="bb339-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb339-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb339-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb339-114">Not supported.</span></span>|
|<span data-ttu-id="bb339-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb339-115">Application</span></span>|<span data-ttu-id="bb339-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb339-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb339-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb339-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="bb339-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb339-118">Request headers</span></span>
|<span data-ttu-id="bb339-119">标头</span><span class="sxs-lookup"><span data-stu-id="bb339-119">Header</span></span>|<span data-ttu-id="bb339-120">值</span><span class="sxs-lookup"><span data-stu-id="bb339-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb339-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb339-121">Authorization</span></span>|<span data-ttu-id="bb339-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bb339-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb339-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bb339-123">Accept</span></span>|<span data-ttu-id="bb339-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bb339-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb339-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb339-125">Request body</span></span>
<span data-ttu-id="bb339-126">在请求正文中，提供 roleDefinition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb339-126">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="bb339-127">下表显示创建 roleDefinition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bb339-127">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="bb339-128">属性</span><span class="sxs-lookup"><span data-stu-id="bb339-128">Property</span></span>|<span data-ttu-id="bb339-129">类型</span><span class="sxs-lookup"><span data-stu-id="bb339-129">Type</span></span>|<span data-ttu-id="bb339-130">说明</span><span class="sxs-lookup"><span data-stu-id="bb339-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb339-131">id</span><span class="sxs-lookup"><span data-stu-id="bb339-131">id</span></span>|<span data-ttu-id="bb339-132">String</span><span class="sxs-lookup"><span data-stu-id="bb339-132">String</span></span>|<span data-ttu-id="bb339-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bb339-133">Key of the entity.</span></span> <span data-ttu-id="bb339-134">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="bb339-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="bb339-135">displayName</span><span class="sxs-lookup"><span data-stu-id="bb339-135">displayName</span></span>|<span data-ttu-id="bb339-136">String</span><span class="sxs-lookup"><span data-stu-id="bb339-136">String</span></span>|<span data-ttu-id="bb339-137">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="bb339-137">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="bb339-138">说明</span><span class="sxs-lookup"><span data-stu-id="bb339-138">description</span></span>|<span data-ttu-id="bb339-139">String</span><span class="sxs-lookup"><span data-stu-id="bb339-139">String</span></span>|<span data-ttu-id="bb339-140">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="bb339-140">Description of the Role definition.</span></span>|
|<span data-ttu-id="bb339-141">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="bb339-141">rolePermissions</span></span>|<span data-ttu-id="bb339-142">[rolePermission](../resources/intune-rbac-rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bb339-142">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="bb339-143">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="bb339-143">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="bb339-144">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="bb339-144">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="bb339-145">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="bb339-145">isBuiltIn</span></span>|<span data-ttu-id="bb339-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb339-146">Boolean</span></span>|<span data-ttu-id="bb339-147">角色类型。</span><span class="sxs-lookup"><span data-stu-id="bb339-147">Type of Role.</span></span> <span data-ttu-id="bb339-148">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="bb339-148">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="bb339-149">响应</span><span class="sxs-lookup"><span data-stu-id="bb339-149">Response</span></span>
<span data-ttu-id="bb339-150">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [roleDefinition](../resources/intune-rbac-roledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bb339-150">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb339-151">示例</span><span class="sxs-lookup"><span data-stu-id="bb339-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="bb339-152">请求</span><span class="sxs-lookup"><span data-stu-id="bb339-152">Request</span></span>
<span data-ttu-id="bb339-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bb339-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
Content-type: application/json
Content-length: 580

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="bb339-154">响应</span><span class="sxs-lookup"><span data-stu-id="bb339-154">Response</span></span>
<span data-ttu-id="bb339-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bb339-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 629

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```



