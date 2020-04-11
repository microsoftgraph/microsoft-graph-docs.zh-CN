---
title: 列表已分配 tokenLifetimePolicies
description: 列出分配给应用程序的 tokenLifetimePolicies。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c26574d4720765c292f0bb606e57a7c07927b03f
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229113"
---
# <a name="list-assigned-tokenlifetimepolicy"></a><span data-ttu-id="adace-103">列表已分配 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="adace-103">List assigned tokenLifetimePolicy</span></span>

<span data-ttu-id="adace-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adace-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="adace-105">列出分配给[应用程序](../resources/application.md)的[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="adace-105">List the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects that are assigned to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="adace-106">权限</span><span class="sxs-lookup"><span data-stu-id="adace-106">Permissions</span></span>

<span data-ttu-id="adace-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="adace-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="adace-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="adace-109">Permission type</span></span>                        | <span data-ttu-id="adace-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="adace-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="adace-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="adace-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="adace-112">Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="adace-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="adace-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="adace-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adace-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="adace-114">Not supported.</span></span> |
| <span data-ttu-id="adace-115">Application</span><span class="sxs-lookup"><span data-stu-id="adace-115">Application</span></span>                            | <span data-ttu-id="adace-116">Policy. All 和 Application.readwrite.ownedby、Application.readwrite.ownedby、ApplicationConfiguration 和、、ApplicationConfiguration 和应用程序的、、和和的所有应用程序中的</span><span class="sxs-lookup"><span data-stu-id="adace-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="adace-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="adace-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="adace-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="adace-118">Request headers</span></span>

| <span data-ttu-id="adace-119">名称</span><span class="sxs-lookup"><span data-stu-id="adace-119">Name</span></span>          | <span data-ttu-id="adace-120">说明</span><span class="sxs-lookup"><span data-stu-id="adace-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="adace-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="adace-121">Authorization</span></span> | <span data-ttu-id="adace-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="adace-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="adace-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="adace-124">Request body</span></span>

<span data-ttu-id="adace-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="adace-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adace-126">响应</span><span class="sxs-lookup"><span data-stu-id="adace-126">Response</span></span>

<span data-ttu-id="adace-127">如果成功，此方法在响应`200 OK`正文中返回响应代码和[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="adace-127">If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="adace-128">示例</span><span class="sxs-lookup"><span data-stu-id="adace-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="adace-129">请求</span><span class="sxs-lookup"><span data-stu-id="adace-129">Request</span></span>

<span data-ttu-id="adace-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="adace-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_tokenlifetimepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/{id}/tokenLifetimePolicies
```

### <a name="response"></a><span data-ttu-id="adace-131">响应</span><span class="sxs-lookup"><span data-stu-id="adace-131">Response</span></span>

<span data-ttu-id="adace-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="adace-132">The following is an example of the response.</span></span>

> <span data-ttu-id="adace-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="adace-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List assigned tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
