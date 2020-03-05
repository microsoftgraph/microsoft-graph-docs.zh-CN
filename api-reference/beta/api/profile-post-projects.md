---
title: 创建 projectParticipation
description: 使用此 API 创建新的 projectParticipation。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1c77cbf9f6b594bb40cb04e94d2594f67eee2997
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455065"
---
# <a name="create-projectparticipation"></a><span data-ttu-id="609c7-103">创建 projectParticipation</span><span class="sxs-lookup"><span data-stu-id="609c7-103">Create projectParticipation</span></span>

<span data-ttu-id="609c7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="609c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="609c7-105">使用此 API 在用户的[配置文件](../resources/profile.md)中创建新的[projectParticipation](../resources/projectParticipation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="609c7-105">Use this API to create a new [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="609c7-106">权限</span><span class="sxs-lookup"><span data-stu-id="609c7-106">Permissions</span></span>

<span data-ttu-id="609c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="609c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="609c7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="609c7-109">Permission type</span></span>                        | <span data-ttu-id="609c7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="609c7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="609c7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="609c7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="609c7-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="609c7-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="609c7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="609c7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="609c7-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="609c7-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="609c7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="609c7-115">Application</span></span>                            | <span data-ttu-id="609c7-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="609c7-116">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="609c7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="609c7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/projects
```

## <a name="request-headers"></a><span data-ttu-id="609c7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="609c7-118">Request headers</span></span>

| <span data-ttu-id="609c7-119">名称</span><span class="sxs-lookup"><span data-stu-id="609c7-119">Name</span></span>      |<span data-ttu-id="609c7-120">说明</span><span class="sxs-lookup"><span data-stu-id="609c7-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="609c7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="609c7-121">Authorization</span></span>  | <span data-ttu-id="609c7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="609c7-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="609c7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="609c7-124">Content-Type</span></span>   | <span data-ttu-id="609c7-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="609c7-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="609c7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="609c7-127">Request body</span></span>

<span data-ttu-id="609c7-128">在请求正文中，提供[projectParticipation](../resources/projectparticipation.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="609c7-128">In the request body, supply a JSON representation of [projectParticipation](../resources/projectparticipation.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="609c7-129">响应</span><span class="sxs-lookup"><span data-stu-id="609c7-129">Response</span></span>

<span data-ttu-id="609c7-130">如果成功，此方法在`201, Created`响应正文中返回响应代码和新的[projectParticipation](../resources/projectparticipation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="609c7-130">If successful, this method returns `201, Created` response code and a new [projectParticipation](../resources/projectparticipation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="609c7-131">示例</span><span class="sxs-lookup"><span data-stu-id="609c7-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="609c7-132">请求</span><span class="sxs-lookup"><span data-stu-id="609c7-132">Request</span></span>

<span data-ttu-id="609c7-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="609c7-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="609c7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="609c7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_projectparticipation_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/projects
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "client": {
    "displayName": "displayName-value",
    "pronunciation": "pronunciation-value",
    "department": "department-value",
    "officeLocation": "officeLocation-value",
    "address": {
      "type": "type-value",
      "postOfficeBox": "postOfficeBox-value",
      "street": "street-value",
      "city": "city-value",
      "state": "state-value",
      "countryOrRegion": "countryOrRegion-value",
      "postalCode": "postalCode-value"
    },
    "webUrl": "webUrl-value"
  },
  "displayName": "displayName-value",
  "detail": {
    "company": {
      "displayName": "displayName-value",
      "pronunciation": "pronunciation-value",
      "department": "department-value",
      "officeLocation": "officeLocation-value",
      "address": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "webUrl": "webUrl-value"
    },
    "description": "description-value",
    "endMonthYear": "datetime-value",
    "jobTitle": "jobTitle-value",
    "role": "role-value",
    "startMonthYear": "datetime-value",
    "summary": "summary-value"
  },
  "colleagues": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ],
  "sponsors": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="609c7-135">C#</span><span class="sxs-lookup"><span data-stu-id="609c7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-projectparticipation-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="609c7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="609c7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-projectparticipation-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="609c7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="609c7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-projectparticipation-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="609c7-138">响应</span><span class="sxs-lookup"><span data-stu-id="609c7-138">Response</span></span>

<span data-ttu-id="609c7-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="609c7-139">The following is an example of the response.</span></span>

> <span data-ttu-id="609c7-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="609c7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.projectParticipation"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "client": {
    "displayName": "displayName-value",
    "pronunciation": "pronunciation-value",
    "department": "department-value",
    "officeLocation": "officeLocation-value",
    "address": {
      "type": "type-value",
      "postOfficeBox": "postOfficeBox-value",
      "street": "street-value",
      "city": "city-value",
      "state": "state-value",
      "countryOrRegion": "countryOrRegion-value",
      "postalCode": "postalCode-value"
    },
    "webUrl": "webUrl-value"
  },
  "displayName": "displayName-value",
  "detail": {
    "company": {
      "displayName": "displayName-value",
      "pronunciation": "pronunciation-value",
      "department": "department-value",
      "officeLocation": "officeLocation-value",
      "address": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "webUrl": "webUrl-value"
    },
    "description": "description-value",
    "endMonthYear": "datetime-value",
    "jobTitle": "jobTitle-value",
    "role": "role-value",
    "startMonthYear": "datetime-value",
    "summary": "summary-value"
  },
  "colleagues": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ],
  "sponsors": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create projectParticipation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
