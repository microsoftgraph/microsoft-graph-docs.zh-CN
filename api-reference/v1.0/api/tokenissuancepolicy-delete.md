---
title: 删除 tokenIssuancePolicy
description: 删除 tokenIssuancePolicy。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ed3f02e1ff6cb566922282548e0b9fb252f6784b
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229694"
---
# <a name="delete-tokenissuancepolicy"></a><span data-ttu-id="cccbe-103">删除 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="cccbe-103">Delete tokenIssuancePolicy</span></span>

<span data-ttu-id="cccbe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cccbe-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="cccbe-105">删除[tokenIssuancePolicy](../resources/tokenissuancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cccbe-105">Delete a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cccbe-106">权限</span><span class="sxs-lookup"><span data-stu-id="cccbe-106">Permissions</span></span>

<span data-ttu-id="cccbe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cccbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cccbe-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cccbe-109">Permission type</span></span>                        | <span data-ttu-id="cccbe-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cccbe-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cccbe-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cccbe-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cccbe-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="cccbe-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="cccbe-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cccbe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cccbe-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cccbe-114">Not supported.</span></span> |
| <span data-ttu-id="cccbe-115">Application</span><span class="sxs-lookup"><span data-stu-id="cccbe-115">Application</span></span>                            | <span data-ttu-id="cccbe-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="cccbe-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="cccbe-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cccbe-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/tokenIssuancePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cccbe-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cccbe-118">Request headers</span></span>

| <span data-ttu-id="cccbe-119">名称</span><span class="sxs-lookup"><span data-stu-id="cccbe-119">Name</span></span>          | <span data-ttu-id="cccbe-120">说明</span><span class="sxs-lookup"><span data-stu-id="cccbe-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cccbe-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cccbe-121">Authorization</span></span> | <span data-ttu-id="cccbe-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cccbe-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cccbe-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="cccbe-124">Request body</span></span>

<span data-ttu-id="cccbe-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cccbe-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cccbe-126">响应</span><span class="sxs-lookup"><span data-stu-id="cccbe-126">Response</span></span>

<span data-ttu-id="cccbe-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cccbe-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="cccbe-128">示例</span><span class="sxs-lookup"><span data-stu-id="cccbe-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cccbe-129">请求</span><span class="sxs-lookup"><span data-stu-id="cccbe-129">Request</span></span>

<span data-ttu-id="cccbe-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cccbe-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_tokenissuancepolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies/{id}
```

### <a name="response"></a><span data-ttu-id="cccbe-131">响应</span><span class="sxs-lookup"><span data-stu-id="cccbe-131">Response</span></span>

<span data-ttu-id="cccbe-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cccbe-132">The following is an example of the response.</span></span>

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
  "description": "Delete tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
