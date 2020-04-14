---
title: 更新 resourceOperation
description: 更新 resourceOperation 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d6afbcc8a3b6adc0ade92e17588377e220c247f2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43421086"
---
# <a name="update-resourceoperation"></a><span data-ttu-id="3d0a0-103">更新 resourceOperation</span><span class="sxs-lookup"><span data-stu-id="3d0a0-103">Update resourceOperation</span></span>

<span data-ttu-id="3d0a0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d0a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d0a0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3d0a0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d0a0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3d0a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d0a0-107">更新 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3d0a0-107">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d0a0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3d0a0-108">Prerequisites</span></span>
<span data-ttu-id="3d0a0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3d0a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d0a0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d0a0-111">Permission type</span></span>|<span data-ttu-id="3d0a0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3d0a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d0a0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d0a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d0a0-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d0a0-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="3d0a0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d0a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d0a0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d0a0-116">Not supported.</span></span>|
|<span data-ttu-id="3d0a0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d0a0-117">Application</span></span>|<span data-ttu-id="3d0a0-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d0a0-118">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d0a0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d0a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="3d0a0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d0a0-120">Request headers</span></span>
|<span data-ttu-id="3d0a0-121">标头</span><span class="sxs-lookup"><span data-stu-id="3d0a0-121">Header</span></span>|<span data-ttu-id="3d0a0-122">值</span><span class="sxs-lookup"><span data-stu-id="3d0a0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d0a0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d0a0-123">Authorization</span></span>|<span data-ttu-id="3d0a0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3d0a0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d0a0-125">接受</span><span class="sxs-lookup"><span data-stu-id="3d0a0-125">Accept</span></span>|<span data-ttu-id="3d0a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d0a0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d0a0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3d0a0-127">Request body</span></span>
<span data-ttu-id="3d0a0-128">在请求正文中，提供 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d0a0-128">In the request body, supply a JSON representation for the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

<span data-ttu-id="3d0a0-129">下表显示创建 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3d0a0-129">The following table shows the properties that are required when you create the [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>

|<span data-ttu-id="3d0a0-130">属性</span><span class="sxs-lookup"><span data-stu-id="3d0a0-130">Property</span></span>|<span data-ttu-id="3d0a0-131">类型</span><span class="sxs-lookup"><span data-stu-id="3d0a0-131">Type</span></span>|<span data-ttu-id="3d0a0-132">说明</span><span class="sxs-lookup"><span data-stu-id="3d0a0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d0a0-133">id</span><span class="sxs-lookup"><span data-stu-id="3d0a0-133">id</span></span>|<span data-ttu-id="3d0a0-134">字符串</span><span class="sxs-lookup"><span data-stu-id="3d0a0-134">String</span></span>|<span data-ttu-id="3d0a0-135">资源操作的键。</span><span class="sxs-lookup"><span data-stu-id="3d0a0-135">Key of the Resource Operation.</span></span> <span data-ttu-id="3d0a0-136">只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="3d0a0-136">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="3d0a0-137">resource</span><span class="sxs-lookup"><span data-stu-id="3d0a0-137">resource</span></span>|<span data-ttu-id="3d0a0-138">String</span><span class="sxs-lookup"><span data-stu-id="3d0a0-138">String</span></span>|<span data-ttu-id="3d0a0-139">此操作所属的资源类别。</span><span class="sxs-lookup"><span data-stu-id="3d0a0-139">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="3d0a0-140">resourceName</span><span class="sxs-lookup"><span data-stu-id="3d0a0-140">resourceName</span></span>|<span data-ttu-id="3d0a0-141">String</span><span class="sxs-lookup"><span data-stu-id="3d0a0-141">String</span></span>|<span data-ttu-id="3d0a0-142">执行此操作的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="3d0a0-142">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="3d0a0-143">actionName</span><span class="sxs-lookup"><span data-stu-id="3d0a0-143">actionName</span></span>|<span data-ttu-id="3d0a0-144">String</span><span class="sxs-lookup"><span data-stu-id="3d0a0-144">String</span></span>|<span data-ttu-id="3d0a0-145">此操作将执行的操作类型。</span><span class="sxs-lookup"><span data-stu-id="3d0a0-145">Type of action this operation is going to perform.</span></span> <span data-ttu-id="3d0a0-146">actionName 应简明，并尽可能限制在几个字以内。</span><span class="sxs-lookup"><span data-stu-id="3d0a0-146">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="3d0a0-147">description</span><span class="sxs-lookup"><span data-stu-id="3d0a0-147">description</span></span>|<span data-ttu-id="3d0a0-148">String</span><span class="sxs-lookup"><span data-stu-id="3d0a0-148">String</span></span>|<span data-ttu-id="3d0a0-149">资源操作的说明。</span><span class="sxs-lookup"><span data-stu-id="3d0a0-149">Description of the resource operation.</span></span> <span data-ttu-id="3d0a0-150">当在 Azure 门户中显示时，会在操作的鼠标悬停文本中使用说明。</span><span class="sxs-lookup"><span data-stu-id="3d0a0-150">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="3d0a0-151">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="3d0a0-151">enabledForScopeValidation</span></span>|<span data-ttu-id="3d0a0-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d0a0-152">Boolean</span></span>|<span data-ttu-id="3d0a0-153">确定是否针对按角色分配定义的作用域验证权限。</span><span class="sxs-lookup"><span data-stu-id="3d0a0-153">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="3d0a0-154">响应</span><span class="sxs-lookup"><span data-stu-id="3d0a0-154">Response</span></span>
<span data-ttu-id="3d0a0-155">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3d0a0-155">If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d0a0-156">示例</span><span class="sxs-lookup"><span data-stu-id="3d0a0-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d0a0-157">请求</span><span class="sxs-lookup"><span data-stu-id="3d0a0-157">Request</span></span>
<span data-ttu-id="3d0a0-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3d0a0-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}
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

### <a name="response"></a><span data-ttu-id="3d0a0-159">响应</span><span class="sxs-lookup"><span data-stu-id="3d0a0-159">Response</span></span>
<span data-ttu-id="3d0a0-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3d0a0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



