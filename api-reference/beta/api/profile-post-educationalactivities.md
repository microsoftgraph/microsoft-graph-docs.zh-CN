---
title: 创建 educationalActivity
description: 创建新的 educationalActivity。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9d860955227de6b85f110c794e264559586fa172
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937712"
---
# <a name="create-educationalactivity"></a><span data-ttu-id="02cdc-103">创建 educationalActivity</span><span class="sxs-lookup"><span data-stu-id="02cdc-103">Create educationalActivity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02cdc-104">在用户的[配置文件](../resources/profile.md)中创建新的[educationalActivity](../resources/educationalactivity.md) 。</span><span class="sxs-lookup"><span data-stu-id="02cdc-104">Create a new [educationalActivity](../resources/educationalactivity.md) in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="02cdc-105">权限</span><span class="sxs-lookup"><span data-stu-id="02cdc-105">Permissions</span></span>

<span data-ttu-id="02cdc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="02cdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="02cdc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="02cdc-108">Permission type</span></span>                        | <span data-ttu-id="02cdc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="02cdc-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="02cdc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02cdc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="02cdc-111">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="02cdc-111">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="02cdc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02cdc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02cdc-113">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="02cdc-113">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="02cdc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="02cdc-114">Application</span></span>                            | <span data-ttu-id="02cdc-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02cdc-115">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02cdc-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02cdc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /user/profile/educationalActivities
```

## <a name="request-headers"></a><span data-ttu-id="02cdc-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="02cdc-117">Request headers</span></span>

| <span data-ttu-id="02cdc-118">名称</span><span class="sxs-lookup"><span data-stu-id="02cdc-118">Name</span></span>      |<span data-ttu-id="02cdc-119">说明</span><span class="sxs-lookup"><span data-stu-id="02cdc-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="02cdc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="02cdc-120">Authorization</span></span>  | <span data-ttu-id="02cdc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="02cdc-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="02cdc-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="02cdc-123">Content-Type</span></span>   | <span data-ttu-id="02cdc-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="02cdc-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02cdc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="02cdc-126">Request body</span></span>

<span data-ttu-id="02cdc-127">在请求正文中，提供[educationalActivity](../resources/educationalactivity.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02cdc-127">In the request body, supply a JSON representation of an [educationalActivity](../resources/educationalactivity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="02cdc-128">响应</span><span class="sxs-lookup"><span data-stu-id="02cdc-128">Response</span></span>

<span data-ttu-id="02cdc-129">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[educationalActivity](../resources/educationalactivity.md)对象。</span><span class="sxs-lookup"><span data-stu-id="02cdc-129">If successful, this method returns a `201 Created` response code and a new [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="02cdc-130">示例</span><span class="sxs-lookup"><span data-stu-id="02cdc-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="02cdc-131">请求</span><span class="sxs-lookup"><span data-stu-id="02cdc-131">Request</span></span>

<span data-ttu-id="02cdc-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="02cdc-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationalactivity_from_profile"
}-->

```http
POST /me/profile/educationalActivities
Content-type: application/json

{
  "completionMonthYear": "datetime-value",
  "endMonthYear": "datetime-value",
  "institution": {
    "description": "description-value",
    "displayName": "displayName-value",
    "location": {
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
  "program": {
    "abbreviation": "abbreviation-value",
    "activities": "activities-value",
    "awards": "awards-value",
    "description": "description-value",
    "displayName": "displayName-value",
    "fieldsOfStudy": "fieldsOfStudy-value",
    "grade": "grade-value",
    "notes": "notes-value",
    "webUrl": "webUrl-value"
  },
  "startMonthYear": "datetime-value"
}
```

### <a name="response"></a><span data-ttu-id="02cdc-133">响应</span><span class="sxs-lookup"><span data-stu-id="02cdc-133">Response</span></span>

<span data-ttu-id="02cdc-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="02cdc-134">The following is an example of the response.</span></span>

> <span data-ttu-id="02cdc-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="02cdc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalActivity"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "completionMonthYear": "datetime-value",
  "endMonthYear": "datetime-value",
  "institution": {
    "description": "description-value",
    "displayName": "displayName-value",
    "location": {
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
  "program": {
    "abbreviation": "abbreviation-value",
    "activities": "activities-value",
    "awards": "awards-value",
    "description": "description-value",
    "displayName": "displayName-value",
    "fieldsOfStudy": "fieldsOfStudy-value",
    "grade": "grade-value",
    "notes": "notes-value",
    "webUrl": "webUrl-value"
  },
  "startMonthYear": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationalActivity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
