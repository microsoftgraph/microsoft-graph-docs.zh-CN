---
title: 列出用户
description: 检索用户对象列表。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 00cf39a3e50c6c9911471f60a1cc7def1ee4563b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544195"
---
# <a name="list-users"></a><span data-ttu-id="ed26a-103">列出用户</span><span class="sxs-lookup"><span data-stu-id="ed26a-103">List users</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed26a-104">检索 user 对象列表。</span><span class="sxs-lookup"><span data-stu-id="ed26a-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed26a-105">权限</span><span class="sxs-lookup"><span data-stu-id="ed26a-105">Permissions</span></span>

<span data-ttu-id="ed26a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed26a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed26a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed26a-108">Permission type</span></span>      | <span data-ttu-id="ed26a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed26a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed26a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed26a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ed26a-111">User.ReadBasic.All、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ed26a-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ed26a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed26a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed26a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed26a-113">Not supported.</span></span>    |
|<span data-ttu-id="ed26a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed26a-114">Application</span></span> | <span data-ttu-id="ed26a-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed26a-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed26a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed26a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed26a-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ed26a-117">Optional query parameters</span></span>

<span data-ttu-id="ed26a-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ed26a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed26a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed26a-119">Request headers</span></span>
| <span data-ttu-id="ed26a-120">标头</span><span class="sxs-lookup"><span data-stu-id="ed26a-120">Header</span></span>        | <span data-ttu-id="ed26a-121">值</span><span class="sxs-lookup"><span data-stu-id="ed26a-121">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="ed26a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed26a-122">Authorization</span></span> | <span data-ttu-id="ed26a-123">Bearer {token}（必需）</span><span class="sxs-lookup"><span data-stu-id="ed26a-123">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="ed26a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ed26a-124">Content-Type</span></span>  | <span data-ttu-id="ed26a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ed26a-125">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="ed26a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed26a-126">Request body</span></span>

<span data-ttu-id="ed26a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ed26a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed26a-128">响应</span><span class="sxs-lookup"><span data-stu-id="ed26a-128">Response</span></span>

<span data-ttu-id="ed26a-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ed26a-129">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed26a-130">示例</span><span class="sxs-lookup"><span data-stu-id="ed26a-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ed26a-131">请求</span><span class="sxs-lookup"><span data-stu-id="ed26a-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/users
```

##### <a name="response"></a><span data-ttu-id="ed26a-132">响应</span><span class="sxs-lookup"><span data-stu-id="ed26a-132">Response</span></span>

<span data-ttu-id="ed26a-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ed26a-133">Here is an example of the response.</span></span> <span data-ttu-id="ed26a-134">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ed26a-134">Note: The response object shown here may be truncated for brevity.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
