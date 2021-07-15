---
title: updatableAssetGroup：removeMembers
description: 从 updatableAssetGroup 中删除成员。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: bd2275ce1971d341214899a5b56cecdd9c820e3c
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440411"
---
# <a name="updatableassetgroup-removemembers"></a><span data-ttu-id="59813-103">updatableAssetGroup：removeMembers</span><span class="sxs-lookup"><span data-stu-id="59813-103">updatableAssetGroup: removeMembers</span></span>
<span data-ttu-id="59813-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="59813-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59813-105">从 [updatableAssetGroup 中删除成员](../resources/windowsupdates-updatableassetgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="59813-105">Remove members from an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="59813-106">您还可以使用 [removeMembersById](windowsupdates-updatableassetgroup-removemembersbyid.md) 方法删除成员。</span><span class="sxs-lookup"><span data-stu-id="59813-106">You can also use the method [removeMembersById](windowsupdates-updatableassetgroup-removemembersbyid.md) to remove members.</span></span>

## <a name="permissions"></a><span data-ttu-id="59813-107">权限</span><span class="sxs-lookup"><span data-stu-id="59813-107">Permissions</span></span>
<span data-ttu-id="59813-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59813-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59813-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="59813-110">Permission type</span></span>|<span data-ttu-id="59813-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59813-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59813-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59813-112">Delegated (work or school account)</span></span>|<span data-ttu-id="59813-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59813-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="59813-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59813-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59813-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="59813-115">Not supported.</span></span>|
|<span data-ttu-id="59813-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="59813-116">Application</span></span>|<span data-ttu-id="59813-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59813-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59813-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59813-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/removeMembers
```

## <a name="request-headers"></a><span data-ttu-id="59813-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="59813-119">Request headers</span></span>
|<span data-ttu-id="59813-120">名称</span><span class="sxs-lookup"><span data-stu-id="59813-120">Name</span></span>|<span data-ttu-id="59813-121">说明</span><span class="sxs-lookup"><span data-stu-id="59813-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="59813-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="59813-122">Authorization</span></span>|<span data-ttu-id="59813-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="59813-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="59813-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59813-125">Content-Type</span></span>|<span data-ttu-id="59813-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="59813-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59813-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="59813-128">Request body</span></span>
<span data-ttu-id="59813-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59813-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="59813-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="59813-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="59813-131">参数</span><span class="sxs-lookup"><span data-stu-id="59813-131">Parameter</span></span>|<span data-ttu-id="59813-132">类型</span><span class="sxs-lookup"><span data-stu-id="59813-132">Type</span></span>|<span data-ttu-id="59813-133">说明</span><span class="sxs-lookup"><span data-stu-id="59813-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59813-134">assets</span><span class="sxs-lookup"><span data-stu-id="59813-134">assets</span></span>|<span data-ttu-id="59813-135">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="59813-135">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="59813-136">要 **作为 updatableAssetGroup** 成员删除的 **updatableAsset 资源的列表**。</span><span class="sxs-lookup"><span data-stu-id="59813-136">List of **updatableAsset** resources to remove as members of the **updatableAssetGroup**.</span></span>|

## <a name="response"></a><span data-ttu-id="59813-137">响应</span><span class="sxs-lookup"><span data-stu-id="59813-137">Response</span></span>

<span data-ttu-id="59813-138">如果成功，此操作返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="59813-138">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="59813-139">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="59813-139">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="59813-140">示例</span><span class="sxs-lookup"><span data-stu-id="59813-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="59813-141">请求</span><span class="sxs-lookup"><span data-stu-id="59813-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="59813-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="59813-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updatableassetgroup_removemembers"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/removeMembers
Content-Type: application/json

{
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="59813-143">C#</span><span class="sxs-lookup"><span data-stu-id="59813-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updatableassetgroup-removemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59813-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59813-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updatableassetgroup-removemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59813-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59813-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updatableassetgroup-removemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59813-146">Java</span><span class="sxs-lookup"><span data-stu-id="59813-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/updatableassetgroup-removemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="59813-147">响应</span><span class="sxs-lookup"><span data-stu-id="59813-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```
