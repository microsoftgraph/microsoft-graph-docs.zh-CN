---
title: 删除 educationRubric
description: 删除 educationRubric 对象。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f54816be7872734ecbd6d8a0b46a8a57694b4c68
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173151"
---
# <a name="delete-educationrubric"></a><span data-ttu-id="7a3b6-103">删除 educationRubric</span><span class="sxs-lookup"><span data-stu-id="7a3b6-103">Delete educationRubric</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a3b6-104">删除[educationRubric](../resources/educationrubric.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7a3b6-104">Delete an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a3b6-105">权限</span><span class="sxs-lookup"><span data-stu-id="7a3b6-105">Permissions</span></span>

<span data-ttu-id="7a3b6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7a3b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7a3b6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7a3b6-108">Permission type</span></span>                        | <span data-ttu-id="7a3b6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7a3b6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7a3b6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7a3b6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7a3b6-111">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="7a3b6-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="7a3b6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7a3b6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a3b6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a3b6-113">Not supported.</span></span> |
| <span data-ttu-id="7a3b6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7a3b6-114">Application</span></span>                            | <span data-ttu-id="7a3b6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a3b6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a3b6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7a3b6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/me/rubrics/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7a3b6-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7a3b6-117">Request headers</span></span>

| <span data-ttu-id="7a3b6-118">名称</span><span class="sxs-lookup"><span data-stu-id="7a3b6-118">Name</span></span>          | <span data-ttu-id="7a3b6-119">说明</span><span class="sxs-lookup"><span data-stu-id="7a3b6-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7a3b6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a3b6-120">Authorization</span></span> | <span data-ttu-id="7a3b6-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="7a3b6-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a3b6-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="7a3b6-122">Request body</span></span>

<span data-ttu-id="7a3b6-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7a3b6-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a3b6-124">响应</span><span class="sxs-lookup"><span data-stu-id="7a3b6-124">Response</span></span>

<span data-ttu-id="7a3b6-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7a3b6-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7a3b6-127">示例</span><span class="sxs-lookup"><span data-stu-id="7a3b6-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7a3b6-128">请求</span><span class="sxs-lookup"><span data-stu-id="7a3b6-128">Request</span></span>

<span data-ttu-id="7a3b6-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7a3b6-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/rubrics/{id}
```

### <a name="response"></a><span data-ttu-id="7a3b6-130">响应</span><span class="sxs-lookup"><span data-stu-id="7a3b6-130">Response</span></span>

<span data-ttu-id="7a3b6-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7a3b6-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->