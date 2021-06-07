---
title: 创建 roleAssignment
description: 创建新的 roleAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4876100121d29520396884b00014207470e4c418
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756847"
---
# <a name="create-roleassignment"></a><span data-ttu-id="a440b-103">创建 roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a440b-103">Create roleAssignment</span></span>

<span data-ttu-id="a440b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a440b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a440b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a440b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a440b-106">创建新的 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a440b-106">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a440b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a440b-107">Prerequisites</span></span>
<span data-ttu-id="a440b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a440b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a440b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a440b-110">Permission type</span></span>|<span data-ttu-id="a440b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a440b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a440b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a440b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a440b-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a440b-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="a440b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a440b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a440b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a440b-115">Not supported.</span></span>|
|<span data-ttu-id="a440b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a440b-116">Application</span></span>|<span data-ttu-id="a440b-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a440b-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a440b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a440b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="a440b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a440b-119">Request headers</span></span>
|<span data-ttu-id="a440b-120">标头</span><span class="sxs-lookup"><span data-stu-id="a440b-120">Header</span></span>|<span data-ttu-id="a440b-121">值</span><span class="sxs-lookup"><span data-stu-id="a440b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a440b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a440b-122">Authorization</span></span>|<span data-ttu-id="a440b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a440b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a440b-124">接受</span><span class="sxs-lookup"><span data-stu-id="a440b-124">Accept</span></span>|<span data-ttu-id="a440b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a440b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a440b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a440b-126">Request body</span></span>
<span data-ttu-id="a440b-127">在请求正文中，提供 roleAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a440b-127">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="a440b-128">下表显示创建 roleAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a440b-128">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="a440b-129">属性</span><span class="sxs-lookup"><span data-stu-id="a440b-129">Property</span></span>|<span data-ttu-id="a440b-130">类型</span><span class="sxs-lookup"><span data-stu-id="a440b-130">Type</span></span>|<span data-ttu-id="a440b-131">说明</span><span class="sxs-lookup"><span data-stu-id="a440b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a440b-132">id</span><span class="sxs-lookup"><span data-stu-id="a440b-132">id</span></span>|<span data-ttu-id="a440b-133">String</span><span class="sxs-lookup"><span data-stu-id="a440b-133">String</span></span>|<span data-ttu-id="a440b-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a440b-134">Key of the entity.</span></span> <span data-ttu-id="a440b-135">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="a440b-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="a440b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a440b-136">displayName</span></span>|<span data-ttu-id="a440b-137">String</span><span class="sxs-lookup"><span data-stu-id="a440b-137">String</span></span>|<span data-ttu-id="a440b-138">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="a440b-138">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="a440b-139">说明</span><span class="sxs-lookup"><span data-stu-id="a440b-139">description</span></span>|<span data-ttu-id="a440b-140">String</span><span class="sxs-lookup"><span data-stu-id="a440b-140">String</span></span>|<span data-ttu-id="a440b-141">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="a440b-141">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="a440b-142">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="a440b-142">resourceScopes</span></span>|<span data-ttu-id="a440b-143">String collection</span><span class="sxs-lookup"><span data-stu-id="a440b-143">String collection</span></span>|<span data-ttu-id="a440b-144">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="a440b-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="a440b-145">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="a440b-145">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="a440b-146">响应</span><span class="sxs-lookup"><span data-stu-id="a440b-146">Response</span></span>
<span data-ttu-id="a440b-147">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [roleAssignment](../resources/intune-rbac-roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a440b-147">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a440b-148">示例</span><span class="sxs-lookup"><span data-stu-id="a440b-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="a440b-149">请求</span><span class="sxs-lookup"><span data-stu-id="a440b-149">Request</span></span>
<span data-ttu-id="a440b-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a440b-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a440b-151">响应</span><span class="sxs-lookup"><span data-stu-id="a440b-151">Response</span></span>
<span data-ttu-id="a440b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a440b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




