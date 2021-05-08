---
title: 列出 educationClasses
description: 获取 educationClass 对象及其属性的列表。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6b599217cfb87a853fdc6630f210bea969cbaa97
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232159"
---
# <a name="list-educationclasses"></a><span data-ttu-id="a2301-103">列出 educationClasses</span><span class="sxs-lookup"><span data-stu-id="a2301-103">List educationClasses</span></span>

<span data-ttu-id="a2301-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2301-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a2301-105">获取 [educationClass 对象](../resources/educationclass.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="a2301-105">Get a list of the [educationClass](../resources/educationclass.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2301-106">权限</span><span class="sxs-lookup"><span data-stu-id="a2301-106">Permissions</span></span>

<span data-ttu-id="a2301-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2301-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a2301-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2301-109">Permission type</span></span>                        | <span data-ttu-id="a2301-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a2301-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a2301-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2301-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2301-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="a2301-112">EduRoster.ReadBasic</span></span>                         |
| <span data-ttu-id="a2301-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2301-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2301-114">不支持</span><span class="sxs-lookup"><span data-stu-id="a2301-114">Not supported</span></span>                               |
| <span data-ttu-id="a2301-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2301-115">Application</span></span>                            | <span data-ttu-id="a2301-116">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2301-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a2301-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2301-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/classes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a2301-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a2301-118">Optional query parameters</span></span>

<span data-ttu-id="a2301-119">可以使用 OData 查询选项 `$orderby`，按 **displayName** 值对组织中的组进行排序，如下面的示例所示：</span><span class="sxs-lookup"><span data-stu-id="a2301-119">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

<span data-ttu-id="a2301-120">您还可以使用 和 `$filter` `$count` `$search` 查询参数来限制响应。</span><span class="sxs-lookup"><span data-stu-id="a2301-120">You can also use the `$filter`, `$count` and `$search` query parameters to limit the response.</span></span> 

<span data-ttu-id="a2301-121">为该资源添加或更新项目时，将对它们进行专门索引，以便与 `$count` 和 `$search` 查询参数一起使用。</span><span class="sxs-lookup"><span data-stu-id="a2301-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="a2301-122">在添加或更新项目与在索引中可用之间可能会稍有延迟。</span><span class="sxs-lookup"><span data-stu-id="a2301-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

<span data-ttu-id="a2301-123">有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="a2301-123">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2301-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2301-124">Request headers</span></span>

| <span data-ttu-id="a2301-125">名称</span><span class="sxs-lookup"><span data-stu-id="a2301-125">Name</span></span>          | <span data-ttu-id="a2301-126">说明</span><span class="sxs-lookup"><span data-stu-id="a2301-126">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a2301-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2301-127">Authorization</span></span> | <span data-ttu-id="a2301-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a2301-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a2301-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2301-130">Request body</span></span>

<span data-ttu-id="a2301-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a2301-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2301-132">响应</span><span class="sxs-lookup"><span data-stu-id="a2301-132">Response</span></span>

<span data-ttu-id="a2301-133">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="a2301-133">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a2301-134">示例</span><span class="sxs-lookup"><span data-stu-id="a2301-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a2301-135">请求</span><span class="sxs-lookup"><span data-stu-id="a2301-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_educationclass"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/classes
```

### <a name="response"></a><span data-ttu-id="a2301-136">响应</span><span class="sxs-lookup"><span data-stu-id="a2301-136">Response</span></span>

> <span data-ttu-id="a2301-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a2301-137">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.educationClass)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationClass",
      "id": "64ef8ce5-8ce5-64ef-e58c-ef64e58cef64",
      "displayName": "String",
      "mailNickname": "String",
      "description": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "classCode": "String",
      "externalName": "String",
      "externalId": "String",
      "externalSource": "String",
      "externalSourceDetail": "String",
      "grade": "String",
      "term": {
        "@odata.type": "microsoft.graph.educationTerm"
      }
    }
  ]
}
```
