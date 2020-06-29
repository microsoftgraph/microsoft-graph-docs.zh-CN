---
title: educationUser： delta
description: 获取新创建或更新的用户，而无需对整个用户集执行完全读取。
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 408fb43dbad69cbb699db899522cf938e84ec904
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909547"
---
# <a name="educationuser-delta"></a><span data-ttu-id="a2f16-103">educationUser： delta</span><span class="sxs-lookup"><span data-stu-id="a2f16-103">educationUser: delta</span></span>

<span data-ttu-id="a2f16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2f16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2f16-105">获取新创建或更新的[educationUser](../resources/educationuser.md) ，而无需对整个集合执行完全读取。</span><span class="sxs-lookup"><span data-stu-id="a2f16-105">Get newly created or updated [educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="a2f16-106">有关详细信息，请参阅[使用 delta 查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="a2f16-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2f16-107">权限</span><span class="sxs-lookup"><span data-stu-id="a2f16-107">Permissions</span></span>

<span data-ttu-id="a2f16-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="a2f16-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a2f16-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2f16-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a2f16-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2f16-110">Permission type</span></span>                        | <span data-ttu-id="a2f16-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a2f16-111">Permissions (from least to most privileged)</span></span>     |
| :------------------------------------- | :---------------------------------------------- |
| <span data-ttu-id="a2f16-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2f16-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2f16-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2f16-113">Not supported.</span></span>                                  |
| <span data-ttu-id="a2f16-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2f16-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2f16-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2f16-115">Not supported.</span></span>                                  |
| <span data-ttu-id="a2f16-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2f16-116">Application</span></span>                            | <span data-ttu-id="a2f16-117">Eduroster.read.all 或 Eduroster.read.all 的所有 WriteWrite</span><span class="sxs-lookup"><span data-stu-id="a2f16-117">EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2f16-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2f16-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/me/delta
POST /education/users/{id}/delta
POST /education/schools/{id}/users/{id}/delta
```

## <a name="request-headers"></a><span data-ttu-id="a2f16-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2f16-119">Request headers</span></span>

| <span data-ttu-id="a2f16-120">名称</span><span class="sxs-lookup"><span data-stu-id="a2f16-120">Name</span></span>          | <span data-ttu-id="a2f16-121">说明</span><span class="sxs-lookup"><span data-stu-id="a2f16-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="a2f16-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2f16-122">Authorization</span></span> | <span data-ttu-id="a2f16-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a2f16-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2f16-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2f16-124">Request body</span></span>

<span data-ttu-id="a2f16-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a2f16-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2f16-126">响应</span><span class="sxs-lookup"><span data-stu-id="a2f16-126">Response</span></span>

<span data-ttu-id="a2f16-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[educationUser](../resources/educationuser.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="a2f16-127">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) collection object in the response body.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a2f16-128">educationUser 增量不包括已删除的用户。</span><span class="sxs-lookup"><span data-stu-id="a2f16-128">educationUser deltas do not include deleted users.</span></span>

## <a name="example"></a><span data-ttu-id="a2f16-129">示例</span><span class="sxs-lookup"><span data-stu-id="a2f16-129">Example</span></span>

<span data-ttu-id="a2f16-130">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="a2f16-130">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a2f16-131">请求</span><span class="sxs-lookup"><span data-stu-id="a2f16-131">Request</span></span>

<span data-ttu-id="a2f16-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a2f16-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/me/delta
```

##### <a name="response"></a><span data-ttu-id="a2f16-133">响应</span><span class="sxs-lookup"><span data-stu-id="a2f16-133">Response</span></span>

<span data-ttu-id="a2f16-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a2f16-134">The following is an example of the response.</span></span>

> <span data-ttu-id="a2f16-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="a2f16-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a2f16-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="a2f16-136">All the properties will be returned from an actual call.</span></span>

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
