---
title: 创建 certificateBasedAuthConfiguration
description: 使用此 API 创建新的 certificateBasedAuthConfiguration。
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d8b67543ca5a943bfe595c0fd17cd196ad68c82c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047565"
---
# <a name="create-certificatebasedauthconfiguration"></a><span data-ttu-id="df205-103">创建 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="df205-103">Create certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="df205-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df205-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df205-105">创建新的 [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df205-105">Create a new [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="df205-106">只能创建 **certificateBasedAuthConfiguration** 的单个实例 (集合只能有一个成员) 。</span><span class="sxs-lookup"><span data-stu-id="df205-106">Only a single instance of a **certificateBasedAuthConfiguration** can be created (the collection can only have one member).</span></span> <span data-ttu-id="df205-107">它始终具有值为"29728ade-6ae4-4ee9-9103-412912537da5"的固定 ID。</span><span class="sxs-lookup"><span data-stu-id="df205-107">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="df205-108">权限</span><span class="sxs-lookup"><span data-stu-id="df205-108">Permissions</span></span>

<span data-ttu-id="df205-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df205-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="df205-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="df205-111">Permission type</span></span>                        | <span data-ttu-id="df205-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="df205-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="df205-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df205-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="df205-114">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df205-114">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="df205-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df205-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df205-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="df205-116">Not supported.</span></span> |
| <span data-ttu-id="df205-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="df205-117">Application</span></span>    | <span data-ttu-id="df205-118">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df205-118">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="df205-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df205-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="df205-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="df205-120">Request headers</span></span>

| <span data-ttu-id="df205-121">名称</span><span class="sxs-lookup"><span data-stu-id="df205-121">Name</span></span>          | <span data-ttu-id="df205-122">说明</span><span class="sxs-lookup"><span data-stu-id="df205-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="df205-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df205-123">Authorization</span></span> | <span data-ttu-id="df205-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="df205-124">Bearer {token}</span></span> |
| <span data-ttu-id="df205-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="df205-125">Content-Type</span></span> | <span data-ttu-id="df205-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df205-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="df205-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="df205-127">Request body</span></span>

<span data-ttu-id="df205-128">创建 [certificateBasedAuthConfiguration 对象需要以下](../resources/certificatebasedauthconfiguration.md) 属性。</span><span class="sxs-lookup"><span data-stu-id="df205-128">The following properties are required to create the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.</span></span>

| <span data-ttu-id="df205-129">属性</span><span class="sxs-lookup"><span data-stu-id="df205-129">Property</span></span>     | <span data-ttu-id="df205-130">类型</span><span class="sxs-lookup"><span data-stu-id="df205-130">Type</span></span>        | <span data-ttu-id="df205-131">说明</span><span class="sxs-lookup"><span data-stu-id="df205-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="df205-132">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="df205-132">certificateAuthorities</span></span>| <span data-ttu-id="df205-133">[certificateAuthority](../resources/certificateauthority.md) 集合</span><span class="sxs-lookup"><span data-stu-id="df205-133">[certificateAuthority](../resources/certificateauthority.md) collection</span></span> |<span data-ttu-id="df205-134">创建受信任证书链的证书颁发机构的集合。</span><span class="sxs-lookup"><span data-stu-id="df205-134">Collection of certificate authorities that creates a trusted certificate chain.</span></span>  <span data-ttu-id="df205-135">集合的每个成员都必须包含 **证书和** **isRootAuthority** 属性。</span><span class="sxs-lookup"><span data-stu-id="df205-135">Each member of the collection must contain **certificate** and **isRootAuthority** properties.</span></span> |

## <a name="response"></a><span data-ttu-id="df205-136">响应</span><span class="sxs-lookup"><span data-stu-id="df205-136">Response</span></span>

<span data-ttu-id="df205-137">如果成功，此方法在响应正文中返回 响应代码和新 `201 Created` [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df205-137">If successful, this method returns `201 Created` response code and a new [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="df205-138">示例</span><span class="sxs-lookup"><span data-stu-id="df205-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="df205-139">请求</span><span class="sxs-lookup"><span data-stu-id="df205-139">Request</span></span>

<span data-ttu-id="df205-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="df205-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="df205-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="df205-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_certificatebasedauthconfiguration_from_certificatebasedauthconfiguration"
}-->

```http
POST https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration
Content-type: application/json

{
  "certificateAuthorities": [
    {
      "isRootAuthority": true,
      "certificate": "Binary"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="df205-142">C#</span><span class="sxs-lookup"><span data-stu-id="df205-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df205-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df205-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df205-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df205-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df205-145">Java</span><span class="sxs-lookup"><span data-stu-id="df205-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="df205-146">响应</span><span class="sxs-lookup"><span data-stu-id="df205-146">Response</span></span>

<span data-ttu-id="df205-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="df205-147">The following is an example of the response.</span></span>

> <span data-ttu-id="df205-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="df205-148">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "certificateAuthorities": [
    {
      "isRootAuthority": true,
      "certificate": "Binary",
      "issuer": "issuer-value",
      "issuerSki": "issuerSki-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


