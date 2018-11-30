---
title: 用户： translateExchangeIds
description: 翻译格式之间的 Outlook 相关的资源的标识符。
ms.openlocfilehash: 0c6e74ad0bb9676f261ed0202757b1e036b09c85
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045916"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="863d8-103">用户： translateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="863d8-103">user: translateExchangeIds</span></span>

> <span data-ttu-id="863d8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="863d8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="863d8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="863d8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="863d8-106">翻译格式之间的 Outlook 相关的资源的标识符。</span><span class="sxs-lookup"><span data-stu-id="863d8-106">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="863d8-107">权限</span><span class="sxs-lookup"><span data-stu-id="863d8-107">Permissions</span></span>

<span data-ttu-id="863d8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="863d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="863d8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="863d8-110">Permission type</span></span> | <span data-ttu-id="863d8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="863d8-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="863d8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="863d8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="863d8-113">User.ReadBasic、 User.Read、 User.ReadWrite、 User.ReadBasic.All、 User.Read.All、 User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="863d8-113">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="863d8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="863d8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="863d8-115">User.ReadBasic，User.Read，User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="863d8-115">User.ReadBasic, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="863d8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="863d8-116">Application</span></span> | <span data-ttu-id="863d8-117">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="863d8-117">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="863d8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="863d8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="863d8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="863d8-119">Request headers</span></span>

| <span data-ttu-id="863d8-120">名称</span><span class="sxs-lookup"><span data-stu-id="863d8-120">Name</span></span> | <span data-ttu-id="863d8-121">值</span><span class="sxs-lookup"><span data-stu-id="863d8-121">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="863d8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="863d8-122">Authorization</span></span> | <span data-ttu-id="863d8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="863d8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="863d8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="863d8-125">Request body</span></span>

| <span data-ttu-id="863d8-126">参数</span><span class="sxs-lookup"><span data-stu-id="863d8-126">Parameter</span></span> | <span data-ttu-id="863d8-127">类型</span><span class="sxs-lookup"><span data-stu-id="863d8-127">Type</span></span> | <span data-ttu-id="863d8-128">说明</span><span class="sxs-lookup"><span data-stu-id="863d8-128">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="863d8-129">inputIds</span><span class="sxs-lookup"><span data-stu-id="863d8-129">inputIds</span></span> | <span data-ttu-id="863d8-130">Edm.String 集合</span><span class="sxs-lookup"><span data-stu-id="863d8-130">Edm.String collection</span></span> | <span data-ttu-id="863d8-131">要转换的标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="863d8-131">A collection of identifiers to convert.</span></span> <span data-ttu-id="863d8-132">集合中的所有标识符必须具有相同的源 ID 类型，并且必须是同一邮箱中项目的。</span><span class="sxs-lookup"><span data-stu-id="863d8-132">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="863d8-133">此集合的最大大小是 1000年字符串。</span><span class="sxs-lookup"><span data-stu-id="863d8-133">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="863d8-134">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="863d8-134">sourceIdType</span></span> | <span data-ttu-id="863d8-135">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="863d8-135">exchangeIdFormat</span></span> | <span data-ttu-id="863d8-136">ID 类型的标识符的`InputIds`参数。</span><span class="sxs-lookup"><span data-stu-id="863d8-136">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="863d8-137">targetIdType</span><span class="sxs-lookup"><span data-stu-id="863d8-137">targetIdType</span></span> | <span data-ttu-id="863d8-138">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="863d8-138">exchangeIdFormat</span></span> | <span data-ttu-id="863d8-139">要转换的请求的 ID 类型。</span><span class="sxs-lookup"><span data-stu-id="863d8-139">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="863d8-140">exchangeIdFormat 值</span><span class="sxs-lookup"><span data-stu-id="863d8-140">exchangeIdFormat values</span></span>

| <span data-ttu-id="863d8-141">值</span><span class="sxs-lookup"><span data-stu-id="863d8-141">Values</span></span> | <span data-ttu-id="863d8-142">说明</span><span class="sxs-lookup"><span data-stu-id="863d8-142">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="863d8-143">entryId</span><span class="sxs-lookup"><span data-stu-id="863d8-143">entryId</span></span> | <span data-ttu-id="863d8-144">MAPI 客户端使用二进制条目 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="863d8-144">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="863d8-145">ewsId</span><span class="sxs-lookup"><span data-stu-id="863d8-145">ewsId</span></span> | <span data-ttu-id="863d8-146">使用 Exchange Web 服务客户端 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="863d8-146">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="863d8-147">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="863d8-147">immutableEntryId</span></span> | <span data-ttu-id="863d8-148">MAPI 兼容变 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="863d8-148">The MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="863d8-149">restId</span><span class="sxs-lookup"><span data-stu-id="863d8-149">restId</span></span> | <span data-ttu-id="863d8-150">由 Microsoft Graph 中使用的默认 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="863d8-150">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="863d8-151">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="863d8-151">restImmutableEntryId</span></span> | <span data-ttu-id="863d8-152">由 Microsoft Graph 变 ID 格式。</span><span class="sxs-lookup"><span data-stu-id="863d8-152">The immutable ID format used by Microsoft Graph.</span></span> |

## <a name="response"></a><span data-ttu-id="863d8-153">响应</span><span class="sxs-lookup"><span data-stu-id="863d8-153">Response</span></span>

<span data-ttu-id="863d8-154">如果成功，此方法返回`200 OK`响应代码和响应正文中的[convertIdResult](../resources/meetingtimesuggestionsresult.md)集合。</span><span class="sxs-lookup"><span data-stu-id="863d8-154">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/meetingtimesuggestionsresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="863d8-155">示例</span><span class="sxs-lookup"><span data-stu-id="863d8-155">Example</span></span>

<span data-ttu-id="863d8-156">下面的示例演示如何将多个标识符转换从普通的 REST API 格式 (`restId`) 为 REST 变格式 (`restImmutableEntryId`)。</span><span class="sxs-lookup"><span data-stu-id="863d8-156">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

##### <a name="request"></a><span data-ttu-id="863d8-157">请求</span><span class="sxs-lookup"><span data-stu-id="863d8-157">Request</span></span>

<span data-ttu-id="863d8-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="863d8-158">Here is the example request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="863d8-159">响应</span><span class="sxs-lookup"><span data-stu-id="863d8-159">Response</span></span>

<span data-ttu-id="863d8-160">下面是示例响应</span><span class="sxs-lookup"><span data-stu-id="863d8-160">Here is the example response</span></span>
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