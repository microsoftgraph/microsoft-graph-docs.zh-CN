---
title: educationUser： delta
description: 获取新创建或更新的用户，而无需执行整个用户集合的完全读取。
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7477bea6eeb01e74cb824a7d31b0cc5dba3161ef
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042924"
---
# <a name="educationuser-delta"></a><span data-ttu-id="6c37f-103">educationUser： delta</span><span class="sxs-lookup"><span data-stu-id="6c37f-103">educationUser: delta</span></span>

<span data-ttu-id="6c37f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c37f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c37f-105">获取新创建或更新的 [educationUser，](../resources/educationuser.md) 而无需执行整个集合的完整读取。</span><span class="sxs-lookup"><span data-stu-id="6c37f-105">Get newly created or updated [educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="6c37f-106">有关详细信息 [，请参阅使用 delta](/graph/delta-query-overview) 查询。</span><span class="sxs-lookup"><span data-stu-id="6c37f-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c37f-107">权限</span><span class="sxs-lookup"><span data-stu-id="6c37f-107">Permissions</span></span>

<span data-ttu-id="6c37f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6c37f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c37f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c37f-110">Permission type</span></span>                        | <span data-ttu-id="6c37f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6c37f-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="6c37f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c37f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c37f-113">EduRoster.ReadBasic、EduRoster.Read 或 EduRoster.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c37f-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="6c37f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c37f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c37f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c37f-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="6c37f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c37f-116">Application</span></span>                            | <span data-ttu-id="6c37f-117">EduRoster.ReadBasic.All、EduRoster.Read.All 或 EduRoster.WriteWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c37f-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c37f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c37f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/users/delta
```

## <a name="request-headers"></a><span data-ttu-id="6c37f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c37f-119">Request headers</span></span>

| <span data-ttu-id="6c37f-120">名称</span><span class="sxs-lookup"><span data-stu-id="6c37f-120">Name</span></span>          | <span data-ttu-id="6c37f-121">说明</span><span class="sxs-lookup"><span data-stu-id="6c37f-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="6c37f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c37f-122">Authorization</span></span> | <span data-ttu-id="6c37f-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6c37f-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c37f-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c37f-124">Request body</span></span>

<span data-ttu-id="6c37f-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6c37f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c37f-126">响应</span><span class="sxs-lookup"><span data-stu-id="6c37f-126">Response</span></span>

<span data-ttu-id="6c37f-127">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationUser](../resources/educationuser.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="6c37f-127">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) collection object in the response body.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="6c37f-128">educationUser 增量不包括已删除的用户。</span><span class="sxs-lookup"><span data-stu-id="6c37f-128">educationUser deltas do not include deleted users.</span></span>

## <a name="example"></a><span data-ttu-id="6c37f-129">示例</span><span class="sxs-lookup"><span data-stu-id="6c37f-129">Example</span></span>

<span data-ttu-id="6c37f-130">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="6c37f-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="6c37f-131">请求</span><span class="sxs-lookup"><span data-stu-id="6c37f-131">Request</span></span>

<span data-ttu-id="6c37f-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6c37f-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6c37f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c37f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/users/delta
```
# <a name="c"></a>[<span data-ttu-id="6c37f-134">C#</span><span class="sxs-lookup"><span data-stu-id="6c37f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationuser-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c37f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c37f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationuser-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c37f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c37f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationuser-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6c37f-137">Java</span><span class="sxs-lookup"><span data-stu-id="6c37f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationuser-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6c37f-138">响应</span><span class="sxs-lookup"><span data-stu-id="6c37f-138">Response</span></span>

<span data-ttu-id="6c37f-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6c37f-139">The following is an example of the response.</span></span>

> <span data-ttu-id="6c37f-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6c37f-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1039

{
  "value": [
    {
      "accountEnabled": true,
      "assignedLicenses": [{ "@odata.type": "microsoft.graph.assignedLicense" }],
      "assignedPlans": [{ "@odata.type": "microsoft.graph.assignedPlan" }],
      "businessPhones": ["String"],
      "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
      "department": "String",
      "displayName": "String",
      "externalSource": "string",
      "givenName": "String",
      "id": "String (identifier)",
      "mail": "String",
      "mailNickname": "String",
      "mailingAddress": { "@odata.type": "microsoft.graph.physicalAddress" },
      "middleName": "String",
      "mobilePhone": "String",
      "officeLocation": "String",
      "onPremisesInfo": {
        "@odata.type": "microsoft.graph.educationOnPremisesInfo"
      },
      "passwordPolicies": "String",
      "passwordProfile": { "@odata.type": "microsoft.graph.passwordProfile" },
      "preferredLanguage": "String",
      "primaryRole": "string",
      "provisionedPlans": [{ "@odata.type": "microsoft.graph.provisionedPlan" }],
      "residenceAddress": { "@odata.type": "microsoft.graph.physicalAddress" },
      "student": { "@odata.type": "microsoft.graph.educationStudent" },
      "surname": "String",
      "teacher": { "@odata.type": "microsoft.graph.educationTeacher" },
      "usageLocation": "String",
      "userPrincipalName": "String",
      "userType": "String"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationUser: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


