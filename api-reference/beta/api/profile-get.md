---
title: 获取配置文件
description: 检索 profile 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: ed4d1c0cfc507931345d0932d9c9a52f2f7d1971
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970218"
---
# <a name="get-profile"></a><span data-ttu-id="0ce2b-103">获取配置文件</span><span class="sxs-lookup"><span data-stu-id="0ce2b-103">Get profile</span></span>

<span data-ttu-id="0ce2b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ce2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ce2b-105">检索给定用户的 [配置文件](../resources/profile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0ce2b-105">Retrieve the properties and relationships of a [profile](../resources/profile.md) object for a given user.</span></span>

<span data-ttu-id="0ce2b-106">**配置文件** 资源公开了将用户描述为 [关系](../resources/profile.md#relationships)的各种丰富的属性，例如，周年纪念和教育活动。</span><span class="sxs-lookup"><span data-stu-id="0ce2b-106">The **profile** resource exposes various rich properties that are descriptive of the user as [relationships](../resources/profile.md#relationships), for example, anniversaries and education activities.</span></span> <span data-ttu-id="0ce2b-107">若要获取这些导航属性之一，请对该属性使用相应的 GET 方法。</span><span class="sxs-lookup"><span data-stu-id="0ce2b-107">To get one of these navigation properties, use the corresponding GET method on that property.</span></span> <span data-ttu-id="0ce2b-108">请参阅由 **profile** 公开的 [方法](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="0ce2b-108">See the [methods](../resources/profile.md) exposed by **profile**.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ce2b-109">权限</span><span class="sxs-lookup"><span data-stu-id="0ce2b-109">Permissions</span></span>

<span data-ttu-id="0ce2b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ce2b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0ce2b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ce2b-112">Permission type</span></span>                        | <span data-ttu-id="0ce2b-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ce2b-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0ce2b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ce2b-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="0ce2b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ce2b-115">Not supported.</span></span>                              |
| <span data-ttu-id="0ce2b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ce2b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ce2b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ce2b-117">Not supported.</span></span>                              |
| <span data-ttu-id="0ce2b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ce2b-118">Application</span></span>                            | <span data-ttu-id="0ce2b-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ce2b-119">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="0ce2b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ce2b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile
GET /users/{id | userPrincipalName}/profile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0ce2b-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0ce2b-121">Optional query parameters</span></span>

<span data-ttu-id="0ce2b-122">此方法支持 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="0ce2b-122">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="0ce2b-123">指定要包含在响应中的属性的列表，并以逗号分隔。</span><span class="sxs-lookup"><span data-stu-id="0ce2b-123">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="0ce2b-124">为获得最佳性能，请仅选择所需的属性子集。</span><span class="sxs-lookup"><span data-stu-id="0ce2b-124">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ce2b-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ce2b-125">Request headers</span></span>

| <span data-ttu-id="0ce2b-126">名称</span><span class="sxs-lookup"><span data-stu-id="0ce2b-126">Name</span></span>           |<span data-ttu-id="0ce2b-127">说明</span><span class="sxs-lookup"><span data-stu-id="0ce2b-127">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="0ce2b-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ce2b-128">Authorization</span></span>  | <span data-ttu-id="0ce2b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0ce2b-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="0ce2b-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0ce2b-131">Content-Type</span></span>   | <span data-ttu-id="0ce2b-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0ce2b-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ce2b-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ce2b-134">Request body</span></span>

<span data-ttu-id="0ce2b-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0ce2b-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ce2b-136">响应</span><span class="sxs-lookup"><span data-stu-id="0ce2b-136">Response</span></span>

<span data-ttu-id="0ce2b-137">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [配置文件](../resources/profile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0ce2b-137">If successful, this method returns a `200 OK` response code and the requested [profile](../resources/profile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0ce2b-138">示例</span><span class="sxs-lookup"><span data-stu-id="0ce2b-138">Examples</span></span>

### <a name="example-1-get-a-users-profile"></a><span data-ttu-id="0ce2b-139">示例1：获取用户的配置文件</span><span class="sxs-lookup"><span data-stu-id="0ce2b-139">Example 1: GET a user's profile</span></span>

<span data-ttu-id="0ce2b-140">以下是获取配置文件请求的示例。</span><span class="sxs-lookup"><span data-stu-id="0ce2b-140">The following is an example of the GET profile request.</span></span>

#### <a name="request"></a><span data-ttu-id="0ce2b-141">请求</span><span class="sxs-lookup"><span data-stu-id="0ce2b-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0ce2b-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ce2b-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profile"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile
```
# <a name="c"></a>[<span data-ttu-id="0ce2b-143">C#</span><span class="sxs-lookup"><span data-stu-id="0ce2b-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ce2b-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ce2b-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ce2b-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ce2b-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0ce2b-146">Java</span><span class="sxs-lookup"><span data-stu-id="0ce2b-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0ce2b-147">响应</span><span class="sxs-lookup"><span data-stu-id="0ce2b-147">Response</span></span>

<span data-ttu-id="0ce2b-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0ce2b-148">The following is an example of the response.</span></span>

> <span data-ttu-id="0ce2b-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0ce2b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-expand-names-and-skills-collection-and-select-properties-within-the-entities"></a><span data-ttu-id="0ce2b-151">示例2：展开名称和技能集合并在实体中选择属性</span><span class="sxs-lookup"><span data-stu-id="0ce2b-151">Example 2: Expand names and skills collection and select properties within the entities</span></span>

<span data-ttu-id="0ce2b-152">下面是使用 $expand 和 $select 查询参数从用户的配置文件中检索部分信息的示例。</span><span class="sxs-lookup"><span data-stu-id="0ce2b-152">The following is an example of using the $expand and $select query parameters to retrieve partial information from a user's profile.</span></span>

#### <a name="request"></a><span data-ttu-id="0ce2b-153">请求</span><span class="sxs-lookup"><span data-stu-id="0ce2b-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0ce2b-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ce2b-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profile"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile?$expand=names($select=first,last),skills($select=displayName)
```
# <a name="c"></a>[<span data-ttu-id="0ce2b-155">C#</span><span class="sxs-lookup"><span data-stu-id="0ce2b-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ce2b-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ce2b-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ce2b-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ce2b-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0ce2b-158">Java</span><span class="sxs-lookup"><span data-stu-id="0ce2b-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0ce2b-159">响应</span><span class="sxs-lookup"><span data-stu-id="0ce2b-159">Response</span></span>

<span data-ttu-id="0ce2b-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0ce2b-160">The following is an example of the response.</span></span>

> <span data-ttu-id="0ce2b-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0ce2b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


