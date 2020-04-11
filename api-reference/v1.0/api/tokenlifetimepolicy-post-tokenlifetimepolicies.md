---
title: 创建 tokenLifetimePolicy
description: 创建新的 tokenLifetimePolicy。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f52dd8ebfd4273b7d32f3c64b22d163b83b4fa9b
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229533"
---
# <a name="create-tokenlifetimepolicy"></a><span data-ttu-id="26634-103">创建 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="26634-103">Create tokenLifetimePolicy</span></span>

<span data-ttu-id="26634-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26634-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="26634-105">创建新的[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="26634-105">Create a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="26634-106">权限</span><span class="sxs-lookup"><span data-stu-id="26634-106">Permissions</span></span>

<span data-ttu-id="26634-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26634-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26634-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="26634-109">Permission type</span></span>                        | <span data-ttu-id="26634-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="26634-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="26634-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26634-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="26634-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="26634-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="26634-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26634-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26634-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="26634-114">Not supported.</span></span> |
| <span data-ttu-id="26634-115">Application</span><span class="sxs-lookup"><span data-stu-id="26634-115">Application</span></span>                            | <span data-ttu-id="26634-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="26634-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="26634-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26634-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="26634-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="26634-118">Request headers</span></span>

| <span data-ttu-id="26634-119">名称</span><span class="sxs-lookup"><span data-stu-id="26634-119">Name</span></span>          | <span data-ttu-id="26634-120">说明</span><span class="sxs-lookup"><span data-stu-id="26634-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="26634-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="26634-121">Authorization</span></span> | <span data-ttu-id="26634-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="26634-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="26634-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="26634-124">Content-type</span></span> | <span data-ttu-id="26634-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="26634-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26634-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="26634-127">Request body</span></span>

<span data-ttu-id="26634-128">在请求正文中，提供[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26634-128">In the request body, supply a JSON representation of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="26634-129">响应</span><span class="sxs-lookup"><span data-stu-id="26634-129">Response</span></span>

<span data-ttu-id="26634-130">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="26634-130">If successful, this method returns a `201 Created` response code and a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26634-131">示例</span><span class="sxs-lookup"><span data-stu-id="26634-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26634-132">请求</span><span class="sxs-lookup"><span data-stu-id="26634-132">Request</span></span>

<span data-ttu-id="26634-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="26634-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_tokenlifetimepolicies"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```

### <a name="response"></a><span data-ttu-id="26634-134">响应</span><span class="sxs-lookup"><span data-stu-id="26634-134">Response</span></span>

<span data-ttu-id="26634-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="26634-135">The following is an example of the response.</span></span>

> <span data-ttu-id="26634-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="26634-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
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
  "description": "Create tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
