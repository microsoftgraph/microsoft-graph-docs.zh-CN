---
title: 向 educationSchool 添加 educationUser
description: 向学校添加用户。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8da24e46d555c4d673ab2a8a6083a1b670a5b070
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259554"
---
# <a name="add-educationuser-to-an-educationschool"></a><span data-ttu-id="2ed6f-103">向 educationSchool 添加 educationUser</span><span class="sxs-lookup"><span data-stu-id="2ed6f-103">Add educationUser to an educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ed6f-104">向学校添加用户。</span><span class="sxs-lookup"><span data-stu-id="2ed6f-104">Add a user to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ed6f-105">权限</span><span class="sxs-lookup"><span data-stu-id="2ed6f-105">Permissions</span></span>

<span data-ttu-id="2ed6f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ed6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ed6f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ed6f-108">Permission type</span></span>                        | <span data-ttu-id="2ed6f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2ed6f-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="2ed6f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ed6f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ed6f-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ed6f-111">Not supported.</span></span>                              |
| <span data-ttu-id="2ed6f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ed6f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ed6f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ed6f-113">Not supported.</span></span>                              |
| <span data-ttu-id="2ed6f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ed6f-114">Application</span></span>                            | <span data-ttu-id="2ed6f-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ed6f-115">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="2ed6f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ed6f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/users/$ref
```

## <a name="request-headers"></a><span data-ttu-id="2ed6f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ed6f-117">Request headers</span></span>

| <span data-ttu-id="2ed6f-118">标头</span><span class="sxs-lookup"><span data-stu-id="2ed6f-118">Header</span></span>        | <span data-ttu-id="2ed6f-119">值</span><span class="sxs-lookup"><span data-stu-id="2ed6f-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="2ed6f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ed6f-120">Authorization</span></span> | <span data-ttu-id="2ed6f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2ed6f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2ed6f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2ed6f-123">Content-Type</span></span>  | <span data-ttu-id="2ed6f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2ed6f-124">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="2ed6f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ed6f-125">Request body</span></span>

<span data-ttu-id="2ed6f-126">在请求正文中，提供 [educationUser](../resources/educationuser.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ed6f-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2ed6f-127">响应</span><span class="sxs-lookup"><span data-stu-id="2ed6f-127">Response</span></span>

<span data-ttu-id="2ed6f-128">如果成功，此方法会在响应正文中返回 `204 No Content` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2ed6f-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ed6f-129">示例</span><span class="sxs-lookup"><span data-stu-id="2ed6f-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2ed6f-130">请求</span><span class="sxs-lookup"><span data-stu-id="2ed6f-130">Request</span></span>

<span data-ttu-id="2ed6f-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2ed6f-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationschool"
}-->

```http
POST https://graph.microsoft.com/beta/education/schools/{id}/users/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/14008"
}
```

##### <a name="response"></a><span data-ttu-id="2ed6f-132">响应</span><span class="sxs-lookup"><span data-stu-id="2ed6f-132">Response</span></span>

<span data-ttu-id="2ed6f-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2ed6f-133">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="2ed6f-134">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="2ed6f-134">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ed6f-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="2ed6f-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_educationuser_from_educationschool-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2ed6f-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="2ed6f-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_educationuser_from_educationschool-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationschool-post-users.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationschool-post-users.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
