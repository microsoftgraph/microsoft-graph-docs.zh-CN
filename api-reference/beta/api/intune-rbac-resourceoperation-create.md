---
title: 创建 resourceOperation
description: 创建新的 resourceOperation 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ed4978f42ed8f336720a9bc6458640111590d71f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148475"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="3b68a-103">创建 resourceOperation</span><span class="sxs-lookup"><span data-stu-id="3b68a-103">Create resourceOperation</span></span>

<span data-ttu-id="3b68a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b68a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b68a-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3b68a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b68a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3b68a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b68a-107">创建新的 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3b68a-107">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b68a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3b68a-108">Prerequisites</span></span>
<span data-ttu-id="3b68a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3b68a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b68a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b68a-111">Permission type</span></span>|<span data-ttu-id="3b68a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3b68a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b68a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b68a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b68a-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b68a-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="3b68a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b68a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b68a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b68a-116">Not supported.</span></span>|
|<span data-ttu-id="3b68a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b68a-117">Application</span></span>|<span data-ttu-id="3b68a-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b68a-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b68a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b68a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="3b68a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3b68a-120">Request headers</span></span>
|<span data-ttu-id="3b68a-121">标头</span><span class="sxs-lookup"><span data-stu-id="3b68a-121">Header</span></span>|<span data-ttu-id="3b68a-122">值</span><span class="sxs-lookup"><span data-stu-id="3b68a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b68a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b68a-123">Authorization</span></span>|<span data-ttu-id="3b68a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3b68a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b68a-125">接受</span><span class="sxs-lookup"><span data-stu-id="3b68a-125">Accept</span></span>|<span data-ttu-id="3b68a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b68a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b68a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b68a-127">Request body</span></span>
<span data-ttu-id="3b68a-128">在请求正文中，提供 resourceOperation 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b68a-128">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="3b68a-129">下表显示创建 resourceOperation 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3b68a-129">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="3b68a-130">属性</span><span class="sxs-lookup"><span data-stu-id="3b68a-130">Property</span></span>|<span data-ttu-id="3b68a-131">类型</span><span class="sxs-lookup"><span data-stu-id="3b68a-131">Type</span></span>|<span data-ttu-id="3b68a-132">说明</span><span class="sxs-lookup"><span data-stu-id="3b68a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b68a-133">id</span><span class="sxs-lookup"><span data-stu-id="3b68a-133">id</span></span>|<span data-ttu-id="3b68a-134">String</span><span class="sxs-lookup"><span data-stu-id="3b68a-134">String</span></span>|<span data-ttu-id="3b68a-135">资源操作的键。</span><span class="sxs-lookup"><span data-stu-id="3b68a-135">Key of the Resource Operation.</span></span> <span data-ttu-id="3b68a-136">只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="3b68a-136">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="3b68a-137">resource</span><span class="sxs-lookup"><span data-stu-id="3b68a-137">resource</span></span>|<span data-ttu-id="3b68a-138">String</span><span class="sxs-lookup"><span data-stu-id="3b68a-138">String</span></span>|<span data-ttu-id="3b68a-139">此操作所属的资源类别。</span><span class="sxs-lookup"><span data-stu-id="3b68a-139">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="3b68a-140">resourceName</span><span class="sxs-lookup"><span data-stu-id="3b68a-140">resourceName</span></span>|<span data-ttu-id="3b68a-141">String</span><span class="sxs-lookup"><span data-stu-id="3b68a-141">String</span></span>|<span data-ttu-id="3b68a-142">执行此操作的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="3b68a-142">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="3b68a-143">actionName</span><span class="sxs-lookup"><span data-stu-id="3b68a-143">actionName</span></span>|<span data-ttu-id="3b68a-144">String</span><span class="sxs-lookup"><span data-stu-id="3b68a-144">String</span></span>|<span data-ttu-id="3b68a-145">此操作将执行的操作类型。</span><span class="sxs-lookup"><span data-stu-id="3b68a-145">Type of action this operation is going to perform.</span></span> <span data-ttu-id="3b68a-146">actionName 应简明，并尽可能限制在几个字以内。</span><span class="sxs-lookup"><span data-stu-id="3b68a-146">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="3b68a-147">说明</span><span class="sxs-lookup"><span data-stu-id="3b68a-147">description</span></span>|<span data-ttu-id="3b68a-148">String</span><span class="sxs-lookup"><span data-stu-id="3b68a-148">String</span></span>|<span data-ttu-id="3b68a-149">资源操作的说明。</span><span class="sxs-lookup"><span data-stu-id="3b68a-149">Description of the resource operation.</span></span> <span data-ttu-id="3b68a-150">当在 Azure 门户中显示时，会在操作的鼠标悬停文本中使用说明。</span><span class="sxs-lookup"><span data-stu-id="3b68a-150">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="3b68a-151">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="3b68a-151">enabledForScopeValidation</span></span>|<span data-ttu-id="3b68a-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b68a-152">Boolean</span></span>|<span data-ttu-id="3b68a-153">确定是否针对每个角色分配定义的作用域验证权限。</span><span class="sxs-lookup"><span data-stu-id="3b68a-153">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="3b68a-154">响应</span><span class="sxs-lookup"><span data-stu-id="3b68a-154">Response</span></span>
<span data-ttu-id="3b68a-155">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3b68a-155">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b68a-156">示例</span><span class="sxs-lookup"><span data-stu-id="3b68a-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b68a-157">请求</span><span class="sxs-lookup"><span data-stu-id="3b68a-157">Request</span></span>
<span data-ttu-id="3b68a-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3b68a-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceOperations
Content-type: application/json
Content-length: 249

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resource": "Resource value",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value",
  "enabledForScopeValidation": true
}
```

### <a name="response"></a><span data-ttu-id="3b68a-159">响应</span><span class="sxs-lookup"><span data-stu-id="3b68a-159">Response</span></span>
<span data-ttu-id="3b68a-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b68a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 298

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
  "resource": "Resource value",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value",
  "enabledForScopeValidation": true
}
```




