---
title: educationUser： delta
description: 获取新创建或更新的用户，而无需对整个用户集执行完全读取。
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3d96334c4a7f3fd6974fdf08c2eb86809e89326d
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006826"
---
# <a name="educationuser-delta"></a><span data-ttu-id="c607a-103">educationUser： delta</span><span class="sxs-lookup"><span data-stu-id="c607a-103">educationUser: delta</span></span>

<span data-ttu-id="c607a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c607a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c607a-105">获取新创建或更新的[educationUser](../resources/educationuser.md) ，而无需对整个集合执行完全读取。</span><span class="sxs-lookup"><span data-stu-id="c607a-105">Get newly created or updated [educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection.</span></span> <span data-ttu-id="c607a-106">有关详细信息，请参阅[使用 delta 查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="c607a-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="c607a-107">权限</span><span class="sxs-lookup"><span data-stu-id="c607a-107">Permissions</span></span>

<span data-ttu-id="c607a-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c607a-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c607a-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c607a-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c607a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c607a-110">Permission type</span></span>                        | <span data-ttu-id="c607a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c607a-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="c607a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c607a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c607a-113">Eduroster.read.all、User.readbasic.all、Eduroster.read.all 或 Eduroster.read.all</span><span class="sxs-lookup"><span data-stu-id="c607a-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="c607a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c607a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c607a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c607a-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="c607a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c607a-116">Application</span></span>                            | <span data-ttu-id="c607a-117">Eduroster.read.all、Eduroster.read.all、All 或 Eduroster.read.all 的所有 User.readbasic.all</span><span class="sxs-lookup"><span data-stu-id="c607a-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c607a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c607a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/users/delta
```

## <a name="request-headers"></a><span data-ttu-id="c607a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c607a-119">Request headers</span></span>

| <span data-ttu-id="c607a-120">名称</span><span class="sxs-lookup"><span data-stu-id="c607a-120">Name</span></span>          | <span data-ttu-id="c607a-121">说明</span><span class="sxs-lookup"><span data-stu-id="c607a-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="c607a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c607a-122">Authorization</span></span> | <span data-ttu-id="c607a-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c607a-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c607a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="c607a-124">Request body</span></span>

<span data-ttu-id="c607a-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c607a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c607a-126">响应</span><span class="sxs-lookup"><span data-stu-id="c607a-126">Response</span></span>

<span data-ttu-id="c607a-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[educationUser](../resources/educationuser.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="c607a-127">If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) collection object in the response body.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c607a-128">educationUser 增量不包括已删除的用户。</span><span class="sxs-lookup"><span data-stu-id="c607a-128">educationUser deltas do not include deleted users.</span></span>

## <a name="example"></a><span data-ttu-id="c607a-129">示例</span><span class="sxs-lookup"><span data-stu-id="c607a-129">Example</span></span>

<span data-ttu-id="c607a-130">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="c607a-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c607a-131">请求</span><span class="sxs-lookup"><span data-stu-id="c607a-131">Request</span></span>

<span data-ttu-id="c607a-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c607a-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}-->

```http
GET https://graph.microsoft.com/beta/education/users/delta
```

### <a name="response"></a><span data-ttu-id="c607a-133">响应</span><span class="sxs-lookup"><span data-stu-id="c607a-133">Response</span></span>

<span data-ttu-id="c607a-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c607a-134">The following is an example of the response.</span></span>

> <span data-ttu-id="c607a-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="c607a-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c607a-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="c607a-136">All the properties will be returned from an actual call.</span></span>

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
      "accountEnabled": true,
      "assignedLicenses": [{ "@odata.type": "microsoft.graph.assignedLicense" }],
      "assignedPlans": [{ "@odata.type": "microsoft.graph.assignedPlan" }],
      "businessPhones": ["String"],
      "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
      "department": "String",
      "displayName": "String",
      "externalSource": "string",
      "givenName": "String",
      "id": "String (identifier)",
      "mail": "String",
      "mailNickname": "String",
      "mailingAddress": { "@odata.type": "microsoft.graph.physicalAddress" },
      "middleName": "String",
      "mobilePhone": "String",
      "officeLocation": "String",
      "onPremisesInfo": {
        "@odata.type": "microsoft.graph.educationOnPremisesInfo"
      },
      "passwordPolicies": "String",
      "passwordProfile": { "@odata.type": "microsoft.graph.passwordProfile" },
      "preferredLanguage": "String",
      "primaryRole": "string",
      "provisionedPlans": [{ "@odata.type": "microsoft.graph.provisionedPlan" }],
      "residenceAddress": { "@odata.type": "microsoft.graph.physicalAddress" },
      "student": { "@odata.type": "microsoft.graph.educationStudent" },
      "surname": "String",
      "teacher": { "@odata.type": "microsoft.graph.educationTeacher" },
      "usageLocation": "String",
      "userPrincipalName": "String",
      "userType": "String"
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
