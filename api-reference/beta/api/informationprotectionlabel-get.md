---
title: 获取 informationProtectionLabel
description: 检索指定的 informationProtectionLabel 对象的属性和关系。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bcd8c6e3d210615dec4d7bf4233256ab2cd5acb6
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938532"
---
# <a name="get-informationprotectionlabel"></a><span data-ttu-id="aad76-103">获取 informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="aad76-103">Get informationProtectionLabel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aad76-104">检索[informationProtectionLabel](../resources/informationprotectionlabel.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aad76-104">Retrieve the properties and relationships of an [informationProtectionLabel](../resources/informationprotectionlabel.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="aad76-105">权限</span><span class="sxs-lookup"><span data-stu-id="aad76-105">Permissions</span></span>

<span data-ttu-id="aad76-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aad76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aad76-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="aad76-108">Permission type</span></span>                        | <span data-ttu-id="aad76-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aad76-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="aad76-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aad76-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="aad76-111">InformationProtectionPolicy。请阅读</span><span class="sxs-lookup"><span data-stu-id="aad76-111">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="aad76-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aad76-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aad76-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="aad76-113">Not supported.</span></span>                              |
| <span data-ttu-id="aad76-114">Application</span><span class="sxs-lookup"><span data-stu-id="aad76-114">Application</span></span>                            | <span data-ttu-id="aad76-115">InformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="aad76-115">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="aad76-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aad76-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /informationprotection/policy/labels/{id}
GET /informationprotection/policy/labels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aad76-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="aad76-117">Optional query parameters</span></span>

<span data-ttu-id="aad76-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="aad76-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="aad76-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="aad76-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="aad76-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="aad76-120">Request headers</span></span>

| <span data-ttu-id="aad76-121">名称</span><span class="sxs-lookup"><span data-stu-id="aad76-121">Name</span></span>          | <span data-ttu-id="aad76-122">说明</span><span class="sxs-lookup"><span data-stu-id="aad76-122">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="aad76-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aad76-123">Authorization</span></span> | <span data-ttu-id="aad76-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aad76-p103">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="aad76-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="aad76-126">Request body</span></span>

<span data-ttu-id="aad76-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aad76-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aad76-128">响应</span><span class="sxs-lookup"><span data-stu-id="aad76-128">Response</span></span>

<span data-ttu-id="aad76-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[informationProtectionLabel](../resources/informationprotectionlabel.md)对象。</span><span class="sxs-lookup"><span data-stu-id="aad76-129">If successful, this method returns a `200 OK` response code and the requested [informationProtectionLabel](../resources/informationprotectionlabel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aad76-130">示例</span><span class="sxs-lookup"><span data-stu-id="aad76-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aad76-131">请求</span><span class="sxs-lookup"><span data-stu-id="aad76-131">Request</span></span>

<span data-ttu-id="aad76-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aad76-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_informationprotectionlabel"
}-->

```http
GET https://graph.microsoft.com/beta/me/informationprotection/policy/labels/{id}
```

### <a name="response"></a><span data-ttu-id="aad76-133">响应</span><span class="sxs-lookup"><span data-stu-id="aad76-133">Response</span></span>

<span data-ttu-id="aad76-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aad76-134">The following is an example of the response.</span></span>

> <span data-ttu-id="aad76-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="aad76-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
