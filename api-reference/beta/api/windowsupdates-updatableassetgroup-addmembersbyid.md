---
title: updatableAssetGroup：addMembersById
description: 将相同类型的成员添加到 updatableAssetGroup。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 27585b3ad87c4154140024705227612a988c7a76
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239482"
---
# <a name="updatableassetgroup-addmembersbyid"></a><span data-ttu-id="a8934-103">updatableAssetGroup：addMembersById</span><span class="sxs-lookup"><span data-stu-id="a8934-103">updatableAssetGroup: addMembersById</span></span>
<span data-ttu-id="a8934-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="a8934-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8934-105">将相同类型的成员添加到 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="a8934-105">Add members of the same type to an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="a8934-106">您还可以使用 [addMembers 方法](windowsupdates-updatableassetgroup-addmembers.md) 添加成员。</span><span class="sxs-lookup"><span data-stu-id="a8934-106">You can also use the method [addMembers](windowsupdates-updatableassetgroup-addmembers.md) to add members.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8934-107">权限</span><span class="sxs-lookup"><span data-stu-id="a8934-107">Permissions</span></span>
<span data-ttu-id="a8934-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a8934-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8934-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8934-110">Permission type</span></span>|<span data-ttu-id="a8934-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a8934-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8934-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8934-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a8934-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8934-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="a8934-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8934-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8934-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8934-115">Not supported.</span></span>|
|<span data-ttu-id="a8934-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8934-116">Application</span></span>|<span data-ttu-id="a8934-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8934-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8934-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8934-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/addMembersById
```

## <a name="request-headers"></a><span data-ttu-id="a8934-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8934-119">Request headers</span></span>
|<span data-ttu-id="a8934-120">名称</span><span class="sxs-lookup"><span data-stu-id="a8934-120">Name</span></span>|<span data-ttu-id="a8934-121">说明</span><span class="sxs-lookup"><span data-stu-id="a8934-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a8934-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8934-122">Authorization</span></span>|<span data-ttu-id="a8934-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a8934-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a8934-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a8934-125">Content-Type</span></span>|<span data-ttu-id="a8934-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a8934-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8934-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8934-128">Request body</span></span>
<span data-ttu-id="a8934-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8934-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a8934-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="a8934-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a8934-131">参数</span><span class="sxs-lookup"><span data-stu-id="a8934-131">Parameter</span></span>|<span data-ttu-id="a8934-132">类型</span><span class="sxs-lookup"><span data-stu-id="a8934-132">Type</span></span>|<span data-ttu-id="a8934-133">说明</span><span class="sxs-lookup"><span data-stu-id="a8934-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8934-134">ids</span><span class="sxs-lookup"><span data-stu-id="a8934-134">ids</span></span>|<span data-ttu-id="a8934-135">String collection</span><span class="sxs-lookup"><span data-stu-id="a8934-135">String collection</span></span>|<span data-ttu-id="a8934-136">与要添加为 [updatableAssetGroup](../resources/windowsupdates-updatableasset.md) 成员的 **updatableAsset** 资源相对应的标识符列表。</span><span class="sxs-lookup"><span data-stu-id="a8934-136">List of identifiers corresponding to the [updatableAsset](../resources/windowsupdates-updatableasset.md) resources to add as members of the **updatableAssetGroup**.</span></span>|
|<span data-ttu-id="a8934-137">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="a8934-137">memberEntityType</span></span>|<span data-ttu-id="a8934-138">字符串</span><span class="sxs-lookup"><span data-stu-id="a8934-138">String</span></span>|<span data-ttu-id="a8934-139">**updatableAsset 资源的完整** 类型。</span><span class="sxs-lookup"><span data-stu-id="a8934-139">The full type of the **updatableAsset** resources.</span></span> <span data-ttu-id="a8934-140">可能的值是 `#microsoft.graph.windowsUpdates.azureADDevice` ：。</span><span class="sxs-lookup"><span data-stu-id="a8934-140">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`.</span></span>|

## <a name="response"></a><span data-ttu-id="a8934-141">响应</span><span class="sxs-lookup"><span data-stu-id="a8934-141">Response</span></span>

<span data-ttu-id="a8934-142">如果成功，此操作返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a8934-142">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="a8934-143">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a8934-143">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a8934-144">示例</span><span class="sxs-lookup"><span data-stu-id="a8934-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a8934-145">请求</span><span class="sxs-lookup"><span data-stu-id="a8934-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a8934-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8934-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updatableassetgroup_addmembersbyid"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/addMembersById
Content-Type: application/json

{
  "ids": [
    "String",
    "String",
    "String"
  ],
  "memberEntityType": "#microsoft.graph.windowsUpdates.azureADDevice"
}
```
# <a name="c"></a>[<span data-ttu-id="a8934-147">C#</span><span class="sxs-lookup"><span data-stu-id="a8934-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updatableassetgroup-addmembersbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8934-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8934-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updatableassetgroup-addmembersbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8934-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8934-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updatableassetgroup-addmembersbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8934-150">Java</span><span class="sxs-lookup"><span data-stu-id="a8934-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/updatableassetgroup-addmembersbyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a8934-151">响应</span><span class="sxs-lookup"><span data-stu-id="a8934-151">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

