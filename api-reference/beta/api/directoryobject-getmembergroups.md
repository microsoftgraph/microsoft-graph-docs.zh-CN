---
title: 获取成员组
description: 返回指定的用户、组、服务主体或目录对象所属的所有组。 此函数是可传递的。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c599b058b7250dc836806b42bead85f6e67704f6
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656046"
---
# <a name="get-member-groups"></a><span data-ttu-id="01341-104">获取成员组</span><span class="sxs-lookup"><span data-stu-id="01341-104">Get member groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01341-105">返回指定的用户、组、服务主体或目录对象所属的所有组。</span><span class="sxs-lookup"><span data-stu-id="01341-105">Return all the groups that the specified user, group, service principal or directory object is a member of.</span></span> <span data-ttu-id="01341-106">此函数是可传递的。</span><span class="sxs-lookup"><span data-stu-id="01341-106">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="01341-107">权限</span><span class="sxs-lookup"><span data-stu-id="01341-107">Permissions</span></span>
<span data-ttu-id="01341-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01341-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="01341-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="01341-110">Permission type</span></span>      | <span data-ttu-id="01341-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01341-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01341-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01341-112">Delegated (work or school account)</span></span> | <span data-ttu-id="01341-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="01341-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="01341-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01341-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01341-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="01341-115">Not supported.</span></span>    |
|<span data-ttu-id="01341-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="01341-116">Application</span></span> | <span data-ttu-id="01341-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="01341-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01341-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01341-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /servicePrincipals/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="01341-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="01341-119">Request headers</span></span>
| <span data-ttu-id="01341-120">名称</span><span class="sxs-lookup"><span data-stu-id="01341-120">Name</span></span>       | <span data-ttu-id="01341-121">类型</span><span class="sxs-lookup"><span data-stu-id="01341-121">Type</span></span> | <span data-ttu-id="01341-122">说明</span><span class="sxs-lookup"><span data-stu-id="01341-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="01341-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="01341-123">Authorization</span></span>  | <span data-ttu-id="01341-124">string</span><span class="sxs-lookup"><span data-stu-id="01341-124">string</span></span>  | <span data-ttu-id="01341-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01341-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="01341-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="01341-127">Content-Type</span></span>  | <span data-ttu-id="01341-128">application/json</span><span class="sxs-lookup"><span data-stu-id="01341-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="01341-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="01341-129">Request body</span></span>
<span data-ttu-id="01341-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="01341-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="01341-131">参数</span><span class="sxs-lookup"><span data-stu-id="01341-131">Parameter</span></span>    | <span data-ttu-id="01341-132">类型</span><span class="sxs-lookup"><span data-stu-id="01341-132">Type</span></span>   |<span data-ttu-id="01341-133">说明</span><span class="sxs-lookup"><span data-stu-id="01341-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01341-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="01341-134">securityEnabledOnly</span></span>|<span data-ttu-id="01341-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="01341-135">Boolean</span></span>| <span data-ttu-id="01341-p105">**true** 指定仅应返回包含实体的安全组；**false** 指定应返回包含实体的所有组和目录角色。**注意**：如果参数为 **true**，只能对一位用户调用此函数。</span><span class="sxs-lookup"><span data-stu-id="01341-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="01341-138">响应</span><span class="sxs-lookup"><span data-stu-id="01341-138">Response</span></span>

<span data-ttu-id="01341-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="01341-139">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01341-140">示例</span><span class="sxs-lookup"><span data-stu-id="01341-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="01341-141">请求</span><span class="sxs-lookup"><span data-stu-id="01341-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="01341-142">响应</span><span class="sxs-lookup"><span data-stu-id="01341-142">Response</span></span>
<span data-ttu-id="01341-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="01341-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="01341-145">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="01341-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="01341-146">C#</span><span class="sxs-lookup"><span data-stu-id="01341-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/directoryobject_getmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="01341-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="01341-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/directoryobject_getmembergroups-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryobject-getmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryobject-getmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
