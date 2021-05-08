---
title: updatableAsset：unenrollAssetsById
description: 从部署服务的更新管理中注销相同类型的 UpdatableAsset 资源。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 72a3e97aee449953204225d40fee236126bddaa1
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240690"
---
# <a name="updatableasset-unenrollassetsbyid"></a><span data-ttu-id="1f178-103">updatableAsset：unenrollAssetsById</span><span class="sxs-lookup"><span data-stu-id="1f178-103">updatableAsset: unenrollAssetsById</span></span>
<span data-ttu-id="1f178-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="1f178-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f178-105">从部署服务的更新管理中注销相同类型的 [UpdatableAsset](../resources/windowsupdates-updatableasset.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="1f178-105">Unenroll [updatableAsset](../resources/windowsupdates-updatableasset.md) resources of the same type from update management by the deployment service.</span></span>

<span data-ttu-id="1f178-106">您还可以使用 [unenrollAssets 方法](windowsupdates-updatableasset-unenrollassets.md) 注销资产。</span><span class="sxs-lookup"><span data-stu-id="1f178-106">You can also use the method [unenrollAssets](windowsupdates-updatableasset-unenrollassets.md) to unenroll assets.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f178-107">权限</span><span class="sxs-lookup"><span data-stu-id="1f178-107">Permissions</span></span>
<span data-ttu-id="1f178-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1f178-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f178-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f178-110">Permission type</span></span>|<span data-ttu-id="1f178-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1f178-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f178-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f178-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1f178-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f178-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="1f178-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f178-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f178-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f178-115">Not supported.</span></span>|
|<span data-ttu-id="1f178-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f178-116">Application</span></span>|<span data-ttu-id="1f178-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f178-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f178-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f178-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/unenrollAssetsById
```

## <a name="request-headers"></a><span data-ttu-id="1f178-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f178-119">Request headers</span></span>
|<span data-ttu-id="1f178-120">名称</span><span class="sxs-lookup"><span data-stu-id="1f178-120">Name</span></span>|<span data-ttu-id="1f178-121">说明</span><span class="sxs-lookup"><span data-stu-id="1f178-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1f178-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f178-122">Authorization</span></span>|<span data-ttu-id="1f178-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1f178-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1f178-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1f178-125">Content-Type</span></span>|<span data-ttu-id="1f178-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1f178-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f178-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f178-128">Request body</span></span>
<span data-ttu-id="1f178-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f178-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1f178-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="1f178-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1f178-131">参数</span><span class="sxs-lookup"><span data-stu-id="1f178-131">Parameter</span></span>|<span data-ttu-id="1f178-132">类型</span><span class="sxs-lookup"><span data-stu-id="1f178-132">Type</span></span>|<span data-ttu-id="1f178-133">说明</span><span class="sxs-lookup"><span data-stu-id="1f178-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f178-134">updateCategory</span><span class="sxs-lookup"><span data-stu-id="1f178-134">updateCategory</span></span>|<span data-ttu-id="1f178-135">microsoft.graph.windowsUpdates.updateCategory</span><span class="sxs-lookup"><span data-stu-id="1f178-135">microsoft.graph.windowsUpdates.updateCategory</span></span>|<span data-ttu-id="1f178-136">要停止管理的服务的更新类别。</span><span class="sxs-lookup"><span data-stu-id="1f178-136">The category of updates for the service to stop managing.</span></span> <span data-ttu-id="1f178-137">支持 **updateCategory** 值的子集。</span><span class="sxs-lookup"><span data-stu-id="1f178-137">Supports a subset of the values for **updateCategory**.</span></span> <span data-ttu-id="1f178-138">可能的值是 `feature` ：。</span><span class="sxs-lookup"><span data-stu-id="1f178-138">Possible values are: `feature`.</span></span>|
|<span data-ttu-id="1f178-139">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="1f178-139">memberEntityType</span></span>|<span data-ttu-id="1f178-140">字符串</span><span class="sxs-lookup"><span data-stu-id="1f178-140">String</span></span>|<span data-ttu-id="1f178-141">**updatableAsset 资源的完整** 类型。</span><span class="sxs-lookup"><span data-stu-id="1f178-141">The full type of the **updatableAsset** resources.</span></span> <span data-ttu-id="1f178-142">可能的值是 `#microsoft.graph.windowsUpdates.azureADDevice` ：。</span><span class="sxs-lookup"><span data-stu-id="1f178-142">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`.</span></span>|
|<span data-ttu-id="1f178-143">ids</span><span class="sxs-lookup"><span data-stu-id="1f178-143">ids</span></span>|<span data-ttu-id="1f178-144">String collection</span><span class="sxs-lookup"><span data-stu-id="1f178-144">String collection</span></span>|<span data-ttu-id="1f178-145">与 **updatableAsset** 资源对应的标识符列表，用于注销给定 **updateCategory** 的服务的更新管理。</span><span class="sxs-lookup"><span data-stu-id="1f178-145">List of identifiers corresponding to the **updatableAsset** resources to unenroll from update management by the service for the given **updateCategory**.</span></span>|

## <a name="response"></a><span data-ttu-id="1f178-146">响应</span><span class="sxs-lookup"><span data-stu-id="1f178-146">Response</span></span>

<span data-ttu-id="1f178-147">如果成功，此操作返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1f178-147">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="1f178-148">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1f178-148">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1f178-149">示例</span><span class="sxs-lookup"><span data-stu-id="1f178-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1f178-150">请求</span><span class="sxs-lookup"><span data-stu-id="1f178-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1f178-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f178-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updatableasset_unenrollassetsbyid"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/unenrollAssetsById
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
# <a name="c"></a>[<span data-ttu-id="1f178-152">C#</span><span class="sxs-lookup"><span data-stu-id="1f178-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updatableasset-unenrollassetsbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f178-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f178-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updatableasset-unenrollassetsbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f178-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f178-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updatableasset-unenrollassetsbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f178-155">Java</span><span class="sxs-lookup"><span data-stu-id="1f178-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/updatableasset-unenrollassetsbyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1f178-156">响应</span><span class="sxs-lookup"><span data-stu-id="1f178-156">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

