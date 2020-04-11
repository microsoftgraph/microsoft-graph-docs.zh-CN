---
title: 创建 tokenIssuancePolicy
description: 创建新的 tokenIssuancePolicy。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bd008f78f2fc4f4faacf0ffd62589bb7032bd2a7
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229666"
---
# <a name="create-tokenissuancepolicy"></a><span data-ttu-id="f88aa-103">创建 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="f88aa-103">Create tokenIssuancePolicy</span></span>

<span data-ttu-id="f88aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f88aa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f88aa-105">创建新的[tokenIssuancePolicy](../resources/tokenissuancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f88aa-105">Create a new [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f88aa-106">权限</span><span class="sxs-lookup"><span data-stu-id="f88aa-106">Permissions</span></span>

<span data-ttu-id="f88aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f88aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f88aa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f88aa-109">Permission type</span></span>                        | <span data-ttu-id="f88aa-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f88aa-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f88aa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f88aa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f88aa-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f88aa-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="f88aa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f88aa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f88aa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f88aa-114">Not supported.</span></span> |
| <span data-ttu-id="f88aa-115">Application</span><span class="sxs-lookup"><span data-stu-id="f88aa-115">Application</span></span>                            | <span data-ttu-id="f88aa-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f88aa-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="f88aa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f88aa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/tokenIssuancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="f88aa-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f88aa-118">Request headers</span></span>

| <span data-ttu-id="f88aa-119">名称</span><span class="sxs-lookup"><span data-stu-id="f88aa-119">Name</span></span>          | <span data-ttu-id="f88aa-120">说明</span><span class="sxs-lookup"><span data-stu-id="f88aa-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f88aa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f88aa-121">Authorization</span></span> | <span data-ttu-id="f88aa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f88aa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f88aa-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="f88aa-124">Content-type</span></span> | <span data-ttu-id="f88aa-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f88aa-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f88aa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f88aa-127">Request body</span></span>

<span data-ttu-id="f88aa-128">在请求正文中，提供[tokenIssuancePolicy](../resources/tokenissuancepolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f88aa-128">In the request body, supply a JSON representation of a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f88aa-129">响应</span><span class="sxs-lookup"><span data-stu-id="f88aa-129">Response</span></span>

<span data-ttu-id="f88aa-130">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[tokenIssuancePolicy](../resources/tokenissuancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f88aa-130">If successful, this method returns a `201 Created` response code and a new [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f88aa-131">示例</span><span class="sxs-lookup"><span data-stu-id="f88aa-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f88aa-132">请求</span><span class="sxs-lookup"><span data-stu-id="f88aa-132">Request</span></span>

<span data-ttu-id="f88aa-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f88aa-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_tokenIssuancePolicies_from_tokenIssuancePolicies"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```

### <a name="response"></a><span data-ttu-id="f88aa-134">响应</span><span class="sxs-lookup"><span data-stu-id="f88aa-134">Response</span></span>

<span data-ttu-id="f88aa-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f88aa-135">The following is an example of the response.</span></span>

> <span data-ttu-id="f88aa-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f88aa-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
