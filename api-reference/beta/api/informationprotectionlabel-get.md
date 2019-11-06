---
title: 获取 informationProtectionLabel
description: 检索指定的 informationProtectionLabel 对象的属性和关系。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2e4f2025d899cd5f6686eb6a3800d15ac8bf8526
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37995645"
---
# <a name="get-informationprotectionlabel"></a><span data-ttu-id="f2149-103">获取 informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="f2149-103">Get informationProtectionLabel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2149-104">检索[informationProtectionLabel](../resources/informationprotectionlabel.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f2149-104">Retrieve the properties and relationships of an [informationProtectionLabel](../resources/informationprotectionlabel.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2149-105">权限</span><span class="sxs-lookup"><span data-stu-id="f2149-105">Permissions</span></span>

<span data-ttu-id="f2149-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2149-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f2149-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2149-108">Permission type</span></span>                        | <span data-ttu-id="f2149-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2149-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f2149-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2149-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2149-111">InformationProtectionPolicy。请阅读</span><span class="sxs-lookup"><span data-stu-id="f2149-111">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="f2149-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2149-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2149-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2149-113">Not supported.</span></span>                              |
| <span data-ttu-id="f2149-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2149-114">Application</span></span>                            | <span data-ttu-id="f2149-115">InformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="f2149-115">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="f2149-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2149-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /informationprotection/policy/labels/{id}
GET /informationprotection/policy/labels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2149-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f2149-117">Optional query parameters</span></span>

<span data-ttu-id="f2149-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f2149-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f2149-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f2149-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2149-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2149-120">Request headers</span></span>

| <span data-ttu-id="f2149-121">名称</span><span class="sxs-lookup"><span data-stu-id="f2149-121">Name</span></span>          | <span data-ttu-id="f2149-122">说明</span><span class="sxs-lookup"><span data-stu-id="f2149-122">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="f2149-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2149-123">Authorization</span></span> | <span data-ttu-id="f2149-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2149-p103">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="f2149-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2149-126">Request body</span></span>

<span data-ttu-id="f2149-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f2149-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2149-128">响应</span><span class="sxs-lookup"><span data-stu-id="f2149-128">Response</span></span>

<span data-ttu-id="f2149-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[informationProtectionLabel](../resources/informationprotectionlabel.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f2149-129">If successful, this method returns a `200 OK` response code and the requested [informationProtectionLabel](../resources/informationprotectionlabel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f2149-130">示例</span><span class="sxs-lookup"><span data-stu-id="f2149-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2149-131">请求</span><span class="sxs-lookup"><span data-stu-id="f2149-131">Request</span></span>

<span data-ttu-id="f2149-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f2149-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f2149-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2149-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_informationprotectionlabel"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/informationprotection/policy/labels/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f2149-134">C#</span><span class="sxs-lookup"><span data-stu-id="f2149-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-informationprotectionlabel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f2149-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2149-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-informationprotectionlabel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f2149-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2149-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-informationprotectionlabel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f2149-137">响应</span><span class="sxs-lookup"><span data-stu-id="f2149-137">Response</span></span>

<span data-ttu-id="f2149-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f2149-138">The following is an example of the response.</span></span>

> <span data-ttu-id="f2149-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f2149-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationProtectionLabel"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('1e36d926-d716-4197-ba86-a6e18eb910b9')/informationProtection/policy/labels/$entity",
    "id": "4662f9a3-dd50-4a20-b984-a7be82e0e79c",
    "name": "LabelWithFooterAndHeaderActions_Tests",
    "description": "",
    "color": "",
    "sensitivity": 12,
    "tooltip": "LabelWithFooterAndHeaderActions_Tests",
    "isActive": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get informationProtectionLabel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
