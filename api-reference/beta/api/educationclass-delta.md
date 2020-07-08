---
title: educationClass： delta
description: 获取新创建的或更新的类（包括成员身份更改），而无需对整个类集合执行完全读取。
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 34766ce4e6fe210369869f71213fb596432cbaab
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081224"
---
# <a name="educationclass-delta"></a><span data-ttu-id="3e953-103">educationClass： delta</span><span class="sxs-lookup"><span data-stu-id="3e953-103">educationClass: delta</span></span>

<span data-ttu-id="3e953-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e953-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e953-105">获取新创建的或更新的类（包括成员身份更改），而无需对整个类集合执行完全读取。</span><span class="sxs-lookup"><span data-stu-id="3e953-105">Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection.</span></span> <span data-ttu-id="3e953-106">有关详细信息，请参阅[使用 delta 查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="3e953-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e953-107">权限</span><span class="sxs-lookup"><span data-stu-id="3e953-107">Permissions</span></span>

<span data-ttu-id="3e953-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="3e953-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3e953-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e953-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e953-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e953-110">Permission type</span></span>                        | <span data-ttu-id="3e953-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e953-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="3e953-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e953-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e953-113">Eduroster.read.all、User.readbasic.all、Eduroster.read.all 或 Eduroster.read.all</span><span class="sxs-lookup"><span data-stu-id="3e953-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="3e953-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e953-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e953-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e953-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="3e953-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e953-116">Application</span></span>                            | <span data-ttu-id="3e953-117">Eduroster.read.all、Eduroster.read.all、All 或 Eduroster.read.all 的所有 User.readbasic.all</span><span class="sxs-lookup"><span data-stu-id="3e953-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e953-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e953-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/delta
```

## <a name="request-headers"></a><span data-ttu-id="3e953-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e953-119">Request headers</span></span>

| <span data-ttu-id="3e953-120">名称</span><span class="sxs-lookup"><span data-stu-id="3e953-120">Name</span></span>          | <span data-ttu-id="3e953-121">说明</span><span class="sxs-lookup"><span data-stu-id="3e953-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="3e953-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e953-122">Authorization</span></span> | <span data-ttu-id="3e953-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3e953-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e953-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e953-124">Request body</span></span>

<span data-ttu-id="3e953-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3e953-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e953-126">响应</span><span class="sxs-lookup"><span data-stu-id="3e953-126">Response</span></span>

<span data-ttu-id="3e953-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[educationClass](../resources/educationclass.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="3e953-127">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) collection object in the response body.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="3e953-128">educationClass 增量不包括已删除的类。</span><span class="sxs-lookup"><span data-stu-id="3e953-128">educationClass deltas do not include deleted classes.</span></span>

## <a name="example"></a><span data-ttu-id="3e953-129">示例</span><span class="sxs-lookup"><span data-stu-id="3e953-129">Example</span></span>

<span data-ttu-id="3e953-130">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="3e953-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="3e953-131">请求</span><span class="sxs-lookup"><span data-stu-id="3e953-131">Request</span></span>

<span data-ttu-id="3e953-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3e953-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3e953-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e953-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationclass_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/delta
```
# <a name="c"></a>[<span data-ttu-id="3e953-134">C#</span><span class="sxs-lookup"><span data-stu-id="3e953-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationclass-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3e953-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e953-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationclass-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3e953-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e953-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationclass-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3e953-137">响应</span><span class="sxs-lookup"><span data-stu-id="3e953-137">Response</span></span>

<span data-ttu-id="3e953-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3e953-138">The following is an example of the response.</span></span>

> <span data-ttu-id="3e953-139">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="3e953-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3e953-140">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="3e953-140">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 585

{
  "value": [
    {
      "classCode": "String",
      "course": { "@odata.type": "microsoft.graph.educationCourse" },
      "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
      "description": "String",
      "displayName": "String",
      "externalId": "String",
      "externalName": "String",
      "externalSource": "string",
      "grade": "string",
      "id": "String (identifier)",
      "mailNickname": "String",
      "term": { "@odata.type": "microsoft.graph.educationTerm" }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationClass: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
