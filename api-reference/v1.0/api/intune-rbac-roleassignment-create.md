---
title: 创建 roleAssignment
description: 创建新的 roleAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b8f757d8131b40912b6e02ca402bb2f5aa622fc
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961558"
---
# <a name="create-roleassignment"></a><span data-ttu-id="b7341-103">创建 roleAssignment</span><span class="sxs-lookup"><span data-stu-id="b7341-103">Create roleAssignment</span></span>

> <span data-ttu-id="b7341-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b7341-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7341-105">创建新的 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b7341-105">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7341-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="b7341-106">Prerequisites</span></span>
<span data-ttu-id="b7341-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7341-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7341-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7341-109">Permission type</span></span>|<span data-ttu-id="b7341-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b7341-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7341-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7341-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b7341-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7341-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="b7341-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7341-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7341-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7341-114">Not supported.</span></span>|
|<span data-ttu-id="b7341-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7341-115">Application</span></span>|<span data-ttu-id="b7341-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7341-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7341-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7341-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="b7341-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7341-118">Request headers</span></span>
|<span data-ttu-id="b7341-119">标头</span><span class="sxs-lookup"><span data-stu-id="b7341-119">Header</span></span>|<span data-ttu-id="b7341-120">值</span><span class="sxs-lookup"><span data-stu-id="b7341-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7341-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7341-121">Authorization</span></span>|<span data-ttu-id="b7341-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b7341-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7341-123">接受</span><span class="sxs-lookup"><span data-stu-id="b7341-123">Accept</span></span>|<span data-ttu-id="b7341-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b7341-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7341-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7341-125">Request body</span></span>
<span data-ttu-id="b7341-126">在请求正文中，提供 roleAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7341-126">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="b7341-127">下表显示创建 roleAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b7341-127">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="b7341-128">属性</span><span class="sxs-lookup"><span data-stu-id="b7341-128">Property</span></span>|<span data-ttu-id="b7341-129">类型</span><span class="sxs-lookup"><span data-stu-id="b7341-129">Type</span></span>|<span data-ttu-id="b7341-130">说明</span><span class="sxs-lookup"><span data-stu-id="b7341-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7341-131">id</span><span class="sxs-lookup"><span data-stu-id="b7341-131">id</span></span>|<span data-ttu-id="b7341-132">String</span><span class="sxs-lookup"><span data-stu-id="b7341-132">String</span></span>|<span data-ttu-id="b7341-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b7341-133">Key of the entity.</span></span> <span data-ttu-id="b7341-134">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="b7341-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="b7341-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b7341-135">displayName</span></span>|<span data-ttu-id="b7341-136">String</span><span class="sxs-lookup"><span data-stu-id="b7341-136">String</span></span>|<span data-ttu-id="b7341-137">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="b7341-137">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="b7341-138">description</span><span class="sxs-lookup"><span data-stu-id="b7341-138">description</span></span>|<span data-ttu-id="b7341-139">String</span><span class="sxs-lookup"><span data-stu-id="b7341-139">String</span></span>|<span data-ttu-id="b7341-140">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="b7341-140">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="b7341-141">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="b7341-141">resourceScopes</span></span>|<span data-ttu-id="b7341-142">String collection</span><span class="sxs-lookup"><span data-stu-id="b7341-142">String collection</span></span>|<span data-ttu-id="b7341-143">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="b7341-143">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="b7341-144">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="b7341-144">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="b7341-145">响应</span><span class="sxs-lookup"><span data-stu-id="b7341-145">Response</span></span>
<span data-ttu-id="b7341-146">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b7341-146">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7341-147">示例</span><span class="sxs-lookup"><span data-stu-id="b7341-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7341-148">请求</span><span class="sxs-lookup"><span data-stu-id="b7341-148">Request</span></span>
<span data-ttu-id="b7341-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b7341-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
Content-type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="b7341-150">响应</span><span class="sxs-lookup"><span data-stu-id="b7341-150">Response</span></span>
<span data-ttu-id="b7341-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b7341-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```



