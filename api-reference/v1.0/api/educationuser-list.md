---
title: 列出 educationUser
description: 获取 educationUser 对象及其属性的列表。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6cf915d28369314d960ee4b868bafd2852819c7f
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475373"
---
# <a name="list-educationusers"></a><span data-ttu-id="5aec3-103">列出 educationUsers</span><span class="sxs-lookup"><span data-stu-id="5aec3-103">List educationUsers</span></span>

<span data-ttu-id="5aec3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5aec3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5aec3-105">获取 [educationUser 对象](../resources/educationuser.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="5aec3-105">Get a list of the [educationUser](../resources/educationuser.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="5aec3-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="5aec3-106">Permissions</span></span>

<span data-ttu-id="5aec3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5aec3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5aec3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5aec3-109">Permission type</span></span>                        | <span data-ttu-id="5aec3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5aec3-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5aec3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5aec3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5aec3-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="5aec3-112">Not supported.</span></span>                              |
| <span data-ttu-id="5aec3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5aec3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5aec3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5aec3-114">Not supported.</span></span>                              |
| <span data-ttu-id="5aec3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5aec3-115">Application</span></span>                            | <span data-ttu-id="5aec3-116">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5aec3-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5aec3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5aec3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5aec3-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5aec3-118">Optional query parameters</span></span>

<span data-ttu-id="5aec3-119">此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="5aec3-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span>

<span data-ttu-id="5aec3-120">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="5aec3-120">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="5aec3-121">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="5aec3-121">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="5aec3-122">有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="5aec3-122">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5aec3-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="5aec3-123">Request headers</span></span>

| <span data-ttu-id="5aec3-124">名称</span><span class="sxs-lookup"><span data-stu-id="5aec3-124">Name</span></span>          | <span data-ttu-id="5aec3-125">说明</span><span class="sxs-lookup"><span data-stu-id="5aec3-125">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5aec3-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5aec3-126">Authorization</span></span> | <span data-ttu-id="5aec3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5aec3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5aec3-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5aec3-129">Request body</span></span>

<span data-ttu-id="5aec3-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5aec3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5aec3-131">响应</span><span class="sxs-lookup"><span data-stu-id="5aec3-131">Response</span></span>

<span data-ttu-id="5aec3-132">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="5aec3-132">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5aec3-133">示例</span><span class="sxs-lookup"><span data-stu-id="5aec3-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5aec3-134">请求</span><span class="sxs-lookup"><span data-stu-id="5aec3-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5aec3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5aec3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_educationuser"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/users
```
# <a name="c"></a>[<span data-ttu-id="5aec3-136">C#</span><span class="sxs-lookup"><span data-stu-id="5aec3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5aec3-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5aec3-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5aec3-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5aec3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5aec3-139">Java</span><span class="sxs-lookup"><span data-stu-id="5aec3-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5aec3-140">响应</span><span class="sxs-lookup"><span data-stu-id="5aec3-140">Response</span></span>

> <span data-ttu-id="5aec3-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5aec3-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.educationUser)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationUser",
      "id": "90eedea1-dea1-90ee-a1de-ee90a1deee90",
      "primaryRole": "String",
      "middleName": "String",
      "externalSource": "String",
      "externalSourceDetail": "String",
      "residenceAddress": {
        "@odata.type": "microsoft.graph.physicalAddress"
      },
      "mailingAddress": {
        "@odata.type": "microsoft.graph.physicalAddress"
      },
      "student": {
        "@odata.type": "microsoft.graph.educationStudent"
      },
      "teacher": {
        "@odata.type": "microsoft.graph.educationTeacher"
      },
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "accountEnabled": "Boolean",
      "assignedLicenses": [
        {
          "@odata.type": "microsoft.graph.assignedLicense"
        }
      ],
      "assignedPlans": [
        {
          "@odata.type": "microsoft.graph.assignedPlan"
        }
      ],
      "businessPhones": [
        "String"
      ],
      "department": "String",
      "displayName": "String",
      "givenName": "String",
      "mail": "String",
      "mailNickname": "String",
      "mobilePhone": "String",
      "passwordPolicies": "String",
      "passwordProfile": {
        "@odata.type": "microsoft.graph.passwordProfile"
      },
      "officeLocation": "String",
      "preferredLanguage": "String",
      "provisionedPlans": [
        {
          "@odata.type": "microsoft.graph.provisionedPlan"
        }
      ],
      "refreshTokensValidFromDateTime": "String (timestamp)",
      "showInAddressList": "Boolean",
      "surname": "String",
      "usageLocation": "String",
      "userPrincipalName": "String",
      "userType": "String",
      "onPremisesInfo": {
        "@odata.type": "microsoft.graph.educationOnPremisesInfo"
      }
    }
  ]
}
```
