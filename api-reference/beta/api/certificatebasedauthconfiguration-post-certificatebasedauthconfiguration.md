---
title: 创建 certificateBasedAuthConfiguration
description: 使用此 API 创建新的 certificateBasedAuthConfiguration。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cc78cd5a2de6a8ce1b44dd346c6c19ad8741736f
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667619"
---
# <a name="create-certificatebasedauthconfiguration"></a><span data-ttu-id="9668a-103">创建 certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="9668a-103">Create certificateBasedAuthConfiguration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9668a-104">创建新的[certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9668a-104">Create a new [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="9668a-105">仅可创建**certificateBasedAuthConfiguration**的单个实例 (集合只能有一个成员)。</span><span class="sxs-lookup"><span data-stu-id="9668a-105">Only a single instance of a **certificateBasedAuthConfiguration** can be created (the collection can only have one member).</span></span> <span data-ttu-id="9668a-106">它始终具有值为 "29728ade-6ae4-4ee9-9103-412912537da5" 的固定 ID。</span><span class="sxs-lookup"><span data-stu-id="9668a-106">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="9668a-107">权限</span><span class="sxs-lookup"><span data-stu-id="9668a-107">Permissions</span></span>

<span data-ttu-id="9668a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9668a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9668a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9668a-110">Permission type</span></span>                        | <span data-ttu-id="9668a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9668a-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9668a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9668a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9668a-113">组织关系。 All</span><span class="sxs-lookup"><span data-stu-id="9668a-113">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="9668a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9668a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9668a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9668a-115">Not supported.</span></span> |
| <span data-ttu-id="9668a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9668a-116">Application</span></span>    | <span data-ttu-id="9668a-117">组织关系。 All</span><span class="sxs-lookup"><span data-stu-id="9668a-117">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9668a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9668a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="9668a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9668a-119">Request headers</span></span>

| <span data-ttu-id="9668a-120">名称</span><span class="sxs-lookup"><span data-stu-id="9668a-120">Name</span></span>          | <span data-ttu-id="9668a-121">说明</span><span class="sxs-lookup"><span data-stu-id="9668a-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9668a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9668a-122">Authorization</span></span> | <span data-ttu-id="9668a-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="9668a-123">Bearer {token}</span></span> |
| <span data-ttu-id="9668a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9668a-124">Content-Type</span></span> | <span data-ttu-id="9668a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9668a-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9668a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9668a-126">Request body</span></span>

<span data-ttu-id="9668a-127">创建[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md)对象需要以下属性。</span><span class="sxs-lookup"><span data-stu-id="9668a-127">The following properties are required to create the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.</span></span>

| <span data-ttu-id="9668a-128">属性</span><span class="sxs-lookup"><span data-stu-id="9668a-128">Property</span></span>     | <span data-ttu-id="9668a-129">类型</span><span class="sxs-lookup"><span data-stu-id="9668a-129">Type</span></span>        | <span data-ttu-id="9668a-130">说明</span><span class="sxs-lookup"><span data-stu-id="9668a-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9668a-131">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="9668a-131">certificateAuthorities</span></span>| <span data-ttu-id="9668a-132">[certificateAuthority](../resources/certificateauthority.md)集合</span><span class="sxs-lookup"><span data-stu-id="9668a-132">[certificateAuthority](../resources/certificateauthority.md) collection</span></span> |<span data-ttu-id="9668a-133">创建受信任的证书链的证书颁发机构的集合。</span><span class="sxs-lookup"><span data-stu-id="9668a-133">Collection of certificate authorities that creates a trusted certificate chain.</span></span>  <span data-ttu-id="9668a-134">集合中的每个成员都必须包含**certificate**和**isRootAuthority**属性。</span><span class="sxs-lookup"><span data-stu-id="9668a-134">Each member of the collection must contain **certificate** and **isRootAuthority** properties.</span></span> |

## <a name="response"></a><span data-ttu-id="9668a-135">响应</span><span class="sxs-lookup"><span data-stu-id="9668a-135">Response</span></span>

<span data-ttu-id="9668a-136">如果成功, 此方法在`201 Created`响应正文中返回响应代码和新的[certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9668a-136">If successful, this method returns `201 Created` response code and a new [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9668a-137">示例</span><span class="sxs-lookup"><span data-stu-id="9668a-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9668a-138">请求</span><span class="sxs-lookup"><span data-stu-id="9668a-138">Request</span></span>

<span data-ttu-id="9668a-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9668a-139">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9668a-140">响应</span><span class="sxs-lookup"><span data-stu-id="9668a-140">Response</span></span>

<span data-ttu-id="9668a-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9668a-141">The following is an example of the response.</span></span>

> <span data-ttu-id="9668a-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9668a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
