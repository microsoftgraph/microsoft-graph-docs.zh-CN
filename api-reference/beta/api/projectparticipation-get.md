---
title: 获取 projectParticipation
description: 检索 projectParticipation 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b767a32220ed21f196334c38efcd69604fc25778
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055202"
---
# <a name="get-projectparticipation"></a><span data-ttu-id="313ee-103">获取 projectParticipation</span><span class="sxs-lookup"><span data-stu-id="313ee-103">Get projectParticipation</span></span>

<span data-ttu-id="313ee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="313ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="313ee-105">检索用户配置文件中的 [projectParticipation](../resources/projectparticipation.md) 对象的属性和 [关系](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="313ee-105">Retrieve the properties and relationships of a [projectParticipation](../resources/projectparticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="313ee-106">权限</span><span class="sxs-lookup"><span data-stu-id="313ee-106">Permissions</span></span>

<span data-ttu-id="313ee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="313ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="313ee-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="313ee-109">Permission type</span></span>                        | <span data-ttu-id="313ee-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="313ee-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="313ee-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="313ee-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="313ee-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="313ee-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="313ee-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="313ee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="313ee-114">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="313ee-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="313ee-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="313ee-115">Application</span></span>                            | <span data-ttu-id="313ee-116">User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="313ee-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="313ee-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="313ee-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/projects/{id}
GET /users/{id | userPrincipalName}/profile/projects/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="313ee-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="313ee-118">Optional query parameters</span></span>

<span data-ttu-id="313ee-119">此方法支持 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="313ee-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="313ee-120">指定要包括在响应中的属性列表，用逗号分隔它们。</span><span class="sxs-lookup"><span data-stu-id="313ee-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="313ee-121">为获得最佳性能，请仅选择所需的属性子集。</span><span class="sxs-lookup"><span data-stu-id="313ee-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="313ee-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="313ee-122">Request headers</span></span>

| <span data-ttu-id="313ee-123">名称</span><span class="sxs-lookup"><span data-stu-id="313ee-123">Name</span></span>           |<span data-ttu-id="313ee-124">说明</span><span class="sxs-lookup"><span data-stu-id="313ee-124">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="313ee-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="313ee-125">Authorization</span></span>  | <span data-ttu-id="313ee-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="313ee-p103">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="313ee-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="313ee-128">Request body</span></span>

<span data-ttu-id="313ee-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="313ee-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="313ee-130">响应</span><span class="sxs-lookup"><span data-stu-id="313ee-130">Response</span></span>

<span data-ttu-id="313ee-131">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [projectParticipation](../resources/projectparticipation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="313ee-131">If successful, this method returns a `200 OK` response code and the requested [projectParticipation](../resources/projectparticipation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="313ee-132">示例</span><span class="sxs-lookup"><span data-stu-id="313ee-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="313ee-133">请求</span><span class="sxs-lookup"><span data-stu-id="313ee-133">Request</span></span>

<span data-ttu-id="313ee-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="313ee-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="313ee-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="313ee-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_projectparticipation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/projects/{id}
```
# <a name="c"></a>[<span data-ttu-id="313ee-136">C#</span><span class="sxs-lookup"><span data-stu-id="313ee-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-projectparticipation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="313ee-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="313ee-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-projectparticipation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="313ee-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="313ee-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-projectparticipation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="313ee-139">Java</span><span class="sxs-lookup"><span data-stu-id="313ee-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-projectparticipation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="313ee-140">响应</span><span class="sxs-lookup"><span data-stu-id="313ee-140">Response</span></span>

<span data-ttu-id="313ee-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="313ee-141">The following is an example of the response.</span></span>

> <span data-ttu-id="313ee-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="313ee-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.projectParticipation"
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
  "categories": [
    "Branding"
  ],
  "client": {
    "displayName": "Contoso Ltd.",
    "pronunciation": null,
    "department": "Corporate Marketing",
    "officeLocation": null,
    "address": null,
    "webUrl": "https://www.contoso.com"
  },
  "displayName": "Contoso Re-branding Project",
  "detail": {
    "company": {
      "displayName": "Adventureworks Inc.",
      "pronunciation": null,
      "department": "Consulting",
      "officeLocation": null,
      "address": null,
      "webUrl": "https://adventureworks.com"
    },
    "description": "Rebranding of Contoso Ltd.",
    "endMonthYear": "datetime-value",
    "jobTitle": "Lead PM Rebranding",
    "role": "project management",
    "startMonthYear": "datetime-value",
    "summary": "A 6 month project to help Contoso rebrand after they were divested from a parent organization."
  },
  "colleagues": null,
  "sponsors": null
}
```


