---
title: 更新 authenticationContextClassReference
description: 更新 authenticationContextClassReference 对象的属性。
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: dcc0a20ac8b10fc1b7fad3fa3472832036f70024
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547327"
---
# <a name="update-authenticationcontextclassreference"></a><span data-ttu-id="40f24-103">更新 authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="40f24-103">Update authenticationContextClassReference</span></span>

<span data-ttu-id="40f24-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40f24-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40f24-105">更新 [authenticationContextClassReference 对象](../resources/authenticationcontextclassreference.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="40f24-105">Update the properties of an [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="40f24-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="40f24-106">Permissions</span></span>

<span data-ttu-id="40f24-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="40f24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40f24-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="40f24-109">Permission type</span></span>                        | <span data-ttu-id="40f24-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="40f24-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="40f24-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40f24-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="40f24-112">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="40f24-112">Policy.ReadWrite.ConditionalAccess</span></span> |
|<span data-ttu-id="40f24-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40f24-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40f24-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="40f24-114">Not supported.</span></span> |
|<span data-ttu-id="40f24-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="40f24-115">Application</span></span>                            | <span data-ttu-id="40f24-116">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="40f24-116">Policy.ReadWrite.ConditionalAccess</span></span> |

> [!NOTE]
> <span data-ttu-id="40f24-117">此 API 有 [一个与](/graph/known-issues#permissions) 权限相关的已知问题。</span><span class="sxs-lookup"><span data-stu-id="40f24-117">This API has a [known issue](/graph/known-issues#permissions) related to permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="40f24-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40f24-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/conditionalAccess/authenticationContextClassReferences/{id}
```

## <a name="request-headers"></a><span data-ttu-id="40f24-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="40f24-119">Request headers</span></span>

| <span data-ttu-id="40f24-120">名称</span><span class="sxs-lookup"><span data-stu-id="40f24-120">Name</span></span>          | <span data-ttu-id="40f24-121">说明</span><span class="sxs-lookup"><span data-stu-id="40f24-121">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="40f24-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="40f24-122">Authorization</span></span> | <span data-ttu-id="40f24-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="40f24-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="40f24-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40f24-125">Content-Type</span></span>  | <span data-ttu-id="40f24-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="40f24-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40f24-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="40f24-128">Request body</span></span>

<span data-ttu-id="40f24-129">在请求正文中，提供应更新的相关属性的值。</span><span class="sxs-lookup"><span data-stu-id="40f24-129">In the request body, supply the values for relevant properties that should be updated.</span></span> <span data-ttu-id="40f24-130">未添加到请求正文的现有属性要么保留旧值，要么根据其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="40f24-130">Existing properties that are not included in the request body maintain their previous values or are recalculated based on changes to other property values.</span></span> <span data-ttu-id="40f24-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="40f24-131">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="40f24-132">有关属性的列表，请参阅 [authenticationContextClassReference](../resources/authenticationContextClassReference.md)。</span><span class="sxs-lookup"><span data-stu-id="40f24-132">For the list of properties, see [authenticationContextClassReference](../resources/authenticationContextClassReference.md).</span></span>

## <a name="response"></a><span data-ttu-id="40f24-133">响应</span><span class="sxs-lookup"><span data-stu-id="40f24-133">Response</span></span>

<span data-ttu-id="40f24-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="40f24-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="40f24-136">示例</span><span class="sxs-lookup"><span data-stu-id="40f24-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="40f24-137">请求</span><span class="sxs-lookup"><span data-stu-id="40f24-137">Request</span></span>

<span data-ttu-id="40f24-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="40f24-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_authenticationcontextclassreference"
}-->

```http
PATCH https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences/c1
Content-type: application/json

{
   "value": 
    [
      {
         "displayName": "Contoso trusted locations",
        "description": "Access is only allowed from trusted locations",
        "isAvailable": true
      }
    ]
}
```



### <a name="response"></a><span data-ttu-id="40f24-139">响应</span><span class="sxs-lookup"><span data-stu-id="40f24-139">Response</span></span>

<span data-ttu-id="40f24-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="40f24-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update authenticationContextClassReference",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
