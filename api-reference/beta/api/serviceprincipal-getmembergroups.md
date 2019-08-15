---
title: 'servicePrincipal: getMemberGroups'
description: 获取此服务主体所属组的列表。  检查是可传递的。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4a6f1fce9f5995762c120ad14597834b06d8b07a
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410309"
---
# <a name="serviceprincipal-getmembergroups"></a><span data-ttu-id="218f5-104">servicePrincipal: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="218f5-104">servicePrincipal: getMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="218f5-105">获取此服务主体所属组的列表。</span><span class="sxs-lookup"><span data-stu-id="218f5-105">Get the list of groups that this service principal is a member of.</span></span>  <span data-ttu-id="218f5-106">检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="218f5-106">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="218f5-107">权限</span><span class="sxs-lookup"><span data-stu-id="218f5-107">Permissions</span></span>
<span data-ttu-id="218f5-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="218f5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="218f5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="218f5-110">Permission type</span></span>      | <span data-ttu-id="218f5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="218f5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="218f5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="218f5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="218f5-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="218f5-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="218f5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="218f5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="218f5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="218f5-115">Not supported.</span></span>    |
|<span data-ttu-id="218f5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="218f5-116">Application</span></span> | <span data-ttu-id="218f5-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="218f5-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="218f5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="218f5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="218f5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="218f5-119">Request headers</span></span>
| <span data-ttu-id="218f5-120">名称</span><span class="sxs-lookup"><span data-stu-id="218f5-120">Name</span></span>       | <span data-ttu-id="218f5-121">类型</span><span class="sxs-lookup"><span data-stu-id="218f5-121">Type</span></span> | <span data-ttu-id="218f5-122">说明</span><span class="sxs-lookup"><span data-stu-id="218f5-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="218f5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="218f5-123">Authorization</span></span>  | <span data-ttu-id="218f5-124">string</span><span class="sxs-lookup"><span data-stu-id="218f5-124">string</span></span>  | <span data-ttu-id="218f5-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="218f5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="218f5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="218f5-127">Request body</span></span>
<span data-ttu-id="218f5-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="218f5-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="218f5-129">参数</span><span class="sxs-lookup"><span data-stu-id="218f5-129">Parameter</span></span>    | <span data-ttu-id="218f5-130">类型</span><span class="sxs-lookup"><span data-stu-id="218f5-130">Type</span></span>   |<span data-ttu-id="218f5-131">说明</span><span class="sxs-lookup"><span data-stu-id="218f5-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="218f5-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="218f5-132">securityEnabledOnly</span></span>|<span data-ttu-id="218f5-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="218f5-133">Boolean</span></span>|<span data-ttu-id="218f5-p105">设置为 **false**。只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="218f5-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="218f5-136">响应</span><span class="sxs-lookup"><span data-stu-id="218f5-136">Response</span></span>

<span data-ttu-id="218f5-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="218f5-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="218f5-138">示例</span><span class="sxs-lookup"><span data-stu-id="218f5-138">Example</span></span>
<span data-ttu-id="218f5-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="218f5-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="218f5-140">请求</span><span class="sxs-lookup"><span data-stu-id="218f5-140">Request</span></span>
<span data-ttu-id="218f5-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="218f5-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="218f5-142">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="218f5-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="218f5-143">C#</span><span class="sxs-lookup"><span data-stu-id="218f5-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="218f5-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="218f5-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="218f5-145">目标-C</span><span class="sxs-lookup"><span data-stu-id="218f5-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="218f5-146">响应</span><span class="sxs-lookup"><span data-stu-id="218f5-146">Response</span></span>
<span data-ttu-id="218f5-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="218f5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
