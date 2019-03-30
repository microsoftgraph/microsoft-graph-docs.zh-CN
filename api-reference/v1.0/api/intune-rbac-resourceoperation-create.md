---
title: 创建 resourceOperation
description: 创建新的 resourceOperation 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8dafd0dff52fdbded8f6ff0fc8d6743a84dee797
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988334"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="01a90-103">创建 resourceOperation</span><span class="sxs-lookup"><span data-stu-id="01a90-103">Create resourceOperation</span></span>

> <span data-ttu-id="01a90-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="01a90-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01a90-105">创建新的 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="01a90-105">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01a90-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="01a90-106">Prerequisites</span></span>
<span data-ttu-id="01a90-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01a90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01a90-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="01a90-109">Permission type</span></span>|<span data-ttu-id="01a90-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="01a90-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01a90-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01a90-111">Delegated (work or school account)</span></span>|<span data-ttu-id="01a90-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01a90-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="01a90-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01a90-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01a90-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="01a90-114">Not supported.</span></span>|
|<span data-ttu-id="01a90-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="01a90-115">Application</span></span>|<span data-ttu-id="01a90-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="01a90-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01a90-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01a90-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="01a90-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="01a90-118">Request headers</span></span>
|<span data-ttu-id="01a90-119">标头</span><span class="sxs-lookup"><span data-stu-id="01a90-119">Header</span></span>|<span data-ttu-id="01a90-120">值</span><span class="sxs-lookup"><span data-stu-id="01a90-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01a90-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="01a90-121">Authorization</span></span>|<span data-ttu-id="01a90-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="01a90-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01a90-123">接受</span><span class="sxs-lookup"><span data-stu-id="01a90-123">Accept</span></span>|<span data-ttu-id="01a90-124">application/json</span><span class="sxs-lookup"><span data-stu-id="01a90-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01a90-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="01a90-125">Request body</span></span>
<span data-ttu-id="01a90-126">在请求正文中，提供 resourceOperation 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01a90-126">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="01a90-127">下表显示创建 resourceOperation 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="01a90-127">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="01a90-128">属性</span><span class="sxs-lookup"><span data-stu-id="01a90-128">Property</span></span>|<span data-ttu-id="01a90-129">类型</span><span class="sxs-lookup"><span data-stu-id="01a90-129">Type</span></span>|<span data-ttu-id="01a90-130">说明</span><span class="sxs-lookup"><span data-stu-id="01a90-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01a90-131">id</span><span class="sxs-lookup"><span data-stu-id="01a90-131">id</span></span>|<span data-ttu-id="01a90-132">String</span><span class="sxs-lookup"><span data-stu-id="01a90-132">String</span></span>|<span data-ttu-id="01a90-133">资源操作的键。</span><span class="sxs-lookup"><span data-stu-id="01a90-133">Key of the Resource Operation.</span></span> <span data-ttu-id="01a90-134">只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="01a90-134">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="01a90-135">resourceName</span><span class="sxs-lookup"><span data-stu-id="01a90-135">resourceName</span></span>|<span data-ttu-id="01a90-136">String</span><span class="sxs-lookup"><span data-stu-id="01a90-136">String</span></span>|<span data-ttu-id="01a90-137">执行此操作的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="01a90-137">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="01a90-138">actionName</span><span class="sxs-lookup"><span data-stu-id="01a90-138">actionName</span></span>|<span data-ttu-id="01a90-139">String</span><span class="sxs-lookup"><span data-stu-id="01a90-139">String</span></span>|<span data-ttu-id="01a90-140">此操作将执行的操作类型。</span><span class="sxs-lookup"><span data-stu-id="01a90-140">Type of action this operation is going to perform.</span></span> <span data-ttu-id="01a90-141">actionName 应简明，并尽可能限制在几个字以内。</span><span class="sxs-lookup"><span data-stu-id="01a90-141">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="01a90-142">description</span><span class="sxs-lookup"><span data-stu-id="01a90-142">description</span></span>|<span data-ttu-id="01a90-143">String</span><span class="sxs-lookup"><span data-stu-id="01a90-143">String</span></span>|<span data-ttu-id="01a90-144">资源操作的说明。</span><span class="sxs-lookup"><span data-stu-id="01a90-144">Description of the resource operation.</span></span> <span data-ttu-id="01a90-145">当在 Azure 门户中显示时，会在操作的鼠标悬停文本中使用说明。</span><span class="sxs-lookup"><span data-stu-id="01a90-145">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="01a90-146">响应</span><span class="sxs-lookup"><span data-stu-id="01a90-146">Response</span></span>
<span data-ttu-id="01a90-147">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="01a90-147">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01a90-148">示例</span><span class="sxs-lookup"><span data-stu-id="01a90-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="01a90-149">请求</span><span class="sxs-lookup"><span data-stu-id="01a90-149">Request</span></span>
<span data-ttu-id="01a90-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="01a90-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="01a90-151">响应</span><span class="sxs-lookup"><span data-stu-id="01a90-151">Response</span></span>
<span data-ttu-id="01a90-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="01a90-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



