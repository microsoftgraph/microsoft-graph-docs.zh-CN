---
title: 创建 authenticationContextClassReference
description: 创建新的 authenticationContextClassReference。
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8ad536988d73e8550ec4561f0ca6ead77c40d256
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547335"
---
# <a name="create-authenticationcontextclassreference"></a><span data-ttu-id="25ef4-103">创建 authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="25ef4-103">Create authenticationContextClassReference</span></span>

<span data-ttu-id="25ef4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25ef4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25ef4-105">创建新的 [authenticationContextClassReference](../resources/authenticationContextClassReference.md)。</span><span class="sxs-lookup"><span data-stu-id="25ef4-105">Create a new [authenticationContextClassReference](../resources/authenticationContextClassReference.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="25ef4-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="25ef4-106">Permissions</span></span>

<span data-ttu-id="25ef4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25ef4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25ef4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="25ef4-109">Permission type</span></span>                        | <span data-ttu-id="25ef4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="25ef4-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="25ef4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25ef4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="25ef4-112">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="25ef4-112">Policy.ReadWrite.ConditionalAccess</span></span> |
|<span data-ttu-id="25ef4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25ef4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25ef4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="25ef4-114">Not supported.</span></span> |
|<span data-ttu-id="25ef4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="25ef4-115">Application</span></span>                            | <span data-ttu-id="25ef4-116">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="25ef4-116">Policy.ReadWrite.ConditionalAccess</span></span> |

> [!NOTE]
> <span data-ttu-id="25ef4-117">此 API 有 [一个与](/graph/known-issues#permissions) 权限相关的已知问题。</span><span class="sxs-lookup"><span data-stu-id="25ef4-117">This API has a [known issue](/graph/known-issues#permissions) related to permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="25ef4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25ef4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/conditionalAccess/authenticationContextClassReferences
```

## <a name="request-headers"></a><span data-ttu-id="25ef4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="25ef4-119">Request headers</span></span>

| <span data-ttu-id="25ef4-120">名称</span><span class="sxs-lookup"><span data-stu-id="25ef4-120">Name</span></span>          | <span data-ttu-id="25ef4-121">说明</span><span class="sxs-lookup"><span data-stu-id="25ef4-121">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="25ef4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="25ef4-122">Authorization</span></span> | <span data-ttu-id="25ef4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="25ef4-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="25ef4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="25ef4-125">Content-Type</span></span>  | <span data-ttu-id="25ef4-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="25ef4-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25ef4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="25ef4-128">Request body</span></span>

<span data-ttu-id="25ef4-129">在请求正文中，提供 [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25ef4-129">In the request body, supply a JSON representation of a [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="25ef4-130">响应</span><span class="sxs-lookup"><span data-stu-id="25ef4-130">Response</span></span>

<span data-ttu-id="25ef4-131">如果成功，此方法在响应正文中返回 响应代码和新 `201 Created` [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="25ef4-131">If successful, this method returns a `201 Created` response code and a new [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="25ef4-132">示例</span><span class="sxs-lookup"><span data-stu-id="25ef4-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="25ef4-133">请求</span><span class="sxs-lookup"><span data-stu-id="25ef4-133">Request</span></span>
<span data-ttu-id="25ef4-134">以下示例显示创建可供应用使用的新 authenticationcontextclassreference。</span><span class="sxs-lookup"><span data-stu-id="25ef4-134">The following example shows creating a new authenticationcontextclassreference that is available for apps to use.</span></span>



<!-- {
  "blockType": "request",
  "name": "create_authenticationcontextclassreference"
}-->

```http
POST https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences
Content-type: application/json

{
    "id": "c1",
    "displayName": "Contoso medium",
    "description": "Medium protection level defined for Contoso policy",
    "isAvailable": true
}

```



#### <a name="response"></a><span data-ttu-id="25ef4-135">响应</span><span class="sxs-lookup"><span data-stu-id="25ef4-135">Response</span></span>

<span data-ttu-id="25ef4-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="25ef4-136">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.authenticationContextClassReference"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/authenticationContextClassReference/$entity",
    "id": "c1",
    "displayName": "Contoso medium",
    "description": "Medium protection level defined for Contoso policy",
    "isAvailable": true
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create authenticationContextClassReference",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
