---
title: educationSchool： delta
description: 获取新创建或更新的学校，而无需执行整个学校集合的完整读取。
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 9491a958776797252eada5116b48b25a936b4111
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043463"
---
# <a name="educationschool-delta"></a><span data-ttu-id="704cf-103">educationSchool： delta</span><span class="sxs-lookup"><span data-stu-id="704cf-103">educationSchool: delta</span></span>

<span data-ttu-id="704cf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="704cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="704cf-105">获取新创建或更新的学校，而无需执行整个学校集合的完整读取。</span><span class="sxs-lookup"><span data-stu-id="704cf-105">Get newly created or updated schools without having to perform a full read of the entire school collection.</span></span> <span data-ttu-id="704cf-106">有关详细信息 [，请参阅使用 delta](/graph/delta-query-overview) 查询。</span><span class="sxs-lookup"><span data-stu-id="704cf-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="704cf-107">权限</span><span class="sxs-lookup"><span data-stu-id="704cf-107">Permissions</span></span>

<span data-ttu-id="704cf-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="704cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="704cf-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="704cf-110">Permission type</span></span>                        | <span data-ttu-id="704cf-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="704cf-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="704cf-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="704cf-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="704cf-113">EduRoster.ReadBasic、EduRoster.Read 或 EduRoster.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="704cf-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="704cf-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="704cf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="704cf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="704cf-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="704cf-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="704cf-116">Application</span></span>                            | <span data-ttu-id="704cf-117">EduRoster.ReadBasic.All、EduRoster.Read.All 或 EduRoster.WriteWrite.All</span><span class="sxs-lookup"><span data-stu-id="704cf-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="704cf-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="704cf-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/schools/delta
```

## <a name="request-headers"></a><span data-ttu-id="704cf-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="704cf-119">Request headers</span></span>

| <span data-ttu-id="704cf-120">名称</span><span class="sxs-lookup"><span data-stu-id="704cf-120">Name</span></span>          | <span data-ttu-id="704cf-121">说明</span><span class="sxs-lookup"><span data-stu-id="704cf-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="704cf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="704cf-122">Authorization</span></span> | <span data-ttu-id="704cf-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="704cf-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="704cf-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="704cf-124">Request body</span></span>

<span data-ttu-id="704cf-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="704cf-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="704cf-126">响应</span><span class="sxs-lookup"><span data-stu-id="704cf-126">Response</span></span>

<span data-ttu-id="704cf-127">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [educationSchool](../resources/educationschool.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="704cf-127">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) collection object in the response body.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="704cf-128">educationSchool deltas 不包括已删除的学校。</span><span class="sxs-lookup"><span data-stu-id="704cf-128">educationSchool deltas do not include deleted schools.</span></span>

## <a name="example"></a><span data-ttu-id="704cf-129">示例</span><span class="sxs-lookup"><span data-stu-id="704cf-129">Example</span></span>

<span data-ttu-id="704cf-130">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="704cf-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="704cf-131">请求</span><span class="sxs-lookup"><span data-stu-id="704cf-131">Request</span></span>

<span data-ttu-id="704cf-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="704cf-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="704cf-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="704cf-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationschool_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools/delta
```
# <a name="c"></a>[<span data-ttu-id="704cf-134">C#</span><span class="sxs-lookup"><span data-stu-id="704cf-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationschool-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="704cf-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="704cf-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationschool-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="704cf-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="704cf-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationschool-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="704cf-137">Java</span><span class="sxs-lookup"><span data-stu-id="704cf-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationschool-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="704cf-138">响应</span><span class="sxs-lookup"><span data-stu-id="704cf-138">Response</span></span>

<span data-ttu-id="704cf-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="704cf-139">The following is an example of the response.</span></span>

> <span data-ttu-id="704cf-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="704cf-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 313

{
  "value": [
    {
      "address": { "@odata.type": "microsoft.graph.physicalAddress" },
      "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
      "description": "String",
      "displayName": "String",
      "externalId": "String",
      "externalPrincipalId": "String",
      "externalSource": "string",
      "highestGrade": "String",
      "id": "String (identifier)",
      "lowestGrade": "String",
      "phone": "String",
      "principalEmail": "String",
      "principalName": "String",
      "schoolNumber": "String"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


