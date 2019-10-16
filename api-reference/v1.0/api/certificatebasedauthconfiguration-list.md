---
title: 列出 certificateBasedAuthConfigurations
description: 获取 certificatebasedauthconfiguration 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a1f284e2cd921b8db3b6e30914f20b14c3da20c2
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539223"
---
# <a name="list-certificatebasedauthconfigurations"></a><span data-ttu-id="4d4e1-103">列出 certificateBasedAuthConfigurations</span><span class="sxs-lookup"><span data-stu-id="4d4e1-103">List certificateBasedAuthConfigurations</span></span>

<span data-ttu-id="4d4e1-104">获取[certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="4d4e1-104">Get a list of [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) objects.</span></span>

> [!NOTE]
> <span data-ttu-id="4d4e1-105">集合中只能存在一个 certificateBasedAuthConfiguration 实例。</span><span class="sxs-lookup"><span data-stu-id="4d4e1-105">Only a single instance of certificateBasedAuthConfiguration can exist in the collection.</span></span> <span data-ttu-id="4d4e1-106">它始终具有值为 "29728ade-6ae4-4ee9-9103-412912537da5" 的固定 ID。</span><span class="sxs-lookup"><span data-stu-id="4d4e1-106">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d4e1-107">权限</span><span class="sxs-lookup"><span data-stu-id="4d4e1-107">Permissions</span></span>

<span data-ttu-id="4d4e1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4d4e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4d4e1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d4e1-110">Permission type</span></span>                        | <span data-ttu-id="4d4e1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4d4e1-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4d4e1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d4e1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4d4e1-113">全部，全部组织。</span><span class="sxs-lookup"><span data-stu-id="4d4e1-113">Organization.Read.All, Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="4d4e1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d4e1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d4e1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d4e1-115">Not supported.</span></span> |
| <span data-ttu-id="4d4e1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d4e1-116">Application</span></span>    | <span data-ttu-id="4d4e1-117">全部，全部组织。</span><span class="sxs-lookup"><span data-stu-id="4d4e1-117">Organization.Read.All, Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d4e1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d4e1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="4d4e1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d4e1-119">Request headers</span></span>

| <span data-ttu-id="4d4e1-120">名称</span><span class="sxs-lookup"><span data-stu-id="4d4e1-120">Name</span></span>      |<span data-ttu-id="4d4e1-121">说明</span><span class="sxs-lookup"><span data-stu-id="4d4e1-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4d4e1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d4e1-122">Authorization</span></span> | <span data-ttu-id="4d4e1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4d4e1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d4e1-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d4e1-125">Request body</span></span>

<span data-ttu-id="4d4e1-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4d4e1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d4e1-127">响应</span><span class="sxs-lookup"><span data-stu-id="4d4e1-127">Response</span></span>

<span data-ttu-id="4d4e1-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="4d4e1-128">If successful, this method returns a `200 OK` response code and a collection of [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4d4e1-129">示例</span><span class="sxs-lookup"><span data-stu-id="4d4e1-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4d4e1-130">请求</span><span class="sxs-lookup"><span data-stu-id="4d4e1-130">Request</span></span>

<span data-ttu-id="4d4e1-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4d4e1-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4d4e1-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d4e1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_certificatebasedauthconfigurations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration
```

---


### <a name="response"></a><span data-ttu-id="4d4e1-133">响应</span><span class="sxs-lookup"><span data-stu-id="4d4e1-133">Response</span></span>

<span data-ttu-id="4d4e1-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4d4e1-134">The following is an example of the response.</span></span>

> <span data-ttu-id="4d4e1-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4d4e1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "certificateAuthorities": [
        {
          "isRootAuthority": true,
          "certificateRevocationListUrl": "CRLUrl-value",
          "deltaCertificateRevocationListUrl": "deltaCRLUrl-value",
          "certificate": "Binary",
          "issuer": "issuer-value",
          "issuerSki": "issuerSki-value"
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
