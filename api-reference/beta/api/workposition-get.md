---
title: 获取 workPosition
description: 检索 workPosition 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9a600be212907e12d03329aa3027c86d41b726ec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092954"
---
# <a name="get-workposition"></a><span data-ttu-id="0645d-103">获取 workPosition</span><span class="sxs-lookup"><span data-stu-id="0645d-103">Get workPosition</span></span>

<span data-ttu-id="0645d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0645d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0645d-105">在用户的[配置文件](../resources/profile.md)中检索[workPosition](../resources/workposition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0645d-105">Retrieve the properties and relationships of a [workPosition](../resources/workposition.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0645d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="0645d-106">Permissions</span></span>

<span data-ttu-id="0645d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0645d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0645d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0645d-109">Permission type</span></span>                        | <span data-ttu-id="0645d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0645d-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="0645d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0645d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0645d-112">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="0645d-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="0645d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0645d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0645d-114">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="0645d-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="0645d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0645d-115">Application</span></span>                            | <span data-ttu-id="0645d-116">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="0645d-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="0645d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0645d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/positions/{id}
GET /users/{id | userPrincipalName}/profile/positions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0645d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0645d-118">Optional query parameters</span></span>

<span data-ttu-id="0645d-119">此方法支持 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="0645d-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="0645d-120">指定要包含在响应中的属性的列表，并以逗号分隔。</span><span class="sxs-lookup"><span data-stu-id="0645d-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="0645d-121">为获得最佳性能，请仅选择所需的属性子集。</span><span class="sxs-lookup"><span data-stu-id="0645d-121">For optimal performance, only select the subset of properties needed.</span></span>                                                                                                                                         |

## <a name="request-headers"></a><span data-ttu-id="0645d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="0645d-122">Request headers</span></span>

| <span data-ttu-id="0645d-123">名称</span><span class="sxs-lookup"><span data-stu-id="0645d-123">Name</span></span>           |<span data-ttu-id="0645d-124">说明</span><span class="sxs-lookup"><span data-stu-id="0645d-124">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="0645d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0645d-125">Authorization</span></span>  | <span data-ttu-id="0645d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0645d-p103">Bearer {token}. Required.</span></span>   |


## <a name="request-body"></a><span data-ttu-id="0645d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0645d-128">Request body</span></span>

<span data-ttu-id="0645d-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0645d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0645d-130">响应</span><span class="sxs-lookup"><span data-stu-id="0645d-130">Response</span></span>

<span data-ttu-id="0645d-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [workPosition](../resources/workposition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0645d-131">If successful, this method returns a `200 OK` response code and the requested [workPosition](../resources/workposition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0645d-132">示例</span><span class="sxs-lookup"><span data-stu-id="0645d-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0645d-133">请求</span><span class="sxs-lookup"><span data-stu-id="0645d-133">Request</span></span>

<span data-ttu-id="0645d-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0645d-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0645d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0645d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workposition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/positions/{id}
```
# <a name="c"></a>[<span data-ttu-id="0645d-136">C#</span><span class="sxs-lookup"><span data-stu-id="0645d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workposition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0645d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0645d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workposition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0645d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0645d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workposition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0645d-139">响应</span><span class="sxs-lookup"><span data-stu-id="0645d-139">Response</span></span>

<span data-ttu-id="0645d-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0645d-140">The following is an example of the response.</span></span>

> <span data-ttu-id="0645d-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0645d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workPosition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "organization",
  "inference": null,
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "source": null,
  "categories": null,
  "detail": {
    "company": {
      "displayName": "Adventureworks Ltd.",
      "pronunciation": null,
      "department": "Consulting",
      "officeLocation": "AW23/344",
      "address": {
        "type": "business",
        "postOfficeBox": null,
        "street": "123 Patriachy Ponds",
        "city": "Moscow",
        "state": null,
        "countryOrRegion": "Russian Federation",
        "postalCode": "RU-34621"
      },
      "webUrl": "https://www.adventureworks.com"
    },
    "description": null,
    "endMonthYear": null,
    "jobTitle": "Senior Product Branding Manager II",
    "role": "consulting",
    "startMonthYear": "datetime-value",
    "summary": null
  },
  "manager": null,
  "colleagues": null,
  "isCurrent": true
}
```


