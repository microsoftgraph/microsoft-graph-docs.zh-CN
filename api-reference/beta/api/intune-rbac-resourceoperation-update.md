---
title: 更新 resourceOperation
description: 更新 resourceOperation 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 435719ff8acc264fe36f431ea62dbb082519bfd4
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37189548"
---
# <a name="update-resourceoperation"></a><span data-ttu-id="194a7-103">更新 resourceOperation</span><span class="sxs-lookup"><span data-stu-id="194a7-103">Update resourceOperation</span></span>

> <span data-ttu-id="194a7-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="194a7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="194a7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="194a7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="194a7-106">更新 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="194a7-106">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="194a7-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="194a7-107">Prerequisites</span></span>
<span data-ttu-id="194a7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="194a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="194a7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="194a7-110">Permission type</span></span>|<span data-ttu-id="194a7-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="194a7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="194a7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="194a7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="194a7-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="194a7-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="194a7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="194a7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="194a7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="194a7-115">Not supported.</span></span>|
|<span data-ttu-id="194a7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="194a7-116">Application</span></span>|<span data-ttu-id="194a7-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="194a7-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="194a7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="194a7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="194a7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="194a7-119">Request headers</span></span>
|<span data-ttu-id="194a7-120">标头</span><span class="sxs-lookup"><span data-stu-id="194a7-120">Header</span></span>|<span data-ttu-id="194a7-121">值</span><span class="sxs-lookup"><span data-stu-id="194a7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="194a7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="194a7-122">Authorization</span></span>|<span data-ttu-id="194a7-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="194a7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="194a7-124">接受</span><span class="sxs-lookup"><span data-stu-id="194a7-124">Accept</span></span>|<span data-ttu-id="194a7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="194a7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="194a7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="194a7-126">Request body</span></span>
<span data-ttu-id="194a7-127">在请求正文中，提供 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="194a7-127">In the request body, supply a JSON representation for the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

<span data-ttu-id="194a7-128">下表显示创建 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="194a7-128">The following table shows the properties that are required when you create the [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>

|<span data-ttu-id="194a7-129">属性</span><span class="sxs-lookup"><span data-stu-id="194a7-129">Property</span></span>|<span data-ttu-id="194a7-130">类型</span><span class="sxs-lookup"><span data-stu-id="194a7-130">Type</span></span>|<span data-ttu-id="194a7-131">说明</span><span class="sxs-lookup"><span data-stu-id="194a7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="194a7-132">id</span><span class="sxs-lookup"><span data-stu-id="194a7-132">id</span></span>|<span data-ttu-id="194a7-133">字符串</span><span class="sxs-lookup"><span data-stu-id="194a7-133">String</span></span>|<span data-ttu-id="194a7-134">资源操作的键。</span><span class="sxs-lookup"><span data-stu-id="194a7-134">Key of the Resource Operation.</span></span> <span data-ttu-id="194a7-135">只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="194a7-135">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="194a7-136">resource</span><span class="sxs-lookup"><span data-stu-id="194a7-136">resource</span></span>|<span data-ttu-id="194a7-137">String</span><span class="sxs-lookup"><span data-stu-id="194a7-137">String</span></span>|<span data-ttu-id="194a7-138">此操作所属的资源类别。</span><span class="sxs-lookup"><span data-stu-id="194a7-138">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="194a7-139">resourceName</span><span class="sxs-lookup"><span data-stu-id="194a7-139">resourceName</span></span>|<span data-ttu-id="194a7-140">String</span><span class="sxs-lookup"><span data-stu-id="194a7-140">String</span></span>|<span data-ttu-id="194a7-141">执行此操作的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="194a7-141">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="194a7-142">actionName</span><span class="sxs-lookup"><span data-stu-id="194a7-142">actionName</span></span>|<span data-ttu-id="194a7-143">String</span><span class="sxs-lookup"><span data-stu-id="194a7-143">String</span></span>|<span data-ttu-id="194a7-144">此操作将执行的操作类型。</span><span class="sxs-lookup"><span data-stu-id="194a7-144">Type of action this operation is going to perform.</span></span> <span data-ttu-id="194a7-145">actionName 应简明，并尽可能限制在几个字以内。</span><span class="sxs-lookup"><span data-stu-id="194a7-145">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="194a7-146">说明</span><span class="sxs-lookup"><span data-stu-id="194a7-146">description</span></span>|<span data-ttu-id="194a7-147">String</span><span class="sxs-lookup"><span data-stu-id="194a7-147">String</span></span>|<span data-ttu-id="194a7-148">资源操作的说明。</span><span class="sxs-lookup"><span data-stu-id="194a7-148">Description of the resource operation.</span></span> <span data-ttu-id="194a7-149">当在 Azure 门户中显示时，会在操作的鼠标悬停文本中使用说明。</span><span class="sxs-lookup"><span data-stu-id="194a7-149">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="194a7-150">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="194a7-150">enabledForScopeValidation</span></span>|<span data-ttu-id="194a7-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="194a7-151">Boolean</span></span>|<span data-ttu-id="194a7-152">确定是否针对按角色分配定义的作用域验证权限。</span><span class="sxs-lookup"><span data-stu-id="194a7-152">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="194a7-153">响应</span><span class="sxs-lookup"><span data-stu-id="194a7-153">Response</span></span>
<span data-ttu-id="194a7-154">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="194a7-154">If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="194a7-155">示例</span><span class="sxs-lookup"><span data-stu-id="194a7-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="194a7-156">请求</span><span class="sxs-lookup"><span data-stu-id="194a7-156">Request</span></span>
<span data-ttu-id="194a7-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="194a7-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="194a7-158">响应</span><span class="sxs-lookup"><span data-stu-id="194a7-158">Response</span></span>
<span data-ttu-id="194a7-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="194a7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




