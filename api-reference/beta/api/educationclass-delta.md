---
title: educationClass： delta
description: 获取新创建的或更新的类（包括成员身份更改），而无需对整个类集合执行完全读取。
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3b86b0c7fb39e274c553811ebb2a838613efedff
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909549"
---
# <a name="educationclass-delta"></a><span data-ttu-id="9400c-103">educationClass： delta</span><span class="sxs-lookup"><span data-stu-id="9400c-103">educationClass: delta</span></span>

<span data-ttu-id="9400c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9400c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9400c-105">获取新创建的或更新的类（包括成员身份更改），而无需对整个类集合执行完全读取。</span><span class="sxs-lookup"><span data-stu-id="9400c-105">Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection.</span></span> <span data-ttu-id="9400c-106">有关详细信息，请参阅[使用 delta 查询](/graph/delta-query-overview)。</span><span class="sxs-lookup"><span data-stu-id="9400c-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="9400c-107">权限</span><span class="sxs-lookup"><span data-stu-id="9400c-107">Permissions</span></span>

<span data-ttu-id="9400c-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="9400c-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="9400c-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9400c-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9400c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9400c-110">Permission type</span></span>                        | <span data-ttu-id="9400c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9400c-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="9400c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9400c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9400c-113">Eduroster.read.all、User.readbasic.all、Eduroster.read.all 或 Eduroster.read.all</span><span class="sxs-lookup"><span data-stu-id="9400c-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="9400c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9400c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9400c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9400c-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="9400c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9400c-116">Application</span></span>                            | <span data-ttu-id="9400c-117">Eduroster.read.all、Eduroster.read.all、All 或 Eduroster.read.all 的所有 User.readbasic.all</span><span class="sxs-lookup"><span data-stu-id="9400c-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9400c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9400c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/classes/{id}/delta
POST /education/me/classes/{id}/delta
```

## <a name="request-headers"></a><span data-ttu-id="9400c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9400c-119">Request headers</span></span>

| <span data-ttu-id="9400c-120">名称</span><span class="sxs-lookup"><span data-stu-id="9400c-120">Name</span></span>          | <span data-ttu-id="9400c-121">说明</span><span class="sxs-lookup"><span data-stu-id="9400c-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="9400c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9400c-122">Authorization</span></span> | <span data-ttu-id="9400c-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9400c-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9400c-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="9400c-124">Request body</span></span>

<span data-ttu-id="9400c-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9400c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9400c-126">响应</span><span class="sxs-lookup"><span data-stu-id="9400c-126">Response</span></span>

<span data-ttu-id="9400c-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[educationClass](../resources/educationclass.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="9400c-127">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) collection object in the response body.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9400c-128">educationClass 增量不包括已删除的类。</span><span class="sxs-lookup"><span data-stu-id="9400c-128">educationClass deltas do not include deleted classes.</span></span>

## <a name="example"></a><span data-ttu-id="9400c-129">示例</span><span class="sxs-lookup"><span data-stu-id="9400c-129">Example</span></span>

<span data-ttu-id="9400c-130">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="9400c-130">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="9400c-131">请求</span><span class="sxs-lookup"><span data-stu-id="9400c-131">Request</span></span>

<span data-ttu-id="9400c-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9400c-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationclass_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/classes/{id}/delta
```

##### <a name="response"></a><span data-ttu-id="9400c-133">响应</span><span class="sxs-lookup"><span data-stu-id="9400c-133">Response</span></span>

<span data-ttu-id="9400c-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9400c-134">The following is an example of the response.</span></span>

> <span data-ttu-id="9400c-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="9400c-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9400c-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="9400c-136">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 585

{
  "value": [
    {
      "displayName": "displayName-value",
      "mailNickname": "mailNickname-value",
      "description": "description-value",
      "createdBy": {
        "application": {
          "displayName": "displayName-value",
          "id": "id-value"
        },
        "device": {
          "displayName": "displayName-value",
          "id": "id-value"
        },
        "user": {
          "displayName": "displayName-value",
          "id": "id-value"
        }
      },
      "classCode": "classCode-value",
      "externalName": "externalName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationClass: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
