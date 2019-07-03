---
title: '用户: translateExchangeIds'
description: 对与 Outlook 相关的资源的标识符进行格式转换。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 399792e21a0d32adc90b7693d8d6addcc0328647
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456678"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="6e4c2-103">用户: translateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="6e4c2-103">user: translateExchangeIds</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e4c2-104">对与 Outlook 相关的资源的标识符进行格式转换。</span><span class="sxs-lookup"><span data-stu-id="6e4c2-104">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e4c2-105">权限</span><span class="sxs-lookup"><span data-stu-id="6e4c2-105">Permissions</span></span>

<span data-ttu-id="6e4c2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e4c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e4c2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e4c2-108">Permission type</span></span> | <span data-ttu-id="6e4c2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e4c2-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="6e4c2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e4c2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6e4c2-111">User.readbasic.all, user. User.readbasic.all, user. all, All, user. all, All: all</span><span class="sxs-lookup"><span data-stu-id="6e4c2-111">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="6e4c2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e4c2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e4c2-113">User.readbasic.all、用户读取、用户读写</span><span class="sxs-lookup"><span data-stu-id="6e4c2-113">User.ReadBasic, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="6e4c2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e4c2-114">Application</span></span> | <span data-ttu-id="6e4c2-115">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e4c2-115">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e4c2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e4c2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="6e4c2-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e4c2-117">Request headers</span></span>

| <span data-ttu-id="6e4c2-118">名称</span><span class="sxs-lookup"><span data-stu-id="6e4c2-118">Name</span></span> | <span data-ttu-id="6e4c2-119">值</span><span class="sxs-lookup"><span data-stu-id="6e4c2-119">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="6e4c2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e4c2-120">Authorization</span></span> | <span data-ttu-id="6e4c2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e4c2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e4c2-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e4c2-123">Request body</span></span>

| <span data-ttu-id="6e4c2-124">参数</span><span class="sxs-lookup"><span data-stu-id="6e4c2-124">Parameter</span></span> | <span data-ttu-id="6e4c2-125">类型</span><span class="sxs-lookup"><span data-stu-id="6e4c2-125">Type</span></span> | <span data-ttu-id="6e4c2-126">说明</span><span class="sxs-lookup"><span data-stu-id="6e4c2-126">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="6e4c2-127">inputIds</span><span class="sxs-lookup"><span data-stu-id="6e4c2-127">inputIds</span></span> | <span data-ttu-id="6e4c2-128">String collection</span><span class="sxs-lookup"><span data-stu-id="6e4c2-128">String collection</span></span> | <span data-ttu-id="6e4c2-129">要转换的标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="6e4c2-129">A collection of identifiers to convert.</span></span> <span data-ttu-id="6e4c2-130">集合中的所有标识符必须具有相同的源 ID 类型, 并且必须是同一邮箱中的项目。</span><span class="sxs-lookup"><span data-stu-id="6e4c2-130">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="6e4c2-131">此集合的最大大小为1000个字符串。</span><span class="sxs-lookup"><span data-stu-id="6e4c2-131">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="6e4c2-132">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="6e4c2-132">sourceIdType</span></span> | <span data-ttu-id="6e4c2-133">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="6e4c2-133">exchangeIdFormat</span></span> | <span data-ttu-id="6e4c2-134">`InputIds`参数中标识符的 ID 类型。</span><span class="sxs-lookup"><span data-stu-id="6e4c2-134">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="6e4c2-135">targetIdType</span><span class="sxs-lookup"><span data-stu-id="6e4c2-135">targetIdType</span></span> | <span data-ttu-id="6e4c2-136">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="6e4c2-136">exchangeIdFormat</span></span> | <span data-ttu-id="6e4c2-137">要转换为的请求的 ID 类型。</span><span class="sxs-lookup"><span data-stu-id="6e4c2-137">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="6e4c2-138">exchangeIdFormat 值</span><span class="sxs-lookup"><span data-stu-id="6e4c2-138">exchangeIdFormat values</span></span>

| <span data-ttu-id="6e4c2-139">值</span><span class="sxs-lookup"><span data-stu-id="6e4c2-139">Values</span></span> | <span data-ttu-id="6e4c2-140">说明</span><span class="sxs-lookup"><span data-stu-id="6e4c2-140">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="6e4c2-141">entryId</span><span class="sxs-lookup"><span data-stu-id="6e4c2-141">entryId</span></span> | <span data-ttu-id="6e4c2-142">MAPI 客户端使用的二进制条目 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="6e4c2-142">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="6e4c2-143">ewsId</span><span class="sxs-lookup"><span data-stu-id="6e4c2-143">ewsId</span></span> | <span data-ttu-id="6e4c2-144">Exchange Web 服务客户端使用的 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="6e4c2-144">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="6e4c2-145">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="6e4c2-145">immutableEntryId</span></span> | <span data-ttu-id="6e4c2-146">二进制 MAPI 兼容的不可变 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="6e4c2-146">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="6e4c2-147">restId</span><span class="sxs-lookup"><span data-stu-id="6e4c2-147">restId</span></span> | <span data-ttu-id="6e4c2-148">Microsoft Graph 使用的默认 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="6e4c2-148">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="6e4c2-149">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="6e4c2-149">restImmutableEntryId</span></span> | <span data-ttu-id="6e4c2-150">Microsoft Graph 使用的不可变 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="6e4c2-150">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="6e4c2-151">二进制格式 (`entryId`和`immutableEntryId`) 是 URL 安全的 base64 编码。</span><span class="sxs-lookup"><span data-stu-id="6e4c2-151">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="6e4c2-152">URL-safeness 通过以下方式修改二进制数据的 base64 编码实现:</span><span class="sxs-lookup"><span data-stu-id="6e4c2-152">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="6e4c2-153">替换`+`为`-`</span><span class="sxs-lookup"><span data-stu-id="6e4c2-153">Replace `+` with `-`</span></span>
- <span data-ttu-id="6e4c2-154">替换`/`为`_`</span><span class="sxs-lookup"><span data-stu-id="6e4c2-154">Replace `/` with `_`</span></span>
- <span data-ttu-id="6e4c2-155">删除任何尾部填充字符 (`=`)</span><span class="sxs-lookup"><span data-stu-id="6e4c2-155">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="6e4c2-156">在字符串末尾添加一个整数, 指示原始字符 (`0`、 `1`或`2`) 中的填充字符数</span><span class="sxs-lookup"><span data-stu-id="6e4c2-156">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="6e4c2-157">响应</span><span class="sxs-lookup"><span data-stu-id="6e4c2-157">Response</span></span>

<span data-ttu-id="6e4c2-158">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[convertIdResult](../resources/convertidresult.md)集合。</span><span class="sxs-lookup"><span data-stu-id="6e4c2-158">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e4c2-159">示例</span><span class="sxs-lookup"><span data-stu-id="6e4c2-159">Example</span></span>

<span data-ttu-id="6e4c2-160">下面的示例演示如何将多个标识符从正常的 REST API 格式 (`restId`) 转换为 REST 不可变格式`restImmutableEntryId`()。</span><span class="sxs-lookup"><span data-stu-id="6e4c2-160">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="6e4c2-161">请求</span><span class="sxs-lookup"><span data-stu-id="6e4c2-161">Request</span></span>

<span data-ttu-id="6e4c2-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6e4c2-162">Here is the example request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6e4c2-163">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="6e4c2-163">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6e4c2-164">C#</span><span class="sxs-lookup"><span data-stu-id="6e4c2-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-translateexchangeids-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6e4c2-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="6e4c2-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-translateexchangeids-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6e4c2-166">目标-C</span><span class="sxs-lookup"><span data-stu-id="6e4c2-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-translateexchangeids-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6e4c2-167">响应</span><span class="sxs-lookup"><span data-stu-id="6e4c2-167">Response</span></span>

<span data-ttu-id="6e4c2-168">下面是示例响应</span><span class="sxs-lookup"><span data-stu-id="6e4c2-168">Here is the example response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.convertIdResult",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/testexchangebeta/$metadata#Collection(microsoft.graph.convertIdResult)",
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
