---
title: 创建 resourceOperation
description: 创建新的 resourceOperation 对象。
ms.openlocfilehash: 40f8c7175c5f6ad5e2885fe7e893bba118458be1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009542"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="2a214-103">创建 resourceOperation</span><span class="sxs-lookup"><span data-stu-id="2a214-103">Create resourceOperation</span></span>

> <span data-ttu-id="2a214-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2a214-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a214-105">创建新的 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2a214-105">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2a214-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="2a214-106">Prerequisites</span></span>
<span data-ttu-id="2a214-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="2a214-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a214-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a214-109">Permission type</span></span>|<span data-ttu-id="2a214-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2a214-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a214-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a214-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2a214-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a214-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="2a214-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a214-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a214-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a214-114">Not supported.</span></span>|
|<span data-ttu-id="2a214-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a214-115">Application</span></span>|<span data-ttu-id="2a214-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a214-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a214-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a214-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="2a214-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a214-118">Request headers</span></span>
|<span data-ttu-id="2a214-119">标头</span><span class="sxs-lookup"><span data-stu-id="2a214-119">Header</span></span>|<span data-ttu-id="2a214-120">值</span><span class="sxs-lookup"><span data-stu-id="2a214-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a214-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a214-121">Authorization</span></span>|<span data-ttu-id="2a214-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2a214-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a214-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2a214-123">Accept</span></span>|<span data-ttu-id="2a214-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2a214-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a214-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a214-125">Request body</span></span>
<span data-ttu-id="2a214-126">在请求正文中，提供 resourceOperation 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a214-126">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="2a214-127">下表显示创建 resourceOperation 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2a214-127">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="2a214-128">属性</span><span class="sxs-lookup"><span data-stu-id="2a214-128">Property</span></span>|<span data-ttu-id="2a214-129">类型</span><span class="sxs-lookup"><span data-stu-id="2a214-129">Type</span></span>|<span data-ttu-id="2a214-130">说明</span><span class="sxs-lookup"><span data-stu-id="2a214-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a214-131">id</span><span class="sxs-lookup"><span data-stu-id="2a214-131">id</span></span>|<span data-ttu-id="2a214-132">String</span><span class="sxs-lookup"><span data-stu-id="2a214-132">String</span></span>|<span data-ttu-id="2a214-133">资源操作的键。</span><span class="sxs-lookup"><span data-stu-id="2a214-133">Key of the Resource Operation.</span></span> <span data-ttu-id="2a214-134">只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="2a214-134">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="2a214-135">resourceName</span><span class="sxs-lookup"><span data-stu-id="2a214-135">resourceName</span></span>|<span data-ttu-id="2a214-136">String</span><span class="sxs-lookup"><span data-stu-id="2a214-136">String</span></span>|<span data-ttu-id="2a214-137">执行此操作的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="2a214-137">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="2a214-138">actionName</span><span class="sxs-lookup"><span data-stu-id="2a214-138">actionName</span></span>|<span data-ttu-id="2a214-139">String</span><span class="sxs-lookup"><span data-stu-id="2a214-139">String</span></span>|<span data-ttu-id="2a214-140">此操作将执行的操作类型。</span><span class="sxs-lookup"><span data-stu-id="2a214-140">Type of action this operation is going to perform.</span></span> <span data-ttu-id="2a214-141">actionName 应简明，并尽可能限制在几个字以内。</span><span class="sxs-lookup"><span data-stu-id="2a214-141">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="2a214-142">说明</span><span class="sxs-lookup"><span data-stu-id="2a214-142">description</span></span>|<span data-ttu-id="2a214-143">String</span><span class="sxs-lookup"><span data-stu-id="2a214-143">String</span></span>|<span data-ttu-id="2a214-144">资源操作的说明。</span><span class="sxs-lookup"><span data-stu-id="2a214-144">Description of the resource operation.</span></span> <span data-ttu-id="2a214-145">当在 Azure 门户中显示时，会在操作的鼠标悬停文本中使用说明。</span><span class="sxs-lookup"><span data-stu-id="2a214-145">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="2a214-146">响应</span><span class="sxs-lookup"><span data-stu-id="2a214-146">Response</span></span>
<span data-ttu-id="2a214-147">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2a214-147">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a214-148">示例</span><span class="sxs-lookup"><span data-stu-id="2a214-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="2a214-149">请求</span><span class="sxs-lookup"><span data-stu-id="2a214-149">Request</span></span>
<span data-ttu-id="2a214-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2a214-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations
Content-type: application/json
Content-length: 178

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="2a214-151">响应</span><span class="sxs-lookup"><span data-stu-id="2a214-151">Response</span></span>
<span data-ttu-id="2a214-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2a214-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 227

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```



