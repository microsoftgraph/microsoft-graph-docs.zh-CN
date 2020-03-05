---
title: servicePrincipal： checkMemberGroups
description: 若要调用此 API，必须有以下权限之一。 若要了解详细信息，包括如何选择权限的信息，请参阅权限。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 63bf38ca44f75781bb501c0871a45e642799748c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453539"
---
# <a name="serviceprincipal-checkmembergroups"></a><span data-ttu-id="c809d-104">servicePrincipal： checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="c809d-104">servicePrincipal: checkMemberGroups</span></span>

<span data-ttu-id="c809d-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c809d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="c809d-106">权限</span><span class="sxs-lookup"><span data-stu-id="c809d-106">Permissions</span></span>
<span data-ttu-id="c809d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c809d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c809d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c809d-109">Permission type</span></span>      | <span data-ttu-id="c809d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c809d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c809d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c809d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c809d-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c809d-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c809d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c809d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c809d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c809d-114">Not supported.</span></span>    |
|<span data-ttu-id="c809d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c809d-115">Application</span></span> | <span data-ttu-id="c809d-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c809d-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c809d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c809d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="c809d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c809d-118">Request headers</span></span>
| <span data-ttu-id="c809d-119">名称</span><span class="sxs-lookup"><span data-stu-id="c809d-119">Name</span></span>       | <span data-ttu-id="c809d-120">类型</span><span class="sxs-lookup"><span data-stu-id="c809d-120">Type</span></span> | <span data-ttu-id="c809d-121">说明</span><span class="sxs-lookup"><span data-stu-id="c809d-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c809d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c809d-122">Authorization</span></span>  | <span data-ttu-id="c809d-123">string</span><span class="sxs-lookup"><span data-stu-id="c809d-123">string</span></span>  | <span data-ttu-id="c809d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c809d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c809d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c809d-126">Request body</span></span>
<span data-ttu-id="c809d-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c809d-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c809d-128">参数</span><span class="sxs-lookup"><span data-stu-id="c809d-128">Parameter</span></span>    | <span data-ttu-id="c809d-129">类型</span><span class="sxs-lookup"><span data-stu-id="c809d-129">Type</span></span>   |<span data-ttu-id="c809d-130">说明</span><span class="sxs-lookup"><span data-stu-id="c809d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c809d-131">groupIds</span><span class="sxs-lookup"><span data-stu-id="c809d-131">groupIds</span></span>|<span data-ttu-id="c809d-132">String collection</span><span class="sxs-lookup"><span data-stu-id="c809d-132">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="c809d-133">响应</span><span class="sxs-lookup"><span data-stu-id="c809d-133">Response</span></span>

<span data-ttu-id="c809d-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="c809d-134">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c809d-135">示例</span><span class="sxs-lookup"><span data-stu-id="c809d-135">Example</span></span>
<span data-ttu-id="c809d-136">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c809d-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c809d-137">请求</span><span class="sxs-lookup"><span data-stu-id="c809d-137">Request</span></span>
<span data-ttu-id="c809d-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c809d-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c809d-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="c809d-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="c809d-140">C#</span><span class="sxs-lookup"><span data-stu-id="c809d-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c809d-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c809d-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c809d-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c809d-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c809d-143">响应</span><span class="sxs-lookup"><span data-stu-id="c809d-143">Response</span></span>
<span data-ttu-id="c809d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c809d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
