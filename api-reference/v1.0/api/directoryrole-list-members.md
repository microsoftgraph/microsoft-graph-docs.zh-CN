---
title: 列出成员
description: 检索分配给目录角色的用户列表。只能将用户分配给目录角色。
ms.openlocfilehash: 52ba5ccf1bc7bbd502c53a659978b12faf129f9c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008171"
---
# <a name="list-members"></a><span data-ttu-id="60679-104">列出成员</span><span class="sxs-lookup"><span data-stu-id="60679-104">List members</span></span>

<span data-ttu-id="60679-p102">检索分配给目录角色的用户列表。只能将用户分配给目录角色。</span><span class="sxs-lookup"><span data-stu-id="60679-p102">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="60679-107">权限</span><span class="sxs-lookup"><span data-stu-id="60679-107">Permissions</span></span>
<span data-ttu-id="60679-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="60679-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="60679-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="60679-110">Permission type</span></span>      | <span data-ttu-id="60679-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="60679-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60679-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60679-112">Delegated (work or school account)</span></span> | <span data-ttu-id="60679-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="60679-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="60679-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60679-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60679-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="60679-115">Not supported.</span></span>    |
|<span data-ttu-id="60679-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="60679-116">Application</span></span> | <span data-ttu-id="60679-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60679-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60679-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60679-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="60679-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="60679-119">Optional query parameters</span></span>
<span data-ttu-id="60679-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="60679-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="60679-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="60679-121">Request headers</span></span>
| <span data-ttu-id="60679-122">名称</span><span class="sxs-lookup"><span data-stu-id="60679-122">Name</span></span>       | <span data-ttu-id="60679-123">类型</span><span class="sxs-lookup"><span data-stu-id="60679-123">Type</span></span> | <span data-ttu-id="60679-124">说明</span><span class="sxs-lookup"><span data-stu-id="60679-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="60679-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="60679-125">Authorization</span></span>  | <span data-ttu-id="60679-126">string</span><span class="sxs-lookup"><span data-stu-id="60679-126">string</span></span>  | <span data-ttu-id="60679-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="60679-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60679-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="60679-129">Request body</span></span>
<span data-ttu-id="60679-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="60679-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60679-131">响应</span><span class="sxs-lookup"><span data-stu-id="60679-131">Response</span></span>

<span data-ttu-id="60679-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="60679-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="60679-133">示例</span><span class="sxs-lookup"><span data-stu-id="60679-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60679-134">请求</span><span class="sxs-lookup"><span data-stu-id="60679-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="60679-135">响应</span><span class="sxs-lookup"><span data-stu-id="60679-135">Response</span></span>
<span data-ttu-id="60679-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="60679-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "businessPhones":["000-000-0000"],
      "displayName":"First Last",
      "givenName":"First",
      "jobTitle":null,
      "mail":"first@example.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Last",
      "userPrincipalName":"first@example.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->