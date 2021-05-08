---
title: updatableAsset： enrollAssetsById
description: 在部署服务更新管理中注册相同类型的 updatableAsset 资源。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 127817e3623b86854f8c69812c385a25aee323f4
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241168"
---
# <a name="updatableasset-enrollassetsbyid"></a><span data-ttu-id="0ceb9-103">updatableAsset： enrollAssetsById</span><span class="sxs-lookup"><span data-stu-id="0ceb9-103">updatableAsset: enrollAssetsById</span></span>
<span data-ttu-id="0ceb9-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="0ceb9-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ceb9-105">在部署服务更新管理中注册相同类型的 [updatableAsset](../resources/windowsupdates-updatableasset.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="0ceb9-105">Enroll [updatableAsset](../resources/windowsupdates-updatableasset.md) resources of the same type in update management by the deployment service.</span></span>

<span data-ttu-id="0ceb9-106">您还可以使用 [enrollAssets 方法](windowsupdates-updatableasset-enrollassets.md) 注册资产。</span><span class="sxs-lookup"><span data-stu-id="0ceb9-106">You can also use the method [enrollAssets](windowsupdates-updatableasset-enrollassets.md) to enroll assets.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ceb9-107">权限</span><span class="sxs-lookup"><span data-stu-id="0ceb9-107">Permissions</span></span>
<span data-ttu-id="0ceb9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ceb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ceb9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ceb9-110">Permission type</span></span>|<span data-ttu-id="0ceb9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ceb9-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ceb9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ceb9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ceb9-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ceb9-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="0ceb9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ceb9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ceb9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ceb9-115">Not supported.</span></span>|
|<span data-ttu-id="0ceb9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ceb9-116">Application</span></span>|<span data-ttu-id="0ceb9-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ceb9-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ceb9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ceb9-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/enrollAssetsById
```

## <a name="request-headers"></a><span data-ttu-id="0ceb9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ceb9-119">Request headers</span></span>
|<span data-ttu-id="0ceb9-120">名称</span><span class="sxs-lookup"><span data-stu-id="0ceb9-120">Name</span></span>|<span data-ttu-id="0ceb9-121">说明</span><span class="sxs-lookup"><span data-stu-id="0ceb9-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0ceb9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ceb9-122">Authorization</span></span>|<span data-ttu-id="0ceb9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0ceb9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0ceb9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0ceb9-125">Content-Type</span></span>|<span data-ttu-id="0ceb9-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0ceb9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ceb9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ceb9-128">Request body</span></span>
<span data-ttu-id="0ceb9-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ceb9-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0ceb9-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="0ceb9-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0ceb9-131">参数</span><span class="sxs-lookup"><span data-stu-id="0ceb9-131">Parameter</span></span>|<span data-ttu-id="0ceb9-132">类型</span><span class="sxs-lookup"><span data-stu-id="0ceb9-132">Type</span></span>|<span data-ttu-id="0ceb9-133">说明</span><span class="sxs-lookup"><span data-stu-id="0ceb9-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ceb9-134">updateCategory</span><span class="sxs-lookup"><span data-stu-id="0ceb9-134">updateCategory</span></span>|<span data-ttu-id="0ceb9-135">microsoft.graph.windowsUpdates.updateCategory</span><span class="sxs-lookup"><span data-stu-id="0ceb9-135">microsoft.graph.windowsUpdates.updateCategory</span></span>|<span data-ttu-id="0ceb9-136">要管理的服务的更新类别。</span><span class="sxs-lookup"><span data-stu-id="0ceb9-136">The category of updates for the service to manage.</span></span> <span data-ttu-id="0ceb9-137">支持 **updateCategory** 值的子集。</span><span class="sxs-lookup"><span data-stu-id="0ceb9-137">Supports a subset of the values for **updateCategory**.</span></span> <span data-ttu-id="0ceb9-138">可能的值是 `feature` ：。</span><span class="sxs-lookup"><span data-stu-id="0ceb9-138">Possible values are: `feature`.</span></span>|
|<span data-ttu-id="0ceb9-139">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="0ceb9-139">memberEntityType</span></span>|<span data-ttu-id="0ceb9-140">字符串</span><span class="sxs-lookup"><span data-stu-id="0ceb9-140">String</span></span>|<span data-ttu-id="0ceb9-141">**updatableAsset 资源的完整** 类型。</span><span class="sxs-lookup"><span data-stu-id="0ceb9-141">The full type of the **updatableAsset** resources.</span></span> <span data-ttu-id="0ceb9-142">可能的值是 `#microsoft.graph.windowsUpdates.azureADDevice` ：。</span><span class="sxs-lookup"><span data-stu-id="0ceb9-142">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`.</span></span>|
|<span data-ttu-id="0ceb9-143">ids</span><span class="sxs-lookup"><span data-stu-id="0ceb9-143">ids</span></span>|<span data-ttu-id="0ceb9-144">String collection</span><span class="sxs-lookup"><span data-stu-id="0ceb9-144">String collection</span></span>|<span data-ttu-id="0ceb9-145">与 **updatableAsset** 资源相对应的标识符列表，这些资源由服务针对给定 **updateCategory** 注册更新管理。</span><span class="sxs-lookup"><span data-stu-id="0ceb9-145">List of identifiers corresponding to the **updatableAsset** resources to enroll in update management by the service for the given **updateCategory**.</span></span>|

## <a name="response"></a><span data-ttu-id="0ceb9-146">响应</span><span class="sxs-lookup"><span data-stu-id="0ceb9-146">Response</span></span>

<span data-ttu-id="0ceb9-147">如果成功，此操作返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0ceb9-147">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="0ceb9-148">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0ceb9-148">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0ceb9-149">示例</span><span class="sxs-lookup"><span data-stu-id="0ceb9-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0ceb9-150">请求</span><span class="sxs-lookup"><span data-stu-id="0ceb9-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0ceb9-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ceb9-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updatableasset_enrollassetsbyid"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/enrollAssetsById
Content-Type: application/json

{
  "updateCategory": "feature",
  "memberEntityType": "#microsoft.graph.windowsUpdates.azureADDevice",
  "ids": [
    "String",
    "String",
    "String"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="0ceb9-152">C#</span><span class="sxs-lookup"><span data-stu-id="0ceb9-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updatableasset-enrollassetsbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ceb9-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ceb9-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updatableasset-enrollassetsbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ceb9-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ceb9-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updatableasset-enrollassetsbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0ceb9-155">Java</span><span class="sxs-lookup"><span data-stu-id="0ceb9-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/updatableasset-enrollassetsbyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="0ceb9-156">响应</span><span class="sxs-lookup"><span data-stu-id="0ceb9-156">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

