---
title: 'orgContact: checkMemberGroups'
description: 若要调用此 API, 必须有以下权限之一。 若要了解详细信息，包括如何选择权限的信息，请参阅权限。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8d35e9e9679fd79e48175fa97a0b3fe17e49097f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596879"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="335bb-104">orgContact: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="335bb-104">orgContact: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="335bb-105">权限</span><span class="sxs-lookup"><span data-stu-id="335bb-105">Permissions</span></span>
<span data-ttu-id="335bb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="335bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="335bb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="335bb-108">Permission type</span></span>      | <span data-ttu-id="335bb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="335bb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="335bb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="335bb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="335bb-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="335bb-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="335bb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="335bb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="335bb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="335bb-113">Not supported.</span></span>    |
|<span data-ttu-id="335bb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="335bb-114">Application</span></span> | <span data-ttu-id="335bb-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="335bb-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="335bb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="335bb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="335bb-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="335bb-117">Request headers</span></span>
| <span data-ttu-id="335bb-118">名称</span><span class="sxs-lookup"><span data-stu-id="335bb-118">Name</span></span>       | <span data-ttu-id="335bb-119">类型</span><span class="sxs-lookup"><span data-stu-id="335bb-119">Type</span></span> | <span data-ttu-id="335bb-120">说明</span><span class="sxs-lookup"><span data-stu-id="335bb-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="335bb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="335bb-121">Authorization</span></span>  | <span data-ttu-id="335bb-122">string</span><span class="sxs-lookup"><span data-stu-id="335bb-122">string</span></span>  | <span data-ttu-id="335bb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="335bb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="335bb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="335bb-125">Request body</span></span>
<span data-ttu-id="335bb-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="335bb-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="335bb-127">参数</span><span class="sxs-lookup"><span data-stu-id="335bb-127">Parameter</span></span>    | <span data-ttu-id="335bb-128">类型</span><span class="sxs-lookup"><span data-stu-id="335bb-128">Type</span></span>   |<span data-ttu-id="335bb-129">说明</span><span class="sxs-lookup"><span data-stu-id="335bb-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="335bb-130">groupIds</span><span class="sxs-lookup"><span data-stu-id="335bb-130">groupIds</span></span>|<span data-ttu-id="335bb-131">String collection</span><span class="sxs-lookup"><span data-stu-id="335bb-131">String collection</span></span> ||

## <a name="response"></a><span data-ttu-id="335bb-132">响应</span><span class="sxs-lookup"><span data-stu-id="335bb-132">Response</span></span>

<span data-ttu-id="335bb-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="335bb-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="335bb-134">示例</span><span class="sxs-lookup"><span data-stu-id="335bb-134">Example</span></span>
<span data-ttu-id="335bb-135">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="335bb-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="335bb-136">请求</span><span class="sxs-lookup"><span data-stu-id="335bb-136">Request</span></span>
<span data-ttu-id="335bb-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="335bb-137">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="335bb-138">响应</span><span class="sxs-lookup"><span data-stu-id="335bb-138">Response</span></span>
<span data-ttu-id="335bb-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="335bb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="335bb-142">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="335bb-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="335bb-143">语言</span><span class="sxs-lookup"><span data-stu-id="335bb-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/orgcontact_checkmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="335bb-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="335bb-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/orgcontact_checkmembergroups-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/orgcontact-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/orgcontact-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
