---
title: 'orgContact: checkMemberGroups'
description: 若要调用此 API, 必须有以下权限之一。 若要了解详细信息，包括如何选择权限的信息，请参阅权限。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 59b2a1771887fbe085e918b93c4b118dda7134ca
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440216"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="adecc-104">orgContact: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="adecc-104">orgContact: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="adecc-105">权限</span><span class="sxs-lookup"><span data-stu-id="adecc-105">Permissions</span></span>
<span data-ttu-id="adecc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="adecc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adecc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="adecc-108">Permission type</span></span>      | <span data-ttu-id="adecc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="adecc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="adecc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="adecc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="adecc-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="adecc-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="adecc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="adecc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adecc-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="adecc-113">Not supported.</span></span>    |
|<span data-ttu-id="adecc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="adecc-114">Application</span></span> | <span data-ttu-id="adecc-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adecc-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="adecc-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="adecc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="adecc-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="adecc-117">Request headers</span></span>
| <span data-ttu-id="adecc-118">名称</span><span class="sxs-lookup"><span data-stu-id="adecc-118">Name</span></span>       | <span data-ttu-id="adecc-119">类型</span><span class="sxs-lookup"><span data-stu-id="adecc-119">Type</span></span> | <span data-ttu-id="adecc-120">说明</span><span class="sxs-lookup"><span data-stu-id="adecc-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="adecc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="adecc-121">Authorization</span></span>  | <span data-ttu-id="adecc-122">string</span><span class="sxs-lookup"><span data-stu-id="adecc-122">string</span></span>  | <span data-ttu-id="adecc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="adecc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="adecc-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="adecc-125">Request body</span></span>
<span data-ttu-id="adecc-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="adecc-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="adecc-127">参数</span><span class="sxs-lookup"><span data-stu-id="adecc-127">Parameter</span></span>    | <span data-ttu-id="adecc-128">类型</span><span class="sxs-lookup"><span data-stu-id="adecc-128">Type</span></span>   |<span data-ttu-id="adecc-129">说明</span><span class="sxs-lookup"><span data-stu-id="adecc-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="adecc-130">groupIds</span><span class="sxs-lookup"><span data-stu-id="adecc-130">groupIds</span></span>|<span data-ttu-id="adecc-131">String collection</span><span class="sxs-lookup"><span data-stu-id="adecc-131">String collection</span></span> ||

## <a name="response"></a><span data-ttu-id="adecc-132">响应</span><span class="sxs-lookup"><span data-stu-id="adecc-132">Response</span></span>

<span data-ttu-id="adecc-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="adecc-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adecc-134">示例</span><span class="sxs-lookup"><span data-stu-id="adecc-134">Example</span></span>
<span data-ttu-id="adecc-135">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="adecc-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="adecc-136">请求</span><span class="sxs-lookup"><span data-stu-id="adecc-136">Request</span></span>
<span data-ttu-id="adecc-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="adecc-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="adecc-138">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="adecc-138">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="adecc-139">C#</span><span class="sxs-lookup"><span data-stu-id="adecc-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="adecc-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="adecc-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="adecc-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="adecc-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="adecc-142">响应</span><span class="sxs-lookup"><span data-stu-id="adecc-142">Response</span></span>
<span data-ttu-id="adecc-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="adecc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
