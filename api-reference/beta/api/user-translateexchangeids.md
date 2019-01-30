---
title: 用户： translateExchangeIds
description: 对与 Outlook 相关的资源的标识符进行格式转换。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a00368c918685f6f94020dbea655232bae58ad57
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643613"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="0ddda-103">用户： translateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="0ddda-103">user: translateExchangeIds</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ddda-104">对与 Outlook 相关的资源的标识符进行格式转换。</span><span class="sxs-lookup"><span data-stu-id="0ddda-104">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ddda-105">权限</span><span class="sxs-lookup"><span data-stu-id="0ddda-105">Permissions</span></span>

<span data-ttu-id="0ddda-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ddda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0ddda-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ddda-108">Permission type</span></span> | <span data-ttu-id="0ddda-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ddda-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="0ddda-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ddda-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ddda-111">User.ReadBasic、 User.Read、 User.ReadWrite、 User.ReadBasic.All、 User.Read.All、 User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ddda-111">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="0ddda-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ddda-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ddda-113">User.ReadBasic，User.Read，User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ddda-113">User.ReadBasic, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="0ddda-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ddda-114">Application</span></span> | <span data-ttu-id="0ddda-115">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ddda-115">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ddda-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ddda-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="0ddda-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ddda-117">Request headers</span></span>

| <span data-ttu-id="0ddda-118">名称</span><span class="sxs-lookup"><span data-stu-id="0ddda-118">Name</span></span> | <span data-ttu-id="0ddda-119">值</span><span class="sxs-lookup"><span data-stu-id="0ddda-119">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="0ddda-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ddda-120">Authorization</span></span> | <span data-ttu-id="0ddda-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0ddda-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ddda-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ddda-123">Request body</span></span>

| <span data-ttu-id="0ddda-124">参数</span><span class="sxs-lookup"><span data-stu-id="0ddda-124">Parameter</span></span> | <span data-ttu-id="0ddda-125">类型</span><span class="sxs-lookup"><span data-stu-id="0ddda-125">Type</span></span> | <span data-ttu-id="0ddda-126">说明</span><span class="sxs-lookup"><span data-stu-id="0ddda-126">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="0ddda-127">inputIds</span><span class="sxs-lookup"><span data-stu-id="0ddda-127">inputIds</span></span> | <span data-ttu-id="0ddda-128">Edm.String 集合</span><span class="sxs-lookup"><span data-stu-id="0ddda-128">Edm.String collection</span></span> | <span data-ttu-id="0ddda-129">要转换的标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="0ddda-129">A collection of identifiers to convert.</span></span> <span data-ttu-id="0ddda-130">集合中的所有标识符必须具有相同的源 ID 类型，并且必须是同一邮箱中项目的。</span><span class="sxs-lookup"><span data-stu-id="0ddda-130">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="0ddda-131">此集合的最大大小是 1000年字符串。</span><span class="sxs-lookup"><span data-stu-id="0ddda-131">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="0ddda-132">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="0ddda-132">sourceIdType</span></span> | <span data-ttu-id="0ddda-133">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="0ddda-133">exchangeIdFormat</span></span> | <span data-ttu-id="0ddda-134">ID 类型的标识符的`InputIds`参数。</span><span class="sxs-lookup"><span data-stu-id="0ddda-134">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="0ddda-135">targetIdType</span><span class="sxs-lookup"><span data-stu-id="0ddda-135">targetIdType</span></span> | <span data-ttu-id="0ddda-136">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="0ddda-136">exchangeIdFormat</span></span> | <span data-ttu-id="0ddda-137">要转换的请求的 ID 类型。</span><span class="sxs-lookup"><span data-stu-id="0ddda-137">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="0ddda-138">exchangeIdFormat 值</span><span class="sxs-lookup"><span data-stu-id="0ddda-138">exchangeIdFormat values</span></span>

| <span data-ttu-id="0ddda-139">值</span><span class="sxs-lookup"><span data-stu-id="0ddda-139">Values</span></span> | <span data-ttu-id="0ddda-140">说明</span><span class="sxs-lookup"><span data-stu-id="0ddda-140">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="0ddda-141">entryId</span><span class="sxs-lookup"><span data-stu-id="0ddda-141">entryId</span></span> | <span data-ttu-id="0ddda-142">MAPI 客户端使用二进制条目 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="0ddda-142">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="0ddda-143">ewsId</span><span class="sxs-lookup"><span data-stu-id="0ddda-143">ewsId</span></span> | <span data-ttu-id="0ddda-144">使用 Exchange Web 服务客户端 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="0ddda-144">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="0ddda-145">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="0ddda-145">immutableEntryId</span></span> | <span data-ttu-id="0ddda-146">二进制 MAPI 兼容变 ID 的格式。</span><span class="sxs-lookup"><span data-stu-id="0ddda-146">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="0ddda-147">restId</span><span class="sxs-lookup"><span data-stu-id="0ddda-147">restId</span></span> | <span data-ttu-id="0ddda-148">由 Microsoft Graph 中使用的默认 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="0ddda-148">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="0ddda-149">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="0ddda-149">restImmutableEntryId</span></span> | <span data-ttu-id="0ddda-150">由 Microsoft Graph 变 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="0ddda-150">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="0ddda-151">二进制格式 (`entryId`和`immutableEntryId`) 的 URL 安全 base64 编码。</span><span class="sxs-lookup"><span data-stu-id="0ddda-151">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="0ddda-152">URL safeness 实现通过修改 base64 编码的二进制数据采用以下方式：</span><span class="sxs-lookup"><span data-stu-id="0ddda-152">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="0ddda-153">替换`+`与`-`</span><span class="sxs-lookup"><span data-stu-id="0ddda-153">Replace `+` with `-`</span></span>
- <span data-ttu-id="0ddda-154">替换`/`与`_`</span><span class="sxs-lookup"><span data-stu-id="0ddda-154">Replace `/` with `_`</span></span>
- <span data-ttu-id="0ddda-155">删除任何尾随空白字符 (`=`)</span><span class="sxs-lookup"><span data-stu-id="0ddda-155">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="0ddda-156">指示在原始了多少填充字符的字符串的末尾添加一个整数 (`0`， `1`，或`2`)</span><span class="sxs-lookup"><span data-stu-id="0ddda-156">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="0ddda-157">响应</span><span class="sxs-lookup"><span data-stu-id="0ddda-157">Response</span></span>

<span data-ttu-id="0ddda-158">如果成功，此方法返回`200 OK`响应代码和响应正文中的[convertIdResult](../resources/convertidresult.md)集合。</span><span class="sxs-lookup"><span data-stu-id="0ddda-158">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ddda-159">示例</span><span class="sxs-lookup"><span data-stu-id="0ddda-159">Example</span></span>

<span data-ttu-id="0ddda-160">下面的示例演示如何将多个标识符转换从普通的 REST API 格式 (`restId`) 为 REST 变格式 (`restImmutableEntryId`)。</span><span class="sxs-lookup"><span data-stu-id="0ddda-160">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="0ddda-161">请求</span><span class="sxs-lookup"><span data-stu-id="0ddda-161">Request</span></span>

<span data-ttu-id="0ddda-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0ddda-162">Here is the example request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0ddda-163">响应</span><span class="sxs-lookup"><span data-stu-id="0ddda-163">Response</span></span>

<span data-ttu-id="0ddda-164">下面是示例响应</span><span class="sxs-lookup"><span data-stu-id="0ddda-164">Here is the example response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
