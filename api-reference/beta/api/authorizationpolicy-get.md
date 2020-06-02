---
title: 获取 authorizationPolicy
description: 检索 authorizationPolicy 对象的属性和关系。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 04a13bba8d434465a65598ec490d96fb8d3c4916
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492203"
---
# <a name="get-authorizationpolicy"></a><span data-ttu-id="1ef07-103">获取 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="1ef07-103">Get authorizationPolicy</span></span>

<span data-ttu-id="1ef07-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ef07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ef07-105">检索[authorizationPolicy](../resources/authorizationpolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1ef07-105">Retrieve the properties of an [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ef07-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="1ef07-106">Permissions</span></span>

<span data-ttu-id="1ef07-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ef07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1ef07-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ef07-109">Permission type</span></span>                        | <span data-ttu-id="1ef07-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ef07-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1ef07-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ef07-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1ef07-112">Policy： Read. All，Policy. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ef07-112">Policy.Read.All, Policy.ReadWrite.Authorization</span></span> |
| <span data-ttu-id="1ef07-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ef07-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ef07-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ef07-114">Not supported.</span></span> |
| <span data-ttu-id="1ef07-115">Application</span><span class="sxs-lookup"><span data-stu-id="1ef07-115">Application</span></span>                            | <span data-ttu-id="1ef07-116">Policy： Read. All，Policy. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ef07-116">Policy.Read.All, Policy.ReadWrite.Authorization</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ef07-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ef07-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="1ef07-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ef07-118">Request headers</span></span>

| <span data-ttu-id="1ef07-119">名称</span><span class="sxs-lookup"><span data-stu-id="1ef07-119">Name</span></span>      |<span data-ttu-id="1ef07-120">说明</span><span class="sxs-lookup"><span data-stu-id="1ef07-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1ef07-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ef07-121">Authorization</span></span> | <span data-ttu-id="1ef07-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1ef07-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ef07-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ef07-124">Request body</span></span>

<span data-ttu-id="1ef07-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1ef07-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ef07-126">响应</span><span class="sxs-lookup"><span data-stu-id="1ef07-126">Response</span></span>

<span data-ttu-id="1ef07-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和单个[authorizationPolicy](../resources/authorizationpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1ef07-127">If successful, this method returns a `200 OK` response code and the single [authorizationPolicy](../resources/authorizationpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1ef07-128">示例</span><span class="sxs-lookup"><span data-stu-id="1ef07-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1ef07-129">请求</span><span class="sxs-lookup"><span data-stu-id="1ef07-129">Request</span></span>

<span data-ttu-id="1ef07-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1ef07-130">The following is an example of the request.</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy
```
---

### <a name="response"></a><span data-ttu-id="1ef07-131">响应</span><span class="sxs-lookup"><span data-stu-id="1ef07-131">Response</span></span>

<span data-ttu-id="1ef07-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1ef07-132">The following is an example of the response.</span></span>

> <span data-ttu-id="1ef07-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1ef07-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/authorizationPolicy/$entity",
    "id": "authorizationPolicy",
    "displayName": "Authorization Policy",
    "description": "Used to manage authorization related settings across the company.",
    "enabledPreviewFeatures": [],
    "guestUserRoleId": "10dae51f-b6af-4016-8d66-8c2a99b929b3",
    "blockMsolPowerShell": ""
}
```
