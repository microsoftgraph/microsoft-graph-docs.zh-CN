---
title: 获取配置文件
description: 检索 profile 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 6365c1dfdc2cb8ae1e737b1305b3ccb7f4d60fb7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034894"
---
# <a name="get-profile"></a><span data-ttu-id="94876-103">获取配置文件</span><span class="sxs-lookup"><span data-stu-id="94876-103">Get profile</span></span>

<span data-ttu-id="94876-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94876-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94876-105">检索给定用户的 [配置文件](../resources/profile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94876-105">Retrieve the properties and relationships of a [profile](../resources/profile.md) object for a given user.</span></span>

<span data-ttu-id="94876-106">**配置文件**资源公开了将用户描述为[关系](../resources/profile.md#relationships)的各种丰富的属性，例如，周年纪念和教育活动。</span><span class="sxs-lookup"><span data-stu-id="94876-106">The **profile** resource exposes various rich properties that are descriptive of the user as [relationships](../resources/profile.md#relationships), for example, anniversaries and education activities.</span></span> <span data-ttu-id="94876-107">若要获取这些导航属性之一，请对该属性使用相应的 GET 方法。</span><span class="sxs-lookup"><span data-stu-id="94876-107">To get one of these navigation properties, use the corresponding GET method on that property.</span></span> <span data-ttu-id="94876-108">请参阅由**profile**公开的[方法](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="94876-108">See the [methods](../resources/profile.md) exposed by **profile**.</span></span>

## <a name="permissions"></a><span data-ttu-id="94876-109">权限</span><span class="sxs-lookup"><span data-stu-id="94876-109">Permissions</span></span>

<span data-ttu-id="94876-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94876-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94876-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="94876-112">Permission type</span></span>                        | <span data-ttu-id="94876-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94876-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="94876-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94876-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="94876-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="94876-115">Not supported.</span></span>                              |
| <span data-ttu-id="94876-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94876-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94876-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="94876-117">Not supported.</span></span>                              |
| <span data-ttu-id="94876-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="94876-118">Application</span></span>                            | <span data-ttu-id="94876-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="94876-119">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="94876-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94876-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile
GET /users/{id | userPrincipalName}/profile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94876-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="94876-121">Optional query parameters</span></span>

<span data-ttu-id="94876-122">此方法支持 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="94876-122">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="94876-123">指定要包含在响应中的属性的列表，并以逗号分隔。</span><span class="sxs-lookup"><span data-stu-id="94876-123">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="94876-124">为获得最佳性能，请仅选择所需的属性子集。</span><span class="sxs-lookup"><span data-stu-id="94876-124">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94876-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="94876-125">Request headers</span></span>

| <span data-ttu-id="94876-126">名称</span><span class="sxs-lookup"><span data-stu-id="94876-126">Name</span></span>           |<span data-ttu-id="94876-127">说明</span><span class="sxs-lookup"><span data-stu-id="94876-127">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="94876-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="94876-128">Authorization</span></span>  | <span data-ttu-id="94876-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94876-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="94876-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="94876-131">Content-Type</span></span>   | <span data-ttu-id="94876-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="94876-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94876-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="94876-134">Request body</span></span>

<span data-ttu-id="94876-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="94876-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94876-136">响应</span><span class="sxs-lookup"><span data-stu-id="94876-136">Response</span></span>

<span data-ttu-id="94876-137">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [配置文件](../resources/profile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="94876-137">If successful, this method returns a `200 OK` response code and the requested [profile](../resources/profile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94876-138">示例</span><span class="sxs-lookup"><span data-stu-id="94876-138">Examples</span></span>

### <a name="example-1-get-a-users-profile"></a><span data-ttu-id="94876-139">示例1：获取用户的配置文件</span><span class="sxs-lookup"><span data-stu-id="94876-139">Example 1: GET a user's profile</span></span>

<span data-ttu-id="94876-140">以下是获取配置文件请求的示例。</span><span class="sxs-lookup"><span data-stu-id="94876-140">The following is an example of the GET profile request.</span></span>

#### <a name="request"></a><span data-ttu-id="94876-141">请求</span><span class="sxs-lookup"><span data-stu-id="94876-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="94876-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="94876-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profile"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile
```
# <a name="c"></a>[<span data-ttu-id="94876-143">C#</span><span class="sxs-lookup"><span data-stu-id="94876-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94876-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94876-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94876-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94876-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="94876-146">响应</span><span class="sxs-lookup"><span data-stu-id="94876-146">Response</span></span>

<span data-ttu-id="94876-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="94876-147">The following is an example of the response.</span></span>

> <span data-ttu-id="94876-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="94876-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "34545-32444234-2334452-234332-432234",
  "accounts": [],
  "addresses": [
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
      "displayName": "Home",
      "detail": {
        "type": "home",
        "postOfficeBox": null,
        "street": "221B Baker Street",
        "city": "London",
        "state": null,
        "countryOrRegion": "United Kingdom",
        "postalCode": "E14 3TD"
      },
      "geoCoordinates": null
    }
  ],
  "anniversaries": [
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
      "type": "birthday",
      "date": "Date"
    }
  ],
  "websites": [],
  "educationalActivities": [],
  "emails": [
    {
      "id": "e13f7a4d-303c-464f-a6af-80ea18eb74f3",
      "allowedAudiences": "organization",
      "inference": null,
      "createdDateTime": "2020-07-06T06:34:12.2294868Z",
      "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Innocenty Popov"
        }
      },
      "lastModifiedDateTime": "2020-07-08T06:34:12.2294868Z",
      "lastModifiedBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Innocenty Popov"
        }
      },
      "source": {
        "type": "User"
      },
      "address": "innocenty.popov@adventureworks.com",
      "displayName": "Innocenty Popov",
      "type": "work"
    }
  ],
  "notes": [],
  "interests": [],
  "languages": [],
  "names": [
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
      "displayName": "Innocenty Popov",
      "first": "Innocenty",
      "initials": "IP",
      "last": "Popov",
      "languageTag": "en-US",
      "maiden": null,
      "middle": null,
      "nickname": "Kesha",
      "suffix": null,
      "title": null,
      "pronunciation": {
        "displayName": "In-no ken-te ",
        "first": "In-no ken-te Pop-ov",
        "maiden": null,
        "middle": null,
        "last": "Pop-ov"
      }
    }
  ],
  "phones": [
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
      "displayName": "Car Phone",
      "type": "other",
      "number": "+7 499 342 22 13"
    }
  ],
  "positions": [],
  "projects": [],
  "skills": [],
  "webAccounts": []
}
```

### <a name="example-2-expand-names-and-skills-collection-and-select-properties-within-the-entities"></a><span data-ttu-id="94876-150">示例2：展开名称和技能集合并在实体中选择属性</span><span class="sxs-lookup"><span data-stu-id="94876-150">Example 2: Expand names and skills collection and select properties within the entities</span></span>

<span data-ttu-id="94876-151">下面是使用 $expand 和 $select 查询参数从用户的配置文件中检索部分信息的示例。</span><span class="sxs-lookup"><span data-stu-id="94876-151">The following is an example of using the $expand and $select query parameters to retrieve partial information from a user's profile.</span></span>

#### <a name="request"></a><span data-ttu-id="94876-152">请求</span><span class="sxs-lookup"><span data-stu-id="94876-152">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="94876-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="94876-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profile"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile?$expand=names($select=first,last),skills($select=displayName)
```
# <a name="c"></a>[<span data-ttu-id="94876-154">C#</span><span class="sxs-lookup"><span data-stu-id="94876-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94876-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94876-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94876-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94876-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="94876-157">响应</span><span class="sxs-lookup"><span data-stu-id="94876-157">Response</span></span>

<span data-ttu-id="94876-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="94876-158">The following is an example of the response.</span></span>

> <span data-ttu-id="94876-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="94876-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "34545-32444234-2334452-234332-432234",
  "names": [
      {
          "first": "Innocenty",
          "last": "Popov"
      }
  ],
  "skills": [
      {
          "displayName": "Machine Learning"
      },
      {
          "displayName": "Artificial Intelligence"
      }
  ]
}
```


