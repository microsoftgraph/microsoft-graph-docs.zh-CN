---
title: 获取成员对象
description: " 返回用户、组、服务主体或目录对象是其中成员的所有组、管理单元和目录角色。 此函数是可传递的。 "
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a5f7ef92699cab5a7f39046e6ac5fe2fdab8585d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046844"
---
# <a name="get-member-objects"></a><span data-ttu-id="ee7ad-104">获取成员对象</span><span class="sxs-lookup"><span data-stu-id="ee7ad-104">Get member objects</span></span>

<span data-ttu-id="ee7ad-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee7ad-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

 <span data-ttu-id="ee7ad-106">返回用户、组、服务主体或目录对象是其中成员的所有组、管理单元和目录角色。</span><span class="sxs-lookup"><span data-stu-id="ee7ad-106">Returns all the groups, administrative units and directory roles that a user, group, service principals or directory object is a member of.</span></span> <span data-ttu-id="ee7ad-107">此函数是可传递的。</span><span class="sxs-lookup"><span data-stu-id="ee7ad-107">This function is transitive.</span></span> 
 > <span data-ttu-id="ee7ad-108">注意：只有用户可以是目录角色的成员。</span><span class="sxs-lookup"><span data-stu-id="ee7ad-108">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee7ad-109">权限</span><span class="sxs-lookup"><span data-stu-id="ee7ad-109">Permissions</span></span>
<span data-ttu-id="ee7ad-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ee7ad-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ee7ad-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee7ad-112">Permission type</span></span>      | <span data-ttu-id="ee7ad-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ee7ad-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee7ad-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee7ad-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ee7ad-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee7ad-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="ee7ad-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee7ad-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee7ad-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee7ad-117">Not supported.</span></span>    |
|<span data-ttu-id="ee7ad-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="ee7ad-118">Application</span></span> | <span data-ttu-id="ee7ad-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee7ad-119">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee7ad-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee7ad-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberObjects
POST /servicePrincipals/{id}/getMemberObjects
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="ee7ad-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee7ad-121">Request headers</span></span>
| <span data-ttu-id="ee7ad-122">名称</span><span class="sxs-lookup"><span data-stu-id="ee7ad-122">Name</span></span>       | <span data-ttu-id="ee7ad-123">类型</span><span class="sxs-lookup"><span data-stu-id="ee7ad-123">Type</span></span> | <span data-ttu-id="ee7ad-124">说明</span><span class="sxs-lookup"><span data-stu-id="ee7ad-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ee7ad-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee7ad-125">Authorization</span></span>  | <span data-ttu-id="ee7ad-126">string</span><span class="sxs-lookup"><span data-stu-id="ee7ad-126">string</span></span>  | <span data-ttu-id="ee7ad-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ee7ad-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ee7ad-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ee7ad-129">Content-Type</span></span>  | <span data-ttu-id="ee7ad-130">application/json</span><span class="sxs-lookup"><span data-stu-id="ee7ad-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ee7ad-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="ee7ad-131">Request body</span></span>
<span data-ttu-id="ee7ad-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ee7ad-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ee7ad-133">参数</span><span class="sxs-lookup"><span data-stu-id="ee7ad-133">Parameter</span></span>    | <span data-ttu-id="ee7ad-134">类型</span><span class="sxs-lookup"><span data-stu-id="ee7ad-134">Type</span></span>   |<span data-ttu-id="ee7ad-135">说明</span><span class="sxs-lookup"><span data-stu-id="ee7ad-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee7ad-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="ee7ad-136">securityEnabledOnly</span></span>|<span data-ttu-id="ee7ad-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee7ad-137">Boolean</span></span>| <span data-ttu-id="ee7ad-p105">**true** 指定仅应返回包含实体的安全组；**false** 指定应返回包含实体的所有组和目录角色。**注意**：如果参数为 **true**，只能对一位用户调用此函数。</span><span class="sxs-lookup"><span data-stu-id="ee7ad-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="ee7ad-140">响应</span><span class="sxs-lookup"><span data-stu-id="ee7ad-140">Response</span></span>

<span data-ttu-id="ee7ad-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="ee7ad-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee7ad-142">示例</span><span class="sxs-lookup"><span data-stu-id="ee7ad-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ee7ad-143">请求</span><span class="sxs-lookup"><span data-stu-id="ee7ad-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ee7ad-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee7ad-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="ee7ad-145">C#</span><span class="sxs-lookup"><span data-stu-id="ee7ad-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee7ad-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee7ad-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee7ad-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee7ad-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee7ad-148">Java</span><span class="sxs-lookup"><span data-stu-id="ee7ad-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ee7ad-149">响应</span><span class="sxs-lookup"><span data-stu-id="ee7ad-149">Response</span></span>
<span data-ttu-id="ee7ad-150">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ee7ad-150">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "c9ee2d50-9e8a-4352-b97c-4c2c99557c22",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


