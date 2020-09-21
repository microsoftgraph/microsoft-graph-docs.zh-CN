---
title: 应用程序： removePassword
description: 删除应用程序中的密码
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3b38007e3482e5cd35bf239deb8a6a823c99702e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968295"
---
# <a name="application-removepassword"></a><span data-ttu-id="a59e1-103">应用程序： removePassword</span><span class="sxs-lookup"><span data-stu-id="a59e1-103">application: removePassword</span></span>

<span data-ttu-id="a59e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a59e1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a59e1-105">删除 [应用程序](../resources/application.md)中的密码。</span><span class="sxs-lookup"><span data-stu-id="a59e1-105">Remove a password from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a59e1-106">权限</span><span class="sxs-lookup"><span data-stu-id="a59e1-106">Permissions</span></span>

<span data-ttu-id="a59e1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a59e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a59e1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a59e1-109">Permission type</span></span>                        | <span data-ttu-id="a59e1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a59e1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a59e1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a59e1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a59e1-112">Directory.accessasuser.all 的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="a59e1-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="a59e1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a59e1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a59e1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a59e1-114">Not supported.</span></span> |
| <span data-ttu-id="a59e1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a59e1-115">Application</span></span>                            | <span data-ttu-id="a59e1-116">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a59e1-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a59e1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a59e1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="a59e1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a59e1-118">Request headers</span></span>

| <span data-ttu-id="a59e1-119">名称</span><span class="sxs-lookup"><span data-stu-id="a59e1-119">Name</span></span>           | <span data-ttu-id="a59e1-120">说明</span><span class="sxs-lookup"><span data-stu-id="a59e1-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="a59e1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a59e1-121">Authorization</span></span>  | <span data-ttu-id="a59e1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a59e1-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a59e1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a59e1-124">Content-Type</span></span>   | <span data-ttu-id="a59e1-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a59e1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a59e1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a59e1-127">Request body</span></span>

| <span data-ttu-id="a59e1-128">属性</span><span class="sxs-lookup"><span data-stu-id="a59e1-128">Property</span></span>  | <span data-ttu-id="a59e1-129">类型</span><span class="sxs-lookup"><span data-stu-id="a59e1-129">Type</span></span> | <span data-ttu-id="a59e1-130">说明</span><span class="sxs-lookup"><span data-stu-id="a59e1-130">Description</span></span>|
|:----------|:-----|:-----------|
| <span data-ttu-id="a59e1-131">keyId</span><span class="sxs-lookup"><span data-stu-id="a59e1-131">keyId</span></span>     | <span data-ttu-id="a59e1-132">GUID</span><span class="sxs-lookup"><span data-stu-id="a59e1-132">GUID</span></span> | <span data-ttu-id="a59e1-133">密码的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a59e1-133">The unique identifier for the password.</span></span> <span data-ttu-id="a59e1-134">必需。</span><span class="sxs-lookup"><span data-stu-id="a59e1-134">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a59e1-135">响应</span><span class="sxs-lookup"><span data-stu-id="a59e1-135">Response</span></span>

<span data-ttu-id="a59e1-136">如果成功，此方法返回 `204 No content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a59e1-136">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a59e1-137">示例</span><span class="sxs-lookup"><span data-stu-id="a59e1-137">Examples</span></span>

<span data-ttu-id="a59e1-138">下面的示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="a59e1-138">The following is example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="a59e1-139">请求</span><span class="sxs-lookup"><span data-stu-id="a59e1-139">Request</span></span>

<span data-ttu-id="a59e1-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a59e1-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a59e1-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="a59e1-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_removepassword"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/removePassword
Content-type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6"
}
```
# <a name="c"></a>[<span data-ttu-id="a59e1-142">C#</span><span class="sxs-lookup"><span data-stu-id="a59e1-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-removepassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a59e1-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a59e1-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-removepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a59e1-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a59e1-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-removepassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a59e1-145">Java</span><span class="sxs-lookup"><span data-stu-id="a59e1-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-removepassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a59e1-146">响应</span><span class="sxs-lookup"><span data-stu-id="a59e1-146">Response</span></span>

<span data-ttu-id="a59e1-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a59e1-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordCredential"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: removePassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

