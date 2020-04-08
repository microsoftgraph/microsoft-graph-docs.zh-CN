---
title: 获取成员对象
description: " 返回用户、组、服务主体或目录对象所属的所有组、管理单元和目录角色。 此函数是可传递的。 "
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 254287569da163b66fb58e9a0be292c3c6d22a64
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43180935"
---
# <a name="get-member-objects"></a><span data-ttu-id="c1202-104">获取成员对象</span><span class="sxs-lookup"><span data-stu-id="c1202-104">Get member objects</span></span>

<span data-ttu-id="c1202-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1202-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

 <span data-ttu-id="c1202-106">返回用户、组、服务主体或目录对象所属的所有组、管理单元和目录角色。</span><span class="sxs-lookup"><span data-stu-id="c1202-106">Returns all the groups, administrative units and directory roles that a user, group, service principals or directory object is a member of.</span></span> <span data-ttu-id="c1202-107">此函数是可传递的。</span><span class="sxs-lookup"><span data-stu-id="c1202-107">This function is transitive.</span></span> 
 > <span data-ttu-id="c1202-108">注意：只有用户可以是目录角色的成员。</span><span class="sxs-lookup"><span data-stu-id="c1202-108">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1202-109">权限</span><span class="sxs-lookup"><span data-stu-id="c1202-109">Permissions</span></span>
<span data-ttu-id="c1202-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1202-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c1202-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1202-112">Permission type</span></span>      | <span data-ttu-id="c1202-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1202-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1202-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1202-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c1202-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1202-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="c1202-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1202-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1202-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1202-117">Not supported.</span></span>    |
|<span data-ttu-id="c1202-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1202-118">Application</span></span> | <span data-ttu-id="c1202-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1202-119">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1202-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1202-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberObjects
POST /servicePrincipals/{id}/getMemberObjects
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="c1202-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1202-121">Request headers</span></span>
| <span data-ttu-id="c1202-122">名称</span><span class="sxs-lookup"><span data-stu-id="c1202-122">Name</span></span>       | <span data-ttu-id="c1202-123">类型</span><span class="sxs-lookup"><span data-stu-id="c1202-123">Type</span></span> | <span data-ttu-id="c1202-124">说明</span><span class="sxs-lookup"><span data-stu-id="c1202-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c1202-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1202-125">Authorization</span></span>  | <span data-ttu-id="c1202-126">string</span><span class="sxs-lookup"><span data-stu-id="c1202-126">string</span></span>  | <span data-ttu-id="c1202-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1202-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c1202-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1202-129">Content-Type</span></span>  | <span data-ttu-id="c1202-130">application/json</span><span class="sxs-lookup"><span data-stu-id="c1202-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c1202-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1202-131">Request body</span></span>
<span data-ttu-id="c1202-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c1202-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c1202-133">参数</span><span class="sxs-lookup"><span data-stu-id="c1202-133">Parameter</span></span>    | <span data-ttu-id="c1202-134">类型</span><span class="sxs-lookup"><span data-stu-id="c1202-134">Type</span></span>   |<span data-ttu-id="c1202-135">说明</span><span class="sxs-lookup"><span data-stu-id="c1202-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1202-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="c1202-136">securityEnabledOnly</span></span>|<span data-ttu-id="c1202-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1202-137">Boolean</span></span>| <span data-ttu-id="c1202-p105">**true** 指定仅应返回包含实体的安全组；**false** 指定应返回包含实体的所有组和目录角色。**注意**：如果参数为 **true**，只能对一位用户调用此函数。</span><span class="sxs-lookup"><span data-stu-id="c1202-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="c1202-140">响应</span><span class="sxs-lookup"><span data-stu-id="c1202-140">Response</span></span>

<span data-ttu-id="c1202-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="c1202-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1202-142">示例</span><span class="sxs-lookup"><span data-stu-id="c1202-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c1202-143">请求</span><span class="sxs-lookup"><span data-stu-id="c1202-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c1202-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1202-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c1202-145">C#</span><span class="sxs-lookup"><span data-stu-id="c1202-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1202-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1202-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1202-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1202-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c1202-148">响应</span><span class="sxs-lookup"><span data-stu-id="c1202-148">Response</span></span>
<span data-ttu-id="c1202-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1202-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
