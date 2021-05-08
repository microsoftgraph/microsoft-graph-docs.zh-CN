---
title: educationClass： delta
description: 获取新创建或更新的类（包括成员身份更改）而无需执行整个类集合的完全读取。
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 80ca48a1494281fed4a39dfff342233a268b5122
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232168"
---
# <a name="educationclass-delta"></a><span data-ttu-id="8848a-103">educationClass： delta</span><span class="sxs-lookup"><span data-stu-id="8848a-103">educationClass: delta</span></span>

<span data-ttu-id="8848a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8848a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8848a-105">获取新创建或更新的类（包括成员身份更改）而无需执行整个类集合的完全读取。</span><span class="sxs-lookup"><span data-stu-id="8848a-105">Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection.</span></span> <span data-ttu-id="8848a-106">有关详细信息 [，请参阅使用 delta](/graph/delta-query-overview) 查询。</span><span class="sxs-lookup"><span data-stu-id="8848a-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="8848a-107">权限</span><span class="sxs-lookup"><span data-stu-id="8848a-107">Permissions</span></span>

<span data-ttu-id="8848a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8848a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8848a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8848a-110">Permission type</span></span>                        | <span data-ttu-id="8848a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8848a-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="8848a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8848a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8848a-113">EduRoster.ReadBasic、EduRoster.Read 或 EduRoster.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8848a-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="8848a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8848a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8848a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8848a-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="8848a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8848a-116">Application</span></span>                            | <span data-ttu-id="8848a-117">EduRoster.ReadBasic.All、EduRoster.Read.All 或 EduRoster.WriteWrite.All</span><span class="sxs-lookup"><span data-stu-id="8848a-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8848a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8848a-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/classes/delta
```

## <a name="request-headers"></a><span data-ttu-id="8848a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8848a-119">Request headers</span></span>

| <span data-ttu-id="8848a-120">名称</span><span class="sxs-lookup"><span data-stu-id="8848a-120">Name</span></span>          | <span data-ttu-id="8848a-121">说明</span><span class="sxs-lookup"><span data-stu-id="8848a-121">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8848a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8848a-122">Authorization</span></span> | <span data-ttu-id="8848a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8848a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8848a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8848a-125">Request body</span></span>

<span data-ttu-id="8848a-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8848a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8848a-127">响应</span><span class="sxs-lookup"><span data-stu-id="8848a-127">Response</span></span>

<span data-ttu-id="8848a-128">如果成功，此函数在响应 `200 OK` 正文中返回 响应代码和 [educationClass](../resources/educationclass.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="8848a-128">If successful, this function returns an `200 OK` response code and an [educationClass](../resources/educationclass.md) collection in the response body.</span></span> <span data-ttu-id="8848a-129">该响应还包括 `nextLink`URL 或 `deltaLink`URL。</span><span class="sxs-lookup"><span data-stu-id="8848a-129">The response also includes a `nextLink` URL or a `deltaLink` URL.</span></span>

- <span data-ttu-id="8848a-130">如果 `nextLink` 返回 URL，则会话中有其他要检索的数据页。</span><span class="sxs-lookup"><span data-stu-id="8848a-130">If a `nextLink` URL is returned, there are additional pages of data to be retrieved in the session.</span></span> <span data-ttu-id="8848a-131">应用程序继续使用 `nextLink` URL 发出请求，直到响应中包含 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="8848a-131">The application continues making requests using the `nextLink` URL until a `deltaLink` URL is included in the response.</span></span>
- <span data-ttu-id="8848a-132">如果 `deltaLink` 返回 URL，则不再返回有关资源现有状态的数据。</span><span class="sxs-lookup"><span data-stu-id="8848a-132">If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned.</span></span> <span data-ttu-id="8848a-133">保留并使用 `deltaLink` URL 了解将来对资源的更改。</span><span class="sxs-lookup"><span data-stu-id="8848a-133">Persist and use the `deltaLink` URL to learn about changes to the resource in the future.</span></span>

<span data-ttu-id="8848a-134">有关详细信息，请参阅使用 [delta 查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="8848a-134">For details, see [Using delta query](/graph/delta-query-overview).</span></span> <span data-ttu-id="8848a-135">有关示例请求，请参阅 [获取用户的增量更改](/graph/delta-query-users)。</span><span class="sxs-lookup"><span data-stu-id="8848a-135">For example requests, see [Get incremental changes for users](/graph/delta-query-users).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="8848a-136">educationClass deltas 不包括已删除的类。</span><span class="sxs-lookup"><span data-stu-id="8848a-136">educationClass deltas do not include deleted classes.</span></span>

## <a name="examples"></a><span data-ttu-id="8848a-137">示例</span><span class="sxs-lookup"><span data-stu-id="8848a-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8848a-138">请求</span><span class="sxs-lookup"><span data-stu-id="8848a-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "educationclass_delta"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/classes/delta
```

### <a name="response"></a><span data-ttu-id="8848a-139">响应</span><span class="sxs-lookup"><span data-stu-id="8848a-139">Response</span></span>

> <span data-ttu-id="8848a-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8848a-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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

  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(educationClass)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/education/classes/delta?$skiptoken=sU1S4IJGk3hwxbia8...",
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationClass",
      "id": "String (identifier)",
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
