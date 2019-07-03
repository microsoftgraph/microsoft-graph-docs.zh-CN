---
title: 'servicePrincipal: getMemberObjects'
description: 获取此服务主体所属的组和目录角色的列表。  此检查是可传递的。
localization_priority: Normal
ms.openlocfilehash: 551a565e7693a4cc031754ad19a0e7cd5f8fb8ad
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35453724"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="8cb91-104">servicePrincipal: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="8cb91-104">servicePrincipal: getMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cb91-105">获取此服务主体所属的组和目录角色的列表。</span><span class="sxs-lookup"><span data-stu-id="8cb91-105">Get the list of groups and directory roles that this service principal is a member of.</span></span>  <span data-ttu-id="8cb91-106">此检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="8cb91-106">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cb91-107">权限</span><span class="sxs-lookup"><span data-stu-id="8cb91-107">Permissions</span></span>
<span data-ttu-id="8cb91-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8cb91-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cb91-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8cb91-110">Permission type</span></span>      | <span data-ttu-id="8cb91-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8cb91-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cb91-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8cb91-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8cb91-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8cb91-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8cb91-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8cb91-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cb91-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8cb91-115">Not supported.</span></span>    |
|<span data-ttu-id="8cb91-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8cb91-116">Application</span></span> | <span data-ttu-id="8cb91-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cb91-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cb91-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8cb91-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="8cb91-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8cb91-119">Request headers</span></span>
| <span data-ttu-id="8cb91-120">名称</span><span class="sxs-lookup"><span data-stu-id="8cb91-120">Name</span></span>       | <span data-ttu-id="8cb91-121">类型</span><span class="sxs-lookup"><span data-stu-id="8cb91-121">Type</span></span> | <span data-ttu-id="8cb91-122">说明</span><span class="sxs-lookup"><span data-stu-id="8cb91-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8cb91-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cb91-123">Authorization</span></span>  | <span data-ttu-id="8cb91-124">string</span><span class="sxs-lookup"><span data-stu-id="8cb91-124">string</span></span>  | <span data-ttu-id="8cb91-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8cb91-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cb91-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8cb91-127">Request body</span></span>
<span data-ttu-id="8cb91-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8cb91-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8cb91-129">参数</span><span class="sxs-lookup"><span data-stu-id="8cb91-129">Parameter</span></span>    | <span data-ttu-id="8cb91-130">类型</span><span class="sxs-lookup"><span data-stu-id="8cb91-130">Type</span></span>   |<span data-ttu-id="8cb91-131">说明</span><span class="sxs-lookup"><span data-stu-id="8cb91-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cb91-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="8cb91-132">securityEnabledOnly</span></span>|<span data-ttu-id="8cb91-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cb91-133">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="8cb91-134">响应</span><span class="sxs-lookup"><span data-stu-id="8cb91-134">Response</span></span>

<span data-ttu-id="8cb91-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="8cb91-135">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cb91-136">示例</span><span class="sxs-lookup"><span data-stu-id="8cb91-136">Example</span></span>
<span data-ttu-id="8cb91-137">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="8cb91-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8cb91-138">请求</span><span class="sxs-lookup"><span data-stu-id="8cb91-138">Request</span></span>
<span data-ttu-id="8cb91-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8cb91-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8cb91-140">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="8cb91-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8cb91-141">C#</span><span class="sxs-lookup"><span data-stu-id="8cb91-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8cb91-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="8cb91-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8cb91-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="8cb91-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8cb91-144">响应</span><span class="sxs-lookup"><span data-stu-id="8cb91-144">Response</span></span>
<span data-ttu-id="8cb91-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8cb91-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
