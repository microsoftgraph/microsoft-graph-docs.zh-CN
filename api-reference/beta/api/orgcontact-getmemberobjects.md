---
title: orgContact： getMemberObjects
description: 若要调用此 API，必须有以下权限之一。 若要了解详细信息，包括如何选择权限的信息，请参阅权限。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c6564953357659644db9ba71e7b62ce6ea00c74f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979831"
---
# <a name="orgcontact-getmemberobjects"></a><span data-ttu-id="664c3-104">orgContact： getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="664c3-104">orgContact: getMemberObjects</span></span>

<span data-ttu-id="664c3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="664c3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="664c3-106">权限</span><span class="sxs-lookup"><span data-stu-id="664c3-106">Permissions</span></span>
<span data-ttu-id="664c3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="664c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="664c3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="664c3-109">Permission type</span></span>      | <span data-ttu-id="664c3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="664c3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="664c3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="664c3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="664c3-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="664c3-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="664c3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="664c3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="664c3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="664c3-114">Not supported.</span></span>    |
|<span data-ttu-id="664c3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="664c3-115">Application</span></span> | <span data-ttu-id="664c3-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="664c3-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="664c3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="664c3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="664c3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="664c3-118">Request headers</span></span>
| <span data-ttu-id="664c3-119">名称</span><span class="sxs-lookup"><span data-stu-id="664c3-119">Name</span></span>       | <span data-ttu-id="664c3-120">类型</span><span class="sxs-lookup"><span data-stu-id="664c3-120">Type</span></span> | <span data-ttu-id="664c3-121">说明</span><span class="sxs-lookup"><span data-stu-id="664c3-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="664c3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="664c3-122">Authorization</span></span>  | <span data-ttu-id="664c3-123">string</span><span class="sxs-lookup"><span data-stu-id="664c3-123">string</span></span>  | <span data-ttu-id="664c3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="664c3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="664c3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="664c3-126">Request body</span></span>
<span data-ttu-id="664c3-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="664c3-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="664c3-128">参数</span><span class="sxs-lookup"><span data-stu-id="664c3-128">Parameter</span></span>    | <span data-ttu-id="664c3-129">类型</span><span class="sxs-lookup"><span data-stu-id="664c3-129">Type</span></span>   |<span data-ttu-id="664c3-130">说明</span><span class="sxs-lookup"><span data-stu-id="664c3-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="664c3-131">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="664c3-131">securityEnabledOnly</span></span>|<span data-ttu-id="664c3-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="664c3-132">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="664c3-133">响应</span><span class="sxs-lookup"><span data-stu-id="664c3-133">Response</span></span>

<span data-ttu-id="664c3-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="664c3-134">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="664c3-135">示例</span><span class="sxs-lookup"><span data-stu-id="664c3-135">Example</span></span>
<span data-ttu-id="664c3-136">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="664c3-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="664c3-137">请求</span><span class="sxs-lookup"><span data-stu-id="664c3-137">Request</span></span>
<span data-ttu-id="664c3-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="664c3-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="664c3-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="664c3-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="664c3-140">C#</span><span class="sxs-lookup"><span data-stu-id="664c3-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="664c3-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="664c3-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="664c3-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="664c3-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="664c3-143">响应</span><span class="sxs-lookup"><span data-stu-id="664c3-143">Response</span></span>
<span data-ttu-id="664c3-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="664c3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


