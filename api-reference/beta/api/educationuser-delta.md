---
title: 'educationUser: delta'
description: 获取新创建或更新的用户, 而无需对整个用户集执行完全读取。
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c89c065d5e4bd8510d6821a3c7a13bd106ce9eb8
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764734"
---
# <a name="educationuser-delta"></a><span data-ttu-id="09ce9-103">educationUser: delta</span><span class="sxs-lookup"><span data-stu-id="09ce9-103">educationUser: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09ce9-104">获取新创建或更新的[educationUser](../resources/educationuser.md) , 而无需对整个集合执行完全读取。</span><span class="sxs-lookup"><span data-stu-id="09ce9-104">Get newly created or updated [educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="09ce9-105">有关详细信息, 请参阅[使用 delta 查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="09ce9-105">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="09ce9-106">权限</span><span class="sxs-lookup"><span data-stu-id="09ce9-106">Permissions</span></span>

<span data-ttu-id="09ce9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09ce9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="09ce9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="09ce9-109">Permission type</span></span>                        | <span data-ttu-id="09ce9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09ce9-110">Permissions (from least to most privileged)</span></span>     |
| :------------------------------------- | :---------------------------------------------- |
| <span data-ttu-id="09ce9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09ce9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="09ce9-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="09ce9-112">Not supported.</span></span>                                  |
| <span data-ttu-id="09ce9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09ce9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09ce9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="09ce9-114">Not supported.</span></span>                                  |
| <span data-ttu-id="09ce9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="09ce9-115">Application</span></span>                            | <span data-ttu-id="09ce9-116">Eduroster.read.all 或 Eduroster.read.all 的所有 WriteWrite</span><span class="sxs-lookup"><span data-stu-id="09ce9-116">EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="09ce9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09ce9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/me/delta
POST /education/users/{id}/delta
POST /education/schools/{id}/users/{id}/delta
```

## <a name="request-headers"></a><span data-ttu-id="09ce9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="09ce9-118">Request headers</span></span>

| <span data-ttu-id="09ce9-119">名称</span><span class="sxs-lookup"><span data-stu-id="09ce9-119">Name</span></span>          | <span data-ttu-id="09ce9-120">说明</span><span class="sxs-lookup"><span data-stu-id="09ce9-120">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="09ce9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="09ce9-121">Authorization</span></span> | <span data-ttu-id="09ce9-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="09ce9-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="09ce9-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="09ce9-123">Request body</span></span>

<span data-ttu-id="09ce9-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="09ce9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09ce9-125">响应</span><span class="sxs-lookup"><span data-stu-id="09ce9-125">Response</span></span>

<span data-ttu-id="09ce9-126">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationUser](../resources/educationuser.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="09ce9-126">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09ce9-127">示例</span><span class="sxs-lookup"><span data-stu-id="09ce9-127">Example</span></span>

<span data-ttu-id="09ce9-128">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="09ce9-128">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="09ce9-129">请求</span><span class="sxs-lookup"><span data-stu-id="09ce9-129">Request</span></span>

<span data-ttu-id="09ce9-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="09ce9-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/me/delta
```

##### <a name="response"></a><span data-ttu-id="09ce9-131">响应</span><span class="sxs-lookup"><span data-stu-id="09ce9-131">Response</span></span>

<span data-ttu-id="09ce9-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="09ce9-132">The following is an example of the response.</span></span>

><span data-ttu-id="09ce9-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="09ce9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "primaryRole": "primaryRole-value",
      "middleName": "middleName-value",
      "externalSource": "externalSource-value",
      "residenceAddress": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "mailingAddress": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "student": {
        "graduationYear": "graduationYear-value",
        "grade": "grade-value",
        "birthDate": "datetime-value",
        "gender": "gender-value",
        "studentNumber": "studentNumber-value",
        "externalId": "externalId-value"
      }
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
