---
title: educationUser： delta
description: 获取新创建或更新的用户，而无需对整个用户集执行完全读取。
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 37dc85ae1c907aaa1cf43428e7ad19188e7c053d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42423922"
---
# <a name="educationuser-delta"></a><span data-ttu-id="6f7c9-103">educationUser： delta</span><span class="sxs-lookup"><span data-stu-id="6f7c9-103">educationUser: delta</span></span>

<span data-ttu-id="6f7c9-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6f7c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f7c9-105">获取新创建或更新的[educationUser](../resources/educationuser.md) ，而无需对整个集合执行完全读取。</span><span class="sxs-lookup"><span data-stu-id="6f7c9-105">Get newly created or updated [educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="6f7c9-106">有关详细信息，请参阅[使用 delta 查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="6f7c9-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f7c9-107">权限</span><span class="sxs-lookup"><span data-stu-id="6f7c9-107">Permissions</span></span>

<span data-ttu-id="6f7c9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6f7c9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6f7c9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f7c9-110">Permission type</span></span>                        | <span data-ttu-id="6f7c9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6f7c9-111">Permissions (from least to most privileged)</span></span>     |
| :------------------------------------- | :---------------------------------------------- |
| <span data-ttu-id="6f7c9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f7c9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6f7c9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f7c9-113">Not supported.</span></span>                                  |
| <span data-ttu-id="6f7c9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f7c9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f7c9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f7c9-115">Not supported.</span></span>                                  |
| <span data-ttu-id="6f7c9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f7c9-116">Application</span></span>                            | <span data-ttu-id="6f7c9-117">Eduroster.read.all 或 Eduroster.read.all 的所有 WriteWrite</span><span class="sxs-lookup"><span data-stu-id="6f7c9-117">EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f7c9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f7c9-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/me/delta
POST /education/users/{id}/delta
POST /education/schools/{id}/users/{id}/delta
```

## <a name="request-headers"></a><span data-ttu-id="6f7c9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f7c9-119">Request headers</span></span>

| <span data-ttu-id="6f7c9-120">名称</span><span class="sxs-lookup"><span data-stu-id="6f7c9-120">Name</span></span>          | <span data-ttu-id="6f7c9-121">说明</span><span class="sxs-lookup"><span data-stu-id="6f7c9-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="6f7c9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f7c9-122">Authorization</span></span> | <span data-ttu-id="6f7c9-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6f7c9-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f7c9-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f7c9-124">Request body</span></span>

<span data-ttu-id="6f7c9-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6f7c9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f7c9-126">响应</span><span class="sxs-lookup"><span data-stu-id="6f7c9-126">Response</span></span>

<span data-ttu-id="6f7c9-127">如果成功，此方法在响应`200 OK`正文中返回响应代码和[educationUser](../resources/educationuser.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="6f7c9-127">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f7c9-128">示例</span><span class="sxs-lookup"><span data-stu-id="6f7c9-128">Example</span></span>

<span data-ttu-id="6f7c9-129">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="6f7c9-129">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="6f7c9-130">请求</span><span class="sxs-lookup"><span data-stu-id="6f7c9-130">Request</span></span>

<span data-ttu-id="6f7c9-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6f7c9-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/me/delta
```

##### <a name="response"></a><span data-ttu-id="6f7c9-132">响应</span><span class="sxs-lookup"><span data-stu-id="6f7c9-132">Response</span></span>

<span data-ttu-id="6f7c9-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6f7c9-133">The following is an example of the response.</span></span>

><span data-ttu-id="6f7c9-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6f7c9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
