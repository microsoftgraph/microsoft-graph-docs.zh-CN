---
title: servicePrincipal： getMemberObjects
description: 获取此服务主体所属的组和目录角色列表。  此检查是可传递的。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 689eb4514207d58cb69a2ea0a32cd89fea93d5b0
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219282"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="b9476-104">servicePrincipal： getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="b9476-104">servicePrincipal: getMemberObjects</span></span>

<span data-ttu-id="b9476-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9476-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9476-106">获取此服务主体所属的组和目录角色列表。</span><span class="sxs-lookup"><span data-stu-id="b9476-106">Get the list of groups and directory roles that this service principal is a member of.</span></span>  <span data-ttu-id="b9476-107">此检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="b9476-107">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9476-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="b9476-108">Permissions</span></span>
<span data-ttu-id="b9476-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9476-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9476-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9476-111">Permission type</span></span>      | <span data-ttu-id="b9476-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9476-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9476-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9476-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b9476-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b9476-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b9476-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9476-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9476-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9476-116">Not supported.</span></span>    |
|<span data-ttu-id="b9476-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9476-117">Application</span></span> | <span data-ttu-id="b9476-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9476-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9476-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9476-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="b9476-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9476-120">Request headers</span></span>
| <span data-ttu-id="b9476-121">名称</span><span class="sxs-lookup"><span data-stu-id="b9476-121">Name</span></span>       | <span data-ttu-id="b9476-122">类型</span><span class="sxs-lookup"><span data-stu-id="b9476-122">Type</span></span> | <span data-ttu-id="b9476-123">说明</span><span class="sxs-lookup"><span data-stu-id="b9476-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b9476-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9476-124">Authorization</span></span>  | <span data-ttu-id="b9476-125">string</span><span class="sxs-lookup"><span data-stu-id="b9476-125">string</span></span>  | <span data-ttu-id="b9476-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9476-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9476-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9476-128">Request body</span></span>
<span data-ttu-id="b9476-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b9476-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b9476-130">参数</span><span class="sxs-lookup"><span data-stu-id="b9476-130">Parameter</span></span>    | <span data-ttu-id="b9476-131">类型</span><span class="sxs-lookup"><span data-stu-id="b9476-131">Type</span></span>   |<span data-ttu-id="b9476-132">说明</span><span class="sxs-lookup"><span data-stu-id="b9476-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9476-133">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="b9476-133">securityEnabledOnly</span></span>|<span data-ttu-id="b9476-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9476-134">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="b9476-135">响应</span><span class="sxs-lookup"><span data-stu-id="b9476-135">Response</span></span>

<span data-ttu-id="b9476-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="b9476-136">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9476-137">示例</span><span class="sxs-lookup"><span data-stu-id="b9476-137">Example</span></span>
<span data-ttu-id="b9476-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="b9476-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b9476-139">请求</span><span class="sxs-lookup"><span data-stu-id="b9476-139">Request</span></span>
<span data-ttu-id="b9476-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9476-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b9476-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9476-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b9476-142">C#</span><span class="sxs-lookup"><span data-stu-id="b9476-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9476-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9476-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9476-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9476-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b9476-145">响应</span><span class="sxs-lookup"><span data-stu-id="b9476-145">Response</span></span>
<span data-ttu-id="b9476-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b9476-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
