---
title: 列出成员
description: 检索分配给目录角色的用户列表。  只能将用户分配给目录角色。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 19a820605c1a912a0f9d6c052bc36de6114c473e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550607"
---
# <a name="list-members"></a><span data-ttu-id="a42d6-104">列出成员</span><span class="sxs-lookup"><span data-stu-id="a42d6-104">List members</span></span>

<span data-ttu-id="a42d6-105">检索分配给目录角色的用户列表。</span><span class="sxs-lookup"><span data-stu-id="a42d6-105">Retrieve a list of the users that are assigned to the directory role.</span></span>  <span data-ttu-id="a42d6-106">只能将用户分配给目录角色。</span><span class="sxs-lookup"><span data-stu-id="a42d6-106">Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="a42d6-107">权限</span><span class="sxs-lookup"><span data-stu-id="a42d6-107">Permissions</span></span>
<span data-ttu-id="a42d6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a42d6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a42d6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a42d6-110">Permission type</span></span>      | <span data-ttu-id="a42d6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a42d6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a42d6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a42d6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a42d6-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a42d6-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a42d6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a42d6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a42d6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a42d6-115">Not supported.</span></span>    |
|<span data-ttu-id="a42d6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a42d6-116">Application</span></span> | <span data-ttu-id="a42d6-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a42d6-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a42d6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a42d6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a42d6-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a42d6-119">Optional query parameters</span></span>
<span data-ttu-id="a42d6-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a42d6-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a42d6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a42d6-121">Request headers</span></span>
| <span data-ttu-id="a42d6-122">名称</span><span class="sxs-lookup"><span data-stu-id="a42d6-122">Name</span></span>       | <span data-ttu-id="a42d6-123">类型</span><span class="sxs-lookup"><span data-stu-id="a42d6-123">Type</span></span> | <span data-ttu-id="a42d6-124">说明</span><span class="sxs-lookup"><span data-stu-id="a42d6-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a42d6-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a42d6-125">Authorization</span></span>  | <span data-ttu-id="a42d6-126">string</span><span class="sxs-lookup"><span data-stu-id="a42d6-126">string</span></span>  | <span data-ttu-id="a42d6-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a42d6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a42d6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a42d6-129">Request body</span></span>
<span data-ttu-id="a42d6-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a42d6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a42d6-131">响应</span><span class="sxs-lookup"><span data-stu-id="a42d6-131">Response</span></span>

<span data-ttu-id="a42d6-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a42d6-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a42d6-133">示例</span><span class="sxs-lookup"><span data-stu-id="a42d6-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a42d6-134">请求</span><span class="sxs-lookup"><span data-stu-id="a42d6-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="a42d6-135">响应</span><span class="sxs-lookup"><span data-stu-id="a42d6-135">Response</span></span>
<span data-ttu-id="a42d6-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a42d6-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
