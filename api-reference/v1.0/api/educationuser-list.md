---
title: 列出 educationUser
description: 获取 educationUser 对象及其属性的列表。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2fa8f0105257991ca5b7ea255d3ea3b534bb079b
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232164"
---
# <a name="list-educationusers"></a><span data-ttu-id="403cf-103">列出 educationUsers</span><span class="sxs-lookup"><span data-stu-id="403cf-103">List educationUsers</span></span>

<span data-ttu-id="403cf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="403cf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="403cf-105">获取 [educationUser 对象](../resources/educationuser.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="403cf-105">Get a list of the [educationUser](../resources/educationuser.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="403cf-106">权限</span><span class="sxs-lookup"><span data-stu-id="403cf-106">Permissions</span></span>

<span data-ttu-id="403cf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="403cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="403cf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="403cf-109">Permission type</span></span>                        | <span data-ttu-id="403cf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="403cf-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="403cf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="403cf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="403cf-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="403cf-112">Not supported.</span></span>                              |
| <span data-ttu-id="403cf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="403cf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="403cf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="403cf-114">Not supported.</span></span>                              |
| <span data-ttu-id="403cf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="403cf-115">Application</span></span>                            | <span data-ttu-id="403cf-116">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="403cf-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="403cf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="403cf-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="403cf-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="403cf-118">Optional query parameters</span></span>

<span data-ttu-id="403cf-119">此方法支持[OData query parameters](/graph/query-parameters)以帮助自定义响应，包括 `$search`、`$count`、 和 `$filter`</span><span class="sxs-lookup"><span data-stu-id="403cf-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span>

<span data-ttu-id="403cf-120">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="403cf-120">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="403cf-121">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="403cf-121">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="403cf-122">有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="403cf-122">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="403cf-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="403cf-123">Request headers</span></span>

| <span data-ttu-id="403cf-124">名称</span><span class="sxs-lookup"><span data-stu-id="403cf-124">Name</span></span>          | <span data-ttu-id="403cf-125">说明</span><span class="sxs-lookup"><span data-stu-id="403cf-125">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="403cf-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="403cf-126">Authorization</span></span> | <span data-ttu-id="403cf-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="403cf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="403cf-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="403cf-129">Request body</span></span>

<span data-ttu-id="403cf-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="403cf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="403cf-131">响应</span><span class="sxs-lookup"><span data-stu-id="403cf-131">Response</span></span>

<span data-ttu-id="403cf-132">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationUser](../resources/educationuser.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="403cf-132">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="403cf-133">示例</span><span class="sxs-lookup"><span data-stu-id="403cf-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="403cf-134">请求</span><span class="sxs-lookup"><span data-stu-id="403cf-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_educationuser"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/users
```

### <a name="response"></a><span data-ttu-id="403cf-135">响应</span><span class="sxs-lookup"><span data-stu-id="403cf-135">Response</span></span>

> <span data-ttu-id="403cf-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="403cf-136">**Note:** The response object shown here might be shortened for readability.</span></span>

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
