---
title: 列出 userFlows
description: 检索 userFlow 对象的列表。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 32957546d058d9f7b6aafabd6d635de067266be4
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734537"
---
# <a name="list-userflows"></a><span data-ttu-id="5d7e4-103">列出 userFlows</span><span class="sxs-lookup"><span data-stu-id="5d7e4-103">List userFlows</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d7e4-104">检索[userflows](../resources/identityuserflow.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="5d7e4-104">Retrieve a list of [userflows](../resources/identityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5d7e4-105">权限</span><span class="sxs-lookup"><span data-stu-id="5d7e4-105">Permissions</span></span>

<span data-ttu-id="5d7e4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5d7e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5d7e4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d7e4-108">Permission type</span></span>                        | <span data-ttu-id="5d7e4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5d7e4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5d7e4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d7e4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5d7e4-111">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="5d7e4-111">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>  |
| <span data-ttu-id="5d7e4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d7e4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d7e4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d7e4-113">Not supported.</span></span> |
| <span data-ttu-id="5d7e4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d7e4-114">Application</span></span>                            | <span data-ttu-id="5d7e4-115">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="5d7e4-115">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d7e4-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d7e4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlows
```

## <a name="request-headers"></a><span data-ttu-id="5d7e4-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d7e4-117">Request headers</span></span>

| <span data-ttu-id="5d7e4-118">名称</span><span class="sxs-lookup"><span data-stu-id="5d7e4-118">Name</span></span>      |<span data-ttu-id="5d7e4-119">说明</span><span class="sxs-lookup"><span data-stu-id="5d7e4-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5d7e4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d7e4-120">Authorization</span></span> | <span data-ttu-id="5d7e4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5d7e4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d7e4-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d7e4-123">Request body</span></span>

<span data-ttu-id="5d7e4-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5d7e4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d7e4-125">响应</span><span class="sxs-lookup"><span data-stu-id="5d7e4-125">Response</span></span>

<span data-ttu-id="5d7e4-126">如果成功，此方法在响应`200 OK`正文中返回响应代码和[userFlow](../resources/identityuserflow.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="5d7e4-126">If successful, this method returns a `200 OK` response code and a collection of [userFlow](../resources/identityuserflow.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5d7e4-127">示例</span><span class="sxs-lookup"><span data-stu-id="5d7e4-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5d7e4-128">请求</span><span class="sxs-lookup"><span data-stu-id="5d7e4-128">Request</span></span>

<span data-ttu-id="5d7e4-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5d7e4-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_userflows"
}-->

```http
GET https://graph.microsoft.com/beta/identity/userFlows
```

### <a name="response"></a><span data-ttu-id="5d7e4-130">响应</span><span class="sxs-lookup"><span data-stu-id="5d7e4-130">Response</span></span>

<span data-ttu-id="5d7e4-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5d7e4-131">The following is an example of the response.</span></span>

> <span data-ttu-id="5d7e4-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5d7e4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.UserFlow",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "B2C_1_UserFlow1",
      "userFlowType": "signUpOrSignIn",
      "userFlowTypeVersion": 1
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List userFlows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_userflows/container/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->