---
title: 用户： translateExchangeIds
description: 对与 Outlook 相关的资源的标识符进行格式转换。
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ae26f5b5a5a109145daa132837890943a98c8c0d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451624"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="0c2cd-103">用户： translateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="0c2cd-103">user: translateExchangeIds</span></span>

<span data-ttu-id="0c2cd-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0c2cd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c2cd-105">对与 Outlook 相关的资源的标识符进行格式转换。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-105">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c2cd-106">权限</span><span class="sxs-lookup"><span data-stu-id="0c2cd-106">Permissions</span></span>

<span data-ttu-id="0c2cd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0c2cd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c2cd-109">Permission type</span></span> | <span data-ttu-id="0c2cd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0c2cd-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="0c2cd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c2cd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0c2cd-112">User.readbasic.all，User.readbasic.all，user. all，user. all，All，All，All，All。 all</span><span class="sxs-lookup"><span data-stu-id="0c2cd-112">User.ReadBasic.All, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="0c2cd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c2cd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c2cd-114">User.readbasic.all、用户读取、用户读写</span><span class="sxs-lookup"><span data-stu-id="0c2cd-114">User.ReadBasic.All, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="0c2cd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c2cd-115">Application</span></span> | <span data-ttu-id="0c2cd-116">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c2cd-116">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c2cd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c2cd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="0c2cd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c2cd-118">Request headers</span></span>

| <span data-ttu-id="0c2cd-119">名称</span><span class="sxs-lookup"><span data-stu-id="0c2cd-119">Name</span></span> | <span data-ttu-id="0c2cd-120">值</span><span class="sxs-lookup"><span data-stu-id="0c2cd-120">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="0c2cd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c2cd-121">Authorization</span></span> | <span data-ttu-id="0c2cd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c2cd-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c2cd-124">Request body</span></span>

| <span data-ttu-id="0c2cd-125">参数</span><span class="sxs-lookup"><span data-stu-id="0c2cd-125">Parameter</span></span> | <span data-ttu-id="0c2cd-126">类型</span><span class="sxs-lookup"><span data-stu-id="0c2cd-126">Type</span></span> | <span data-ttu-id="0c2cd-127">说明</span><span class="sxs-lookup"><span data-stu-id="0c2cd-127">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="0c2cd-128">inputIds</span><span class="sxs-lookup"><span data-stu-id="0c2cd-128">inputIds</span></span> | <span data-ttu-id="0c2cd-129">String 集合</span><span class="sxs-lookup"><span data-stu-id="0c2cd-129">String collection</span></span> | <span data-ttu-id="0c2cd-130">要转换的标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-130">A collection of identifiers to convert.</span></span> <span data-ttu-id="0c2cd-131">集合中的所有标识符必须具有相同的源 ID 类型，并且必须是同一邮箱中的项目。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-131">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="0c2cd-132">此集合的最大大小为1000个字符串。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-132">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="0c2cd-133">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="0c2cd-133">sourceIdType</span></span> | <span data-ttu-id="0c2cd-134">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="0c2cd-134">exchangeIdFormat</span></span> | <span data-ttu-id="0c2cd-135">`InputIds`参数中标识符的 ID 类型。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-135">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="0c2cd-136">targetIdType</span><span class="sxs-lookup"><span data-stu-id="0c2cd-136">targetIdType</span></span> | <span data-ttu-id="0c2cd-137">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="0c2cd-137">exchangeIdFormat</span></span> | <span data-ttu-id="0c2cd-138">要转换为的请求的 ID 类型。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-138">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="0c2cd-139">exchangeIdFormat 值</span><span class="sxs-lookup"><span data-stu-id="0c2cd-139">exchangeIdFormat values</span></span>

| <span data-ttu-id="0c2cd-140">值</span><span class="sxs-lookup"><span data-stu-id="0c2cd-140">Values</span></span> | <span data-ttu-id="0c2cd-141">说明</span><span class="sxs-lookup"><span data-stu-id="0c2cd-141">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="0c2cd-142">entryId</span><span class="sxs-lookup"><span data-stu-id="0c2cd-142">entryId</span></span> | <span data-ttu-id="0c2cd-143">MAPI 客户端使用的二进制条目 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-143">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="0c2cd-144">ewsId</span><span class="sxs-lookup"><span data-stu-id="0c2cd-144">ewsId</span></span> | <span data-ttu-id="0c2cd-145">Exchange Web 服务客户端使用的 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-145">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="0c2cd-146">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="0c2cd-146">immutableEntryId</span></span> | <span data-ttu-id="0c2cd-147">二进制 MAPI 兼容的不可变 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-147">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="0c2cd-148">restId</span><span class="sxs-lookup"><span data-stu-id="0c2cd-148">restId</span></span> | <span data-ttu-id="0c2cd-149">Microsoft Graph 使用的默认 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-149">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="0c2cd-150">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="0c2cd-150">restImmutableEntryId</span></span> | <span data-ttu-id="0c2cd-151">Microsoft Graph 使用的不可变 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-151">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="0c2cd-152">二进制格式（`entryId`和`immutableEntryId`）是 URL 安全的 base64 编码。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-152">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="0c2cd-153">URL-safeness 通过以下方式修改二进制数据的 base64 编码实现：</span><span class="sxs-lookup"><span data-stu-id="0c2cd-153">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="0c2cd-154">替换`+`为`-`</span><span class="sxs-lookup"><span data-stu-id="0c2cd-154">Replace `+` with `-`</span></span>
- <span data-ttu-id="0c2cd-155">替换`/`为`_`</span><span class="sxs-lookup"><span data-stu-id="0c2cd-155">Replace `/` with `_`</span></span>
- <span data-ttu-id="0c2cd-156">删除任何尾部填充字符（`=`）</span><span class="sxs-lookup"><span data-stu-id="0c2cd-156">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="0c2cd-157">在字符串末尾添加一个整数，指示原始字符（`0`、 `1`或`2`）中的填充字符数</span><span class="sxs-lookup"><span data-stu-id="0c2cd-157">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="0c2cd-158">响应</span><span class="sxs-lookup"><span data-stu-id="0c2cd-158">Response</span></span>

<span data-ttu-id="0c2cd-159">如果成功，此方法在`200 OK`响应正文中返回响应代码和[convertIdResult](../resources/convertidresult.md)集合。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-159">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c2cd-160">示例</span><span class="sxs-lookup"><span data-stu-id="0c2cd-160">Example</span></span>

<span data-ttu-id="0c2cd-161">下面的示例演示如何将多个标识符从正常的 REST API 格式（`restId`）转换为 REST 不可变格式`restImmutableEntryId`（）。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-161">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="0c2cd-162">请求</span><span class="sxs-lookup"><span data-stu-id="0c2cd-162">Request</span></span>

<span data-ttu-id="0c2cd-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-163">Here is the example request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0c2cd-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c2cd-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_translateexchangeids"
}-->

```http
POST https://graph.microsoft.com/beta/me/translateExchangeIds
Content-Type: application/json

{
  "inputIds" : [
    "{rest-formatted-id-1}",
    "{rest-formatted-id-2}"
  ],
  "sourceIdType": "restId",
  "targetIdType": "restImmutableEntryId"
}
```
# <a name="c"></a>[<span data-ttu-id="0c2cd-165">C#</span><span class="sxs-lookup"><span data-stu-id="0c2cd-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-translateexchangeids-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0c2cd-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c2cd-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-translateexchangeids-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0c2cd-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0c2cd-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-translateexchangeids-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0c2cd-168">响应</span><span class="sxs-lookup"><span data-stu-id="0c2cd-168">Response</span></span>

<span data-ttu-id="0c2cd-169">下面是示例响应</span><span class="sxs-lookup"><span data-stu-id="0c2cd-169">Here is the example response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.convertIdResult",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "sourceId": "{rest-formatted-id-1}",
      "targetId": "{rest-immutable-formatted-id-1}"
    },
    {
      "sourceId": "{rest-formatted-id-2}",
      "targetId": "{rest-immutable-formatted-id-2}"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
