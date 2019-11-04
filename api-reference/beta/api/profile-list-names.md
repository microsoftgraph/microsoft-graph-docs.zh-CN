---
title: 列出名称
description: 从用户的配置文件中检索 contact.personname 对象的列表。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5c13b3ee7454c8b8f0061aafbd9d0bebea6da94a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937768"
---
# <a name="list-names"></a><span data-ttu-id="e5170-103">列出名称</span><span class="sxs-lookup"><span data-stu-id="e5170-103">List names</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5170-104">从用户的[配置文件](../resources/profile.md)中检索[contact.personname](../resources/personname.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="e5170-104">Retrieve a list of [personName](../resources/personname.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e5170-105">权限</span><span class="sxs-lookup"><span data-stu-id="e5170-105">Permissions</span></span>

<span data-ttu-id="e5170-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5170-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e5170-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5170-108">Permission type</span></span>                        | <span data-ttu-id="e5170-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5170-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="e5170-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5170-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e5170-111">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="e5170-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e5170-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5170-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5170-113">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="e5170-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="e5170-114">Application</span><span class="sxs-lookup"><span data-stu-id="e5170-114">Application</span></span>                            | <span data-ttu-id="e5170-115">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="e5170-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="e5170-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5170-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/names
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e5170-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e5170-117">Optional query parameters</span></span>

<span data-ttu-id="e5170-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e5170-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e5170-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e5170-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5170-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5170-120">Request headers</span></span>

| <span data-ttu-id="e5170-121">名称</span><span class="sxs-lookup"><span data-stu-id="e5170-121">Name</span></span>           |<span data-ttu-id="e5170-122">说明</span><span class="sxs-lookup"><span data-stu-id="e5170-122">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="e5170-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5170-123">Authorization</span></span>  | <span data-ttu-id="e5170-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e5170-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="e5170-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e5170-126">Content-Type</span></span>   | <span data-ttu-id="e5170-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e5170-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5170-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5170-129">Request body</span></span> 

<span data-ttu-id="e5170-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e5170-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5170-131">响应</span><span class="sxs-lookup"><span data-stu-id="e5170-131">Response</span></span>

<span data-ttu-id="e5170-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[contact.personname](../resources/personname.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="e5170-132">If successful, this method returns a `200 OK` response code and a collection of [personName](../resources/personname.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e5170-133">示例</span><span class="sxs-lookup"><span data-stu-id="e5170-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e5170-134">请求</span><span class="sxs-lookup"><span data-stu-id="e5170-134">Request</span></span>

<span data-ttu-id="e5170-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e5170-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_names"
}-->

```http
GET https://graph.microsoft.com/beta/me/profile/names
```

### <a name="response"></a><span data-ttu-id="e5170-136">响应</span><span class="sxs-lookup"><span data-stu-id="e5170-136">Response</span></span>

<span data-ttu-id="e5170-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e5170-137">The following is an example of the response.</span></span>

> <span data-ttu-id="e5170-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e5170-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "displayName": "displayName-value",
      "first": "first-value",
      "initials": "initials-value",
      "last": "last-value",
      "languageTag": "languageTag-value",
      "maiden": "maiden-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List names",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->