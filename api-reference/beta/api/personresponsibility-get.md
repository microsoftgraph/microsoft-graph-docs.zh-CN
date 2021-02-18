---
title: 获取 personResponsibility
description: 读取 personResponsibility 对象的属性和关系。
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 244313cd23c3a5635d75d3af7242df138ce253a5
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292705"
---
# <a name="get-personresponsibility"></a><span data-ttu-id="b3ba5-103">获取 personResponsibility</span><span class="sxs-lookup"><span data-stu-id="b3ba5-103">Get personResponsibility</span></span>
<span data-ttu-id="b3ba5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3ba5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b3ba5-105">读取用户配置文件中的 [personResponsibility](../resources/personresponsibility.md) 对象的属性和 [关系](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="b3ba5-105">Read the properties and relationships of a [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b3ba5-106">权限</span><span class="sxs-lookup"><span data-stu-id="b3ba5-106">Permissions</span></span>

<span data-ttu-id="b3ba5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b3ba5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b3ba5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3ba5-109">Permission type</span></span>                        | <span data-ttu-id="b3ba5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b3ba5-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="b3ba5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3ba5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3ba5-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3ba5-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b3ba5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3ba5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3ba5-114">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3ba5-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b3ba5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3ba5-115">Application</span></span>                            | <span data-ttu-id="b3ba5-116">User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3ba5-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="b3ba5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3ba5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/responsibilities/{id}
GET /users/{id | userPrincipalName}/responsibilities/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b3ba5-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b3ba5-118">Optional query parameters</span></span>

<span data-ttu-id="b3ba5-119">此方法支持 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="b3ba5-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="b3ba5-120">指定要包括在响应中的属性列表，用逗号分隔它们。</span><span class="sxs-lookup"><span data-stu-id="b3ba5-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="b3ba5-121">为获得最佳性能，请仅选择所需的属性子集。</span><span class="sxs-lookup"><span data-stu-id="b3ba5-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3ba5-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3ba5-122">Request headers</span></span>
|<span data-ttu-id="b3ba5-123">名称</span><span class="sxs-lookup"><span data-stu-id="b3ba5-123">Name</span></span>|<span data-ttu-id="b3ba5-124">说明</span><span class="sxs-lookup"><span data-stu-id="b3ba5-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b3ba5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3ba5-125">Authorization</span></span>|<span data-ttu-id="b3ba5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b3ba5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3ba5-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3ba5-128">Request body</span></span>
<span data-ttu-id="b3ba5-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b3ba5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3ba5-130">响应</span><span class="sxs-lookup"><span data-stu-id="b3ba5-130">Response</span></span>

<span data-ttu-id="b3ba5-131">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [personResponsibility](../resources/personresponsibility.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b3ba5-131">If successful, this method returns a `200 OK` response code and a [personResponsibility](../resources/personresponsibility.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b3ba5-132">示例</span><span class="sxs-lookup"><span data-stu-id="b3ba5-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b3ba5-133">请求</span><span class="sxs-lookup"><span data-stu-id="b3ba5-133">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f"],
  "name": "get_personresponsibility"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/responsibilities/0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f
```

### <a name="response"></a><span data-ttu-id="b3ba5-134">响应</span><span class="sxs-lookup"><span data-stu-id="b3ba5-134">Response</span></span>
<span data-ttu-id="b3ba5-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b3ba5-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personResponsibility"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

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
  "description": "Member of the Microsoft API Council",
  "displayName": "API Council",
  "webUrl": null,
  "collaborationTags": [
    "askMeAbout"
  ]
}
```


