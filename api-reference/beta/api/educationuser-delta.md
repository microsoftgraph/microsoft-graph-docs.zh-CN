---
title: educationUser： delta
description: 获取新创建或更新的用户，而无需对整个用户集执行完全读取。
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: df778d95256c96a83bd211c68d129a0b420ff49c
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081117"
---
# <a name="educationuser-delta"></a><span data-ttu-id="8b6c5-103">educationUser： delta</span><span class="sxs-lookup"><span data-stu-id="8b6c5-103">educationUser: delta</span></span>

<span data-ttu-id="8b6c5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b6c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b6c5-105">获取新创建或更新的[educationUser](../resources/educationuser.md) ，而无需对整个集合执行完全读取。</span><span class="sxs-lookup"><span data-stu-id="8b6c5-105">Get newly created or updated [educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="8b6c5-106">有关详细信息，请参阅[使用 delta 查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="8b6c5-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b6c5-107">权限</span><span class="sxs-lookup"><span data-stu-id="8b6c5-107">Permissions</span></span>

<span data-ttu-id="8b6c5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8b6c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b6c5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8b6c5-110">Permission type</span></span>                        | <span data-ttu-id="8b6c5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8b6c5-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="8b6c5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b6c5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b6c5-113">Eduroster.read.all、User.readbasic.all、Eduroster.read.all 或 Eduroster.read.all</span><span class="sxs-lookup"><span data-stu-id="8b6c5-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="8b6c5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b6c5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b6c5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8b6c5-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="8b6c5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8b6c5-116">Application</span></span>                            | <span data-ttu-id="8b6c5-117">Eduroster.read.all、Eduroster.read.all、All 或 Eduroster.read.all 的所有 User.readbasic.all</span><span class="sxs-lookup"><span data-stu-id="8b6c5-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b6c5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b6c5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/users/delta
```

## <a name="request-headers"></a><span data-ttu-id="8b6c5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8b6c5-119">Request headers</span></span>

| <span data-ttu-id="8b6c5-120">名称</span><span class="sxs-lookup"><span data-stu-id="8b6c5-120">Name</span></span>          | <span data-ttu-id="8b6c5-121">说明</span><span class="sxs-lookup"><span data-stu-id="8b6c5-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="8b6c5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b6c5-122">Authorization</span></span> | <span data-ttu-id="8b6c5-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8b6c5-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b6c5-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="8b6c5-124">Request body</span></span>

<span data-ttu-id="8b6c5-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8b6c5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b6c5-126">响应</span><span class="sxs-lookup"><span data-stu-id="8b6c5-126">Response</span></span>

<span data-ttu-id="8b6c5-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[educationUser](../resources/educationuser.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="8b6c5-127">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) collection object in the response body.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="8b6c5-128">educationUser 增量不包括已删除的用户。</span><span class="sxs-lookup"><span data-stu-id="8b6c5-128">educationUser deltas do not include deleted users.</span></span>

## <a name="example"></a><span data-ttu-id="8b6c5-129">示例</span><span class="sxs-lookup"><span data-stu-id="8b6c5-129">Example</span></span>

<span data-ttu-id="8b6c5-130">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="8b6c5-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8b6c5-131">请求</span><span class="sxs-lookup"><span data-stu-id="8b6c5-131">Request</span></span>

<span data-ttu-id="8b6c5-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8b6c5-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8b6c5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b6c5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/users/delta
```
# <a name="c"></a>[<span data-ttu-id="8b6c5-134">C#</span><span class="sxs-lookup"><span data-stu-id="8b6c5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationuser-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b6c5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b6c5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationuser-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b6c5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b6c5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationuser-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8b6c5-137">响应</span><span class="sxs-lookup"><span data-stu-id="8b6c5-137">Response</span></span>

<span data-ttu-id="8b6c5-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8b6c5-138">The following is an example of the response.</span></span>

> <span data-ttu-id="8b6c5-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8b6c5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
