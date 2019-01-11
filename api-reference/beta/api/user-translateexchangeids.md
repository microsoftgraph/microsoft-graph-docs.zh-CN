---
title: 用户： translateExchangeIds
description: 翻译格式之间的 Outlook 相关的资源的标识符。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: b59cc33765586648432736df6067e6c089318729
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831904"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="debcc-103">用户： translateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="debcc-103">user: translateExchangeIds</span></span>

> <span data-ttu-id="debcc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="debcc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="debcc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="debcc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="debcc-106">翻译格式之间的 Outlook 相关的资源的标识符。</span><span class="sxs-lookup"><span data-stu-id="debcc-106">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="debcc-107">权限</span><span class="sxs-lookup"><span data-stu-id="debcc-107">Permissions</span></span>

<span data-ttu-id="debcc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="debcc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="debcc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="debcc-110">Permission type</span></span> | <span data-ttu-id="debcc-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="debcc-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="debcc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="debcc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="debcc-113">User.ReadBasic、 User.Read、 User.ReadWrite、 User.ReadBasic.All、 User.Read.All、 User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="debcc-113">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="debcc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="debcc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="debcc-115">User.ReadBasic，User.Read，User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="debcc-115">User.ReadBasic, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="debcc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="debcc-116">Application</span></span> | <span data-ttu-id="debcc-117">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="debcc-117">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="debcc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="debcc-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="debcc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="debcc-119">Request headers</span></span>

| <span data-ttu-id="debcc-120">名称</span><span class="sxs-lookup"><span data-stu-id="debcc-120">Name</span></span> | <span data-ttu-id="debcc-121">值</span><span class="sxs-lookup"><span data-stu-id="debcc-121">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="debcc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="debcc-122">Authorization</span></span> | <span data-ttu-id="debcc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="debcc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="debcc-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="debcc-125">Request body</span></span>

| <span data-ttu-id="debcc-126">参数</span><span class="sxs-lookup"><span data-stu-id="debcc-126">Parameter</span></span> | <span data-ttu-id="debcc-127">类型</span><span class="sxs-lookup"><span data-stu-id="debcc-127">Type</span></span> | <span data-ttu-id="debcc-128">Description</span><span class="sxs-lookup"><span data-stu-id="debcc-128">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="debcc-129">inputIds</span><span class="sxs-lookup"><span data-stu-id="debcc-129">inputIds</span></span> | <span data-ttu-id="debcc-130">Edm.String 集合</span><span class="sxs-lookup"><span data-stu-id="debcc-130">Edm.String collection</span></span> | <span data-ttu-id="debcc-131">要转换的标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="debcc-131">A collection of identifiers to convert.</span></span> <span data-ttu-id="debcc-132">集合中的所有标识符必须具有相同的源 ID 类型，并且必须是同一邮箱中项目的。</span><span class="sxs-lookup"><span data-stu-id="debcc-132">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="debcc-133">此集合的最大大小是 1000年字符串。</span><span class="sxs-lookup"><span data-stu-id="debcc-133">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="debcc-134">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="debcc-134">sourceIdType</span></span> | <span data-ttu-id="debcc-135">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="debcc-135">exchangeIdFormat</span></span> | <span data-ttu-id="debcc-136">ID 类型的标识符的`InputIds`参数。</span><span class="sxs-lookup"><span data-stu-id="debcc-136">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="debcc-137">targetIdType</span><span class="sxs-lookup"><span data-stu-id="debcc-137">targetIdType</span></span> | <span data-ttu-id="debcc-138">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="debcc-138">exchangeIdFormat</span></span> | <span data-ttu-id="debcc-139">要转换的请求的 ID 类型。</span><span class="sxs-lookup"><span data-stu-id="debcc-139">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="debcc-140">exchangeIdFormat 值</span><span class="sxs-lookup"><span data-stu-id="debcc-140">exchangeIdFormat values</span></span>

| <span data-ttu-id="debcc-141">值</span><span class="sxs-lookup"><span data-stu-id="debcc-141">Values</span></span> | <span data-ttu-id="debcc-142">说明</span><span class="sxs-lookup"><span data-stu-id="debcc-142">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="debcc-143">entryId</span><span class="sxs-lookup"><span data-stu-id="debcc-143">entryId</span></span> | <span data-ttu-id="debcc-144">MAPI 客户端使用二进制条目 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="debcc-144">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="debcc-145">ewsId</span><span class="sxs-lookup"><span data-stu-id="debcc-145">ewsId</span></span> | <span data-ttu-id="debcc-146">使用 Exchange Web 服务客户端 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="debcc-146">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="debcc-147">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="debcc-147">immutableEntryId</span></span> | <span data-ttu-id="debcc-148">二进制 MAPI 兼容变 ID 的格式。</span><span class="sxs-lookup"><span data-stu-id="debcc-148">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="debcc-149">restId</span><span class="sxs-lookup"><span data-stu-id="debcc-149">restId</span></span> | <span data-ttu-id="debcc-150">由 Microsoft Graph 中使用的默认 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="debcc-150">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="debcc-151">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="debcc-151">restImmutableEntryId</span></span> | <span data-ttu-id="debcc-152">由 Microsoft Graph 变 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="debcc-152">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="debcc-153">二进制格式 (`entryId`和`immutableEntryId`) 的 URL 安全 base64 编码。</span><span class="sxs-lookup"><span data-stu-id="debcc-153">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="debcc-154">URL safeness 实现通过修改 base64 编码的二进制数据采用以下方式：</span><span class="sxs-lookup"><span data-stu-id="debcc-154">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="debcc-155">替换`+`与`-`</span><span class="sxs-lookup"><span data-stu-id="debcc-155">Replace `+` with `-`</span></span>
- <span data-ttu-id="debcc-156">替换`/`与`_`</span><span class="sxs-lookup"><span data-stu-id="debcc-156">Replace `/` with `_`</span></span>
- <span data-ttu-id="debcc-157">删除任何尾随空白字符 (`=`)</span><span class="sxs-lookup"><span data-stu-id="debcc-157">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="debcc-158">指示在原始了多少填充字符的字符串的末尾添加一个整数 (`0`， `1`，或`2`)</span><span class="sxs-lookup"><span data-stu-id="debcc-158">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="debcc-159">响应</span><span class="sxs-lookup"><span data-stu-id="debcc-159">Response</span></span>

<span data-ttu-id="debcc-160">如果成功，此方法返回`200 OK`响应代码和响应正文中的[convertIdResult](../resources/convertidresult.md)集合。</span><span class="sxs-lookup"><span data-stu-id="debcc-160">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="debcc-161">示例</span><span class="sxs-lookup"><span data-stu-id="debcc-161">Example</span></span>

<span data-ttu-id="debcc-162">下面的示例演示如何将多个标识符转换从普通的 REST API 格式 (`restId`) 为 REST 变格式 (`restImmutableEntryId`)。</span><span class="sxs-lookup"><span data-stu-id="debcc-162">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="debcc-163">请求</span><span class="sxs-lookup"><span data-stu-id="debcc-163">Request</span></span>

<span data-ttu-id="debcc-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="debcc-164">Here is the example request.</span></span>
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

### <a name="response"></a><span data-ttu-id="debcc-165">响应</span><span class="sxs-lookup"><span data-stu-id="debcc-165">Response</span></span>

<span data-ttu-id="debcc-166">下面是示例响应</span><span class="sxs-lookup"><span data-stu-id="debcc-166">Here is the example response</span></span>
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
      "sourceId": "{rest-formatted-id-1},
      "targetId": "{rest-immutable-formatted-id-1}"
    },
    {
      "sourceId": "{rest-formatted-id-2},
      "targetId": "{rest-immutable-formatted-id-2}"
    }
  ]
}
```
