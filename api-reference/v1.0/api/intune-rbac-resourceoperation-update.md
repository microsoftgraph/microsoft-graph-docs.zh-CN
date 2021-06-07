---
title: 更新 resourceOperation
description: 更新 resourceOperation 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e5a327480fbc5f219dcd56b4436170261357dc17
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756854"
---
# <a name="update-resourceoperation"></a><span data-ttu-id="7c4f8-103">更新 resourceOperation</span><span class="sxs-lookup"><span data-stu-id="7c4f8-103">Update resourceOperation</span></span>

<span data-ttu-id="7c4f8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c4f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c4f8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7c4f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c4f8-106">更新 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7c4f8-106">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c4f8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="7c4f8-107">Prerequisites</span></span>
<span data-ttu-id="7c4f8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c4f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c4f8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c4f8-110">Permission type</span></span>|<span data-ttu-id="7c4f8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c4f8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c4f8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c4f8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c4f8-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c4f8-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="7c4f8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c4f8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c4f8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c4f8-115">Not supported.</span></span>|
|<span data-ttu-id="7c4f8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c4f8-116">Application</span></span>|<span data-ttu-id="7c4f8-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c4f8-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c4f8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c4f8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="7c4f8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c4f8-119">Request headers</span></span>
|<span data-ttu-id="7c4f8-120">标头</span><span class="sxs-lookup"><span data-stu-id="7c4f8-120">Header</span></span>|<span data-ttu-id="7c4f8-121">值</span><span class="sxs-lookup"><span data-stu-id="7c4f8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c4f8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c4f8-122">Authorization</span></span>|<span data-ttu-id="7c4f8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7c4f8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c4f8-124">接受</span><span class="sxs-lookup"><span data-stu-id="7c4f8-124">Accept</span></span>|<span data-ttu-id="7c4f8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7c4f8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c4f8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c4f8-126">Request body</span></span>
<span data-ttu-id="7c4f8-127">在请求正文中，提供 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c4f8-127">In the request body, supply a JSON representation for the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

<span data-ttu-id="7c4f8-128">下表显示创建 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7c4f8-128">The following table shows the properties that are required when you create the [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>

|<span data-ttu-id="7c4f8-129">属性</span><span class="sxs-lookup"><span data-stu-id="7c4f8-129">Property</span></span>|<span data-ttu-id="7c4f8-130">类型</span><span class="sxs-lookup"><span data-stu-id="7c4f8-130">Type</span></span>|<span data-ttu-id="7c4f8-131">说明</span><span class="sxs-lookup"><span data-stu-id="7c4f8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c4f8-132">id</span><span class="sxs-lookup"><span data-stu-id="7c4f8-132">id</span></span>|<span data-ttu-id="7c4f8-133">String</span><span class="sxs-lookup"><span data-stu-id="7c4f8-133">String</span></span>|<span data-ttu-id="7c4f8-134">资源操作的键。</span><span class="sxs-lookup"><span data-stu-id="7c4f8-134">Key of the Resource Operation.</span></span> <span data-ttu-id="7c4f8-135">只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="7c4f8-135">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="7c4f8-136">resourceName</span><span class="sxs-lookup"><span data-stu-id="7c4f8-136">resourceName</span></span>|<span data-ttu-id="7c4f8-137">String</span><span class="sxs-lookup"><span data-stu-id="7c4f8-137">String</span></span>|<span data-ttu-id="7c4f8-138">执行此操作的资源的名称。</span><span class="sxs-lookup"><span data-stu-id="7c4f8-138">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="7c4f8-139">actionName</span><span class="sxs-lookup"><span data-stu-id="7c4f8-139">actionName</span></span>|<span data-ttu-id="7c4f8-140">String</span><span class="sxs-lookup"><span data-stu-id="7c4f8-140">String</span></span>|<span data-ttu-id="7c4f8-141">此操作将执行的操作类型。</span><span class="sxs-lookup"><span data-stu-id="7c4f8-141">Type of action this operation is going to perform.</span></span> <span data-ttu-id="7c4f8-142">actionName 应简明，并尽可能限制在几个字以内。</span><span class="sxs-lookup"><span data-stu-id="7c4f8-142">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="7c4f8-143">说明</span><span class="sxs-lookup"><span data-stu-id="7c4f8-143">description</span></span>|<span data-ttu-id="7c4f8-144">String</span><span class="sxs-lookup"><span data-stu-id="7c4f8-144">String</span></span>|<span data-ttu-id="7c4f8-145">资源操作的说明。</span><span class="sxs-lookup"><span data-stu-id="7c4f8-145">Description of the resource operation.</span></span> <span data-ttu-id="7c4f8-146">当在 Azure 门户中显示时，会在操作的鼠标悬停文本中使用说明。</span><span class="sxs-lookup"><span data-stu-id="7c4f8-146">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="7c4f8-147">响应</span><span class="sxs-lookup"><span data-stu-id="7c4f8-147">Response</span></span>
<span data-ttu-id="7c4f8-148">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [resourceOperation](../resources/intune-rbac-resourceoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7c4f8-148">If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c4f8-149">示例</span><span class="sxs-lookup"><span data-stu-id="7c4f8-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c4f8-150">请求</span><span class="sxs-lookup"><span data-stu-id="7c4f8-150">Request</span></span>
<span data-ttu-id="7c4f8-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7c4f8-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations/{resourceOperationId}
Content-type: application/json
Content-length: 178

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="7c4f8-152">响应</span><span class="sxs-lookup"><span data-stu-id="7c4f8-152">Response</span></span>
<span data-ttu-id="7c4f8-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7c4f8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




