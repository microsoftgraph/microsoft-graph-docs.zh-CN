---
title: user： translateExchangeIds
description: 对与 Outlook 相关的资源的标识符进行格式转换。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4bdb22f649cc0fd30734b5762106c959c34e3cf6
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176974"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="62406-103">user： translateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="62406-103">user: translateExchangeIds</span></span>

<span data-ttu-id="62406-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62406-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62406-105">对与 Outlook 相关的资源的标识符进行格式转换。</span><span class="sxs-lookup"><span data-stu-id="62406-105">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="62406-106">权限</span><span class="sxs-lookup"><span data-stu-id="62406-106">Permissions</span></span>

<span data-ttu-id="62406-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62406-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62406-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="62406-109">Permission type</span></span> | <span data-ttu-id="62406-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62406-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="62406-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62406-111">Delegated (work or school account)</span></span> | <span data-ttu-id="62406-112">User.ReadBasic.All、User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62406-112">User.ReadBasic.All, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="62406-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62406-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62406-114">User.ReadBasic.All、User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62406-114">User.ReadBasic.All, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="62406-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="62406-115">Application</span></span> | <span data-ttu-id="62406-116">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62406-116">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62406-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62406-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="62406-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="62406-118">Request headers</span></span>

| <span data-ttu-id="62406-119">名称</span><span class="sxs-lookup"><span data-stu-id="62406-119">Name</span></span> | <span data-ttu-id="62406-120">值</span><span class="sxs-lookup"><span data-stu-id="62406-120">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="62406-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="62406-121">Authorization</span></span> | <span data-ttu-id="62406-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="62406-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62406-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="62406-124">Request body</span></span>

| <span data-ttu-id="62406-125">参数</span><span class="sxs-lookup"><span data-stu-id="62406-125">Parameter</span></span> | <span data-ttu-id="62406-126">类型</span><span class="sxs-lookup"><span data-stu-id="62406-126">Type</span></span> | <span data-ttu-id="62406-127">说明</span><span class="sxs-lookup"><span data-stu-id="62406-127">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="62406-128">inputIds</span><span class="sxs-lookup"><span data-stu-id="62406-128">inputIds</span></span> | <span data-ttu-id="62406-129">字符串集合</span><span class="sxs-lookup"><span data-stu-id="62406-129">String collection</span></span> | <span data-ttu-id="62406-130">要转换的标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="62406-130">A collection of identifiers to convert.</span></span> <span data-ttu-id="62406-131">集合中所有标识符都必须具有相同的源 ID 类型，并且必须为同一邮箱中的项目。</span><span class="sxs-lookup"><span data-stu-id="62406-131">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="62406-132">此集合的最大大小为 1000 个字符串。</span><span class="sxs-lookup"><span data-stu-id="62406-132">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="62406-133">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="62406-133">sourceIdType</span></span> | <span data-ttu-id="62406-134">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="62406-134">exchangeIdFormat</span></span> | <span data-ttu-id="62406-135">参数中标识符的 ID `InputIds` 类型。</span><span class="sxs-lookup"><span data-stu-id="62406-135">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="62406-136">targetIdType</span><span class="sxs-lookup"><span data-stu-id="62406-136">targetIdType</span></span> | <span data-ttu-id="62406-137">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="62406-137">exchangeIdFormat</span></span> | <span data-ttu-id="62406-138">要转换为的请求 ID 类型。</span><span class="sxs-lookup"><span data-stu-id="62406-138">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="62406-139">exchangeIdFormat 值</span><span class="sxs-lookup"><span data-stu-id="62406-139">exchangeIdFormat values</span></span>

| <span data-ttu-id="62406-140">成员</span><span class="sxs-lookup"><span data-stu-id="62406-140">Member</span></span> | <span data-ttu-id="62406-141">说明</span><span class="sxs-lookup"><span data-stu-id="62406-141">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="62406-142">entryId</span><span class="sxs-lookup"><span data-stu-id="62406-142">entryId</span></span> | <span data-ttu-id="62406-143">MAPI 客户端使用的二进制条目 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="62406-143">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="62406-144">ewsId</span><span class="sxs-lookup"><span data-stu-id="62406-144">ewsId</span></span> | <span data-ttu-id="62406-145">Exchange Web 服务客户端使用的 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="62406-145">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="62406-146">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="62406-146">immutableEntryId</span></span> | <span data-ttu-id="62406-147">二进制 MAPI 兼容不可变 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="62406-147">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="62406-148">restId</span><span class="sxs-lookup"><span data-stu-id="62406-148">restId</span></span> | <span data-ttu-id="62406-149">Microsoft Graph 使用的默认 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="62406-149">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="62406-150">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="62406-150">restImmutableEntryId</span></span> | <span data-ttu-id="62406-151">Microsoft Graph 使用的不可变 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="62406-151">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="62406-152">二进制格式 `entryId` () `immutableEntryId` URL 安全 base64 编码。</span><span class="sxs-lookup"><span data-stu-id="62406-152">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="62406-153">URL 安全性通过按以下方式修改二进制数据的 base64 编码实现：</span><span class="sxs-lookup"><span data-stu-id="62406-153">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="62406-154">替换为 `+``-`</span><span class="sxs-lookup"><span data-stu-id="62406-154">Replace `+` with `-`</span></span>
- <span data-ttu-id="62406-155">替换为 `/``_`</span><span class="sxs-lookup"><span data-stu-id="62406-155">Replace `/` with `_`</span></span>
- <span data-ttu-id="62406-156">删除所有尾部填充 `=` () </span><span class="sxs-lookup"><span data-stu-id="62406-156">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="62406-157">将一个整数添加到字符串的末尾，指示原始文本中填充字符 (， `0` `1` `2` 或) </span><span class="sxs-lookup"><span data-stu-id="62406-157">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="62406-158">响应</span><span class="sxs-lookup"><span data-stu-id="62406-158">Response</span></span>

<span data-ttu-id="62406-159">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [convertIdResult](../resources/convertidresult.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="62406-159">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62406-160">示例</span><span class="sxs-lookup"><span data-stu-id="62406-160">Example</span></span>

<span data-ttu-id="62406-161">以下示例演示如何将常规 REST API 格式的多个标识符 () REST 不可变格式 `restId` `restImmutableEntryId` () 。</span><span class="sxs-lookup"><span data-stu-id="62406-161">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="62406-162">请求</span><span class="sxs-lookup"><span data-stu-id="62406-162">Request</span></span>

<span data-ttu-id="62406-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="62406-163">Here is the example request.</span></span>

# <a name="http"></a>[<span data-ttu-id="62406-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="62406-164">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="62406-165">C#</span><span class="sxs-lookup"><span data-stu-id="62406-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-translateexchangeids-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62406-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62406-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-translateexchangeids-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62406-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62406-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-translateexchangeids-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="62406-168">Java</span><span class="sxs-lookup"><span data-stu-id="62406-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-translateexchangeids-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="62406-169">响应</span><span class="sxs-lookup"><span data-stu-id="62406-169">Response</span></span>

<span data-ttu-id="62406-170">下面是示例响应</span><span class="sxs-lookup"><span data-stu-id="62406-170">Here is the example response</span></span>
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


