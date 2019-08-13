---
title: 'orgContact: checkMemberGroups'
description: 若要调用此 API, 必须有以下权限之一。 若要了解详细信息，包括如何选择权限的信息，请参阅权限。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3abbd7162759fa53103c1a49bb737870412dcfe1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342479"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="c0b7d-104">orgContact: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="c0b7d-104">orgContact: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="c0b7d-105">权限</span><span class="sxs-lookup"><span data-stu-id="c0b7d-105">Permissions</span></span>
<span data-ttu-id="c0b7d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0b7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0b7d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0b7d-108">Permission type</span></span>      | <span data-ttu-id="c0b7d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c0b7d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0b7d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0b7d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c0b7d-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c0b7d-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c0b7d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0b7d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0b7d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0b7d-113">Not supported.</span></span>    |
|<span data-ttu-id="c0b7d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0b7d-114">Application</span></span> | <span data-ttu-id="c0b7d-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0b7d-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0b7d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0b7d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="c0b7d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0b7d-117">Request headers</span></span>
| <span data-ttu-id="c0b7d-118">名称</span><span class="sxs-lookup"><span data-stu-id="c0b7d-118">Name</span></span>       | <span data-ttu-id="c0b7d-119">类型</span><span class="sxs-lookup"><span data-stu-id="c0b7d-119">Type</span></span> | <span data-ttu-id="c0b7d-120">说明</span><span class="sxs-lookup"><span data-stu-id="c0b7d-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c0b7d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0b7d-121">Authorization</span></span>  | <span data-ttu-id="c0b7d-122">string</span><span class="sxs-lookup"><span data-stu-id="c0b7d-122">string</span></span>  | <span data-ttu-id="c0b7d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c0b7d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0b7d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0b7d-125">Request body</span></span>
<span data-ttu-id="c0b7d-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c0b7d-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c0b7d-127">参数</span><span class="sxs-lookup"><span data-stu-id="c0b7d-127">Parameter</span></span>    | <span data-ttu-id="c0b7d-128">类型</span><span class="sxs-lookup"><span data-stu-id="c0b7d-128">Type</span></span>   |<span data-ttu-id="c0b7d-129">说明</span><span class="sxs-lookup"><span data-stu-id="c0b7d-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0b7d-130">groupIds</span><span class="sxs-lookup"><span data-stu-id="c0b7d-130">groupIds</span></span>|<span data-ttu-id="c0b7d-131">String collection</span><span class="sxs-lookup"><span data-stu-id="c0b7d-131">String collection</span></span> ||

## <a name="response"></a><span data-ttu-id="c0b7d-132">响应</span><span class="sxs-lookup"><span data-stu-id="c0b7d-132">Response</span></span>

<span data-ttu-id="c0b7d-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="c0b7d-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0b7d-134">示例</span><span class="sxs-lookup"><span data-stu-id="c0b7d-134">Example</span></span>
<span data-ttu-id="c0b7d-135">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c0b7d-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c0b7d-136">请求</span><span class="sxs-lookup"><span data-stu-id="c0b7d-136">Request</span></span>
<span data-ttu-id="c0b7d-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0b7d-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c0b7d-138">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c0b7d-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c0b7d-139">C#</span><span class="sxs-lookup"><span data-stu-id="c0b7d-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c0b7d-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0b7d-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c0b7d-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="c0b7d-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c0b7d-142">Java</span><span class="sxs-lookup"><span data-stu-id="c0b7d-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c0b7d-143">响应</span><span class="sxs-lookup"><span data-stu-id="c0b7d-143">Response</span></span>
<span data-ttu-id="c0b7d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c0b7d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "orgContact: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
