---
title: 'trustFrameworkKeySet: generateKey'
description: 在键集中自动生成密钥和密码。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c32501031d08e1b6d9dfc0fc78909e127a96b900
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734556"
---
# <a name="trustframeworkkeyset-generatekey"></a><span data-ttu-id="20409-103">trustFrameworkKeySet: generateKey</span><span class="sxs-lookup"><span data-stu-id="20409-103">trustFrameworkKeySet: generateKey</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20409-104">在[trustFrameworkKeyset](../resources/trustframeworkkeyset.md)中自动生成[trustFrameworkKey](../resources/trustFrameworkKey.md)和密码。</span><span class="sxs-lookup"><span data-stu-id="20409-104">Generate a [trustFrameworkKey](../resources/trustFrameworkKey.md) and a secret automatically in the [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="20409-105">呼叫者不必提供密码。</span><span class="sxs-lookup"><span data-stu-id="20409-105">The caller doesn't have to provide a secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="20409-106">权限</span><span class="sxs-lookup"><span data-stu-id="20409-106">Permissions</span></span>

<span data-ttu-id="20409-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20409-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="20409-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="20409-109">Permission type</span></span>                        | <span data-ttu-id="20409-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="20409-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="20409-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20409-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="20409-112">TrustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="20409-112">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="20409-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20409-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20409-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="20409-114">Not supported.</span></span> |
| <span data-ttu-id="20409-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="20409-115">Application</span></span>                            | <span data-ttu-id="20409-116">TrustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="20409-116">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20409-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20409-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/generateKey
```

## <a name="request-headers"></a><span data-ttu-id="20409-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="20409-118">Request headers</span></span>

| <span data-ttu-id="20409-119">名称</span><span class="sxs-lookup"><span data-stu-id="20409-119">Name</span></span>          | <span data-ttu-id="20409-120">说明</span><span class="sxs-lookup"><span data-stu-id="20409-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="20409-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="20409-121">Authorization</span></span> | <span data-ttu-id="20409-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="20409-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20409-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="20409-124">Content-type</span></span>  | <span data-ttu-id="20409-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="20409-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20409-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="20409-127">Request body</span></span>

<span data-ttu-id="20409-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="20409-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="20409-129">参数</span><span class="sxs-lookup"><span data-stu-id="20409-129">Parameter</span></span>    | <span data-ttu-id="20409-130">类型</span><span class="sxs-lookup"><span data-stu-id="20409-130">Type</span></span>        | <span data-ttu-id="20409-131">说明</span><span class="sxs-lookup"><span data-stu-id="20409-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="20409-132">改用</span><span class="sxs-lookup"><span data-stu-id="20409-132">use</span></span> | <span data-ttu-id="20409-133">string</span><span class="sxs-lookup"><span data-stu-id="20409-133">string</span></span> | <span data-ttu-id="20409-134">与**trustFrameworkKey**的**use**属性类似。</span><span class="sxs-lookup"><span data-stu-id="20409-134">Similar to the **use** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="20409-135">kty</span><span class="sxs-lookup"><span data-stu-id="20409-135">kty</span></span> | <span data-ttu-id="20409-136">string</span><span class="sxs-lookup"><span data-stu-id="20409-136">string</span></span> | <span data-ttu-id="20409-137">类似于**trustFrameworkKey**的**kty**属性。</span><span class="sxs-lookup"><span data-stu-id="20409-137">Similar to **kty** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="20409-138">nbf</span><span class="sxs-lookup"><span data-stu-id="20409-138">nbf</span></span> | <span data-ttu-id="20409-139">int</span><span class="sxs-lookup"><span data-stu-id="20409-139">int</span></span> | <span data-ttu-id="20409-140">类似于**trustFrameworkKey**的**nbf**属性。</span><span class="sxs-lookup"><span data-stu-id="20409-140">Similar to **nbf** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="20409-141">exp</span><span class="sxs-lookup"><span data-stu-id="20409-141">exp</span></span> | <span data-ttu-id="20409-142">int</span><span class="sxs-lookup"><span data-stu-id="20409-142">int</span></span> | <span data-ttu-id="20409-143">类似于**trustFrameworkKey**的**exp**属性。</span><span class="sxs-lookup"><span data-stu-id="20409-143">Similar to **exp** property of **trustFrameworkKey**.</span></span> |

## <a name="response"></a><span data-ttu-id="20409-144">响应</span><span class="sxs-lookup"><span data-stu-id="20409-144">Response</span></span>

<span data-ttu-id="20409-145">如果成功，此方法在响应`200 OK`正文中返回响应代码和新的[trustFrameworkKey](../resources/trustframeworkkey.md)对象。</span><span class="sxs-lookup"><span data-stu-id="20409-145">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="20409-146">示例</span><span class="sxs-lookup"><span data-stu-id="20409-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="20409-147">请求</span><span class="sxs-lookup"><span data-stu-id="20409-147">Request</span></span>

<span data-ttu-id="20409-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="20409-148">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_generatekey"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/generateKey
Content-type: application/json

{
  "use": "sig",
  "kty": "RSA",
  "nbf": 1508969811,
  "exp": 1508969811
}
```

### <a name="response"></a><span data-ttu-id="20409-149">响应</span><span class="sxs-lookup"><span data-stu-id="20409-149">Response</span></span>

<span data-ttu-id="20409-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="20409-150">The following is an example of the response.</span></span>

> <span data-ttu-id="20409-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="20409-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKey"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.trustFrameworkKey",
    "k": null,
    "x5c": [],
    "kty": "RSA",
    "use": "sig",
    "exp": 1908969811,
    "nbf": 1908969811,
    "kid": "Gaid7K8sO8RavMX9fzHir_Wg0femGhbY9b-B4rVIxbE",
    "e": "AQAB",
    "n": "rd54s6",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: generateKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
