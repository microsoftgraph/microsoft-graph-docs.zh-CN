---
title: 创建 certificateBasedAuthConfiguration
description: 使用此 API 创建新的 certificateBasedAuthConfiguration。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cc1c4462c3c0ae63a46b4f78c7487a7ccbe364ca
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2019
ms.locfileid: "37632576"
---
# <a name="create-certificatebasedauthconfiguration"></a><span data-ttu-id="6f61f-103">创建 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="6f61f-103">Create certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="6f61f-104">创建新的[certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6f61f-104">Create a new [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="6f61f-105">仅可创建**certificateBasedAuthConfiguration**的单个实例（集合只能有一个成员）。</span><span class="sxs-lookup"><span data-stu-id="6f61f-105">Only a single instance of a **certificateBasedAuthConfiguration** can be created (the collection can only have one member).</span></span> <span data-ttu-id="6f61f-106">它始终具有值为 "29728ade-6ae4-4ee9-9103-412912537da5" 的固定 ID。</span><span class="sxs-lookup"><span data-stu-id="6f61f-106">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f61f-107">权限</span><span class="sxs-lookup"><span data-stu-id="6f61f-107">Permissions</span></span>

<span data-ttu-id="6f61f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6f61f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6f61f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f61f-110">Permission type</span></span>                        | <span data-ttu-id="6f61f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6f61f-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6f61f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f61f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6f61f-113">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f61f-113">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="6f61f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f61f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f61f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f61f-115">Not supported.</span></span> |
| <span data-ttu-id="6f61f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f61f-116">Application</span></span>    | <span data-ttu-id="6f61f-117">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f61f-117">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f61f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f61f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="6f61f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f61f-119">Request headers</span></span>

| <span data-ttu-id="6f61f-120">名称</span><span class="sxs-lookup"><span data-stu-id="6f61f-120">Name</span></span>          | <span data-ttu-id="6f61f-121">说明</span><span class="sxs-lookup"><span data-stu-id="6f61f-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6f61f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f61f-122">Authorization</span></span> | <span data-ttu-id="6f61f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6f61f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6f61f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6f61f-125">Content-Type</span></span> | <span data-ttu-id="6f61f-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6f61f-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f61f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f61f-128">Request body</span></span>

<span data-ttu-id="6f61f-129">创建[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md)对象需要以下属性。</span><span class="sxs-lookup"><span data-stu-id="6f61f-129">The following properties are required to create the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.</span></span>

| <span data-ttu-id="6f61f-130">属性</span><span class="sxs-lookup"><span data-stu-id="6f61f-130">Property</span></span>     | <span data-ttu-id="6f61f-131">类型</span><span class="sxs-lookup"><span data-stu-id="6f61f-131">Type</span></span>        | <span data-ttu-id="6f61f-132">说明</span><span class="sxs-lookup"><span data-stu-id="6f61f-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6f61f-133">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="6f61f-133">certificateAuthorities</span></span>| <span data-ttu-id="6f61f-134">[certificateAuthority](../resources/certificateauthority.md)集合</span><span class="sxs-lookup"><span data-stu-id="6f61f-134">[certificateAuthority](../resources/certificateauthority.md) collection</span></span> |<span data-ttu-id="6f61f-135">创建受信任的证书链的证书颁发机构的集合。</span><span class="sxs-lookup"><span data-stu-id="6f61f-135">Collection of certificate authorities that creates a trusted certificate chain.</span></span>  <span data-ttu-id="6f61f-136">集合中的每个成员都必须包含**certificate**和**isRootAuthority**属性。</span><span class="sxs-lookup"><span data-stu-id="6f61f-136">Each member of the collection must contain **certificate** and **isRootAuthority** properties.</span></span> |

## <a name="response"></a><span data-ttu-id="6f61f-137">响应</span><span class="sxs-lookup"><span data-stu-id="6f61f-137">Response</span></span>

<span data-ttu-id="6f61f-138">如果成功，此方法在`201 Created`响应正文中返回响应代码和新的[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6f61f-138">If successful, this method returns `201 Created` response code and a new [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6f61f-139">示例</span><span class="sxs-lookup"><span data-stu-id="6f61f-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6f61f-140">请求</span><span class="sxs-lookup"><span data-stu-id="6f61f-140">Request</span></span>

<span data-ttu-id="6f61f-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6f61f-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6f61f-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f61f-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_certificatebasedauthconfiguration_from_certificatebasedauthconfiguration"
}-->

```http
POST https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6f61f-143">C#</span><span class="sxs-lookup"><span data-stu-id="6f61f-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6f61f-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f61f-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6f61f-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f61f-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6f61f-146">Java</span><span class="sxs-lookup"><span data-stu-id="6f61f-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a><span data-ttu-id="6f61f-147">响应</span><span class="sxs-lookup"><span data-stu-id="6f61f-147">Response</span></span>

<span data-ttu-id="6f61f-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6f61f-148">The following is an example of the response.</span></span>

> <span data-ttu-id="6f61f-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6f61f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
