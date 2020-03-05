---
title: educationSchool： delta
description: 获取新创建或更新的学校，而无需对整个学校集合执行完全读取。
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b34ff6bad00194ce6d1967e503e280d0e0af2478
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42425553"
---
# <a name="educationschool-delta"></a><span data-ttu-id="fe355-103">educationSchool： delta</span><span class="sxs-lookup"><span data-stu-id="fe355-103">educationSchool: delta</span></span>

<span data-ttu-id="fe355-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="fe355-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe355-105">获取新创建或更新的学校，而无需对整个学校集合执行完全读取。</span><span class="sxs-lookup"><span data-stu-id="fe355-105">Get newly created or updated schools without having to perform a full read of the entire school collection.</span></span> <span data-ttu-id="fe355-106">有关详细信息，请参阅[使用 delta 查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="fe355-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe355-107">权限</span><span class="sxs-lookup"><span data-stu-id="fe355-107">Permissions</span></span>

<span data-ttu-id="fe355-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe355-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fe355-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe355-110">Permission type</span></span>                        | <span data-ttu-id="fe355-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe355-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="fe355-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe355-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe355-113">Eduroster.read.all、User.readbasic.all、Eduroster.read.all 或 Eduroster.read.all</span><span class="sxs-lookup"><span data-stu-id="fe355-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="fe355-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe355-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe355-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe355-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="fe355-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe355-116">Application</span></span>                            | <span data-ttu-id="fe355-117">Eduroster.read.all、Eduroster.read.all、All 或 Eduroster.read.all 的所有 User.readbasic.all</span><span class="sxs-lookup"><span data-stu-id="fe355-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe355-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe355-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/schools/{id}/delta
POST /education/me/schools/{id}/delta
POST /education/users/{id}/schools/{id}/delta

```

## <a name="request-headers"></a><span data-ttu-id="fe355-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe355-119">Request headers</span></span>

| <span data-ttu-id="fe355-120">名称</span><span class="sxs-lookup"><span data-stu-id="fe355-120">Name</span></span>          | <span data-ttu-id="fe355-121">说明</span><span class="sxs-lookup"><span data-stu-id="fe355-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="fe355-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe355-122">Authorization</span></span> | <span data-ttu-id="fe355-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="fe355-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe355-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe355-124">Request body</span></span>

<span data-ttu-id="fe355-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fe355-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe355-126">响应</span><span class="sxs-lookup"><span data-stu-id="fe355-126">Response</span></span>

<span data-ttu-id="fe355-127">如果成功，此方法在响应`200 OK`正文中返回响应代码和[educationSchool](../resources/educationschool.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="fe355-127">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe355-128">示例</span><span class="sxs-lookup"><span data-stu-id="fe355-128">Example</span></span>

<span data-ttu-id="fe355-129">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="fe355-129">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="fe355-130">请求</span><span class="sxs-lookup"><span data-stu-id="fe355-130">Request</span></span>

<span data-ttu-id="fe355-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fe355-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationschool_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/schools/{id}/delta
```

##### <a name="response"></a><span data-ttu-id="fe355-132">响应</span><span class="sxs-lookup"><span data-stu-id="fe355-132">Response</span></span>

<span data-ttu-id="fe355-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fe355-133">The following is an example of the response.</span></span> 

><span data-ttu-id="fe355-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fe355-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 313

{
  "value": [
    {
      "principalEmail": "principalEmail-value",
      "principalName": "principalName-value",
      "externalPrincipalId": "externalPrincipalId-value",
      "lowestGrade": "lowestGrade-value",
      "highestGrade": "highestGrade-value",
      "schoolNumber": "schoolNumber-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
