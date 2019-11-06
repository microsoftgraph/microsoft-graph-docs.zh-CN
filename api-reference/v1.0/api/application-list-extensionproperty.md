---
title: 列出 extensionProperties
description: 检索 extensionproperty 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a6f48b9bce911cde13620c90a906e80500184f33
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37999144"
---
# <a name="list-extensionproperties"></a><span data-ttu-id="5f6d7-103">列出 extensionProperties</span><span class="sxs-lookup"><span data-stu-id="5f6d7-103">List extensionProperties</span></span>

<span data-ttu-id="5f6d7-104">检索应用程序上的[extensionProperty](../resources/extensionproperty.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="5f6d7-104">Retrieve the list of [extensionProperty](../resources/extensionproperty.md) objects on an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f6d7-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="5f6d7-105">Permissions</span></span>

<span data-ttu-id="5f6d7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5f6d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f6d7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f6d7-108">Permission type</span></span>      | <span data-ttu-id="5f6d7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5f6d7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f6d7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f6d7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5f6d7-111">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5f6d7-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5f6d7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f6d7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f6d7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f6d7-113">Not supported.</span></span>    |
|<span data-ttu-id="5f6d7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f6d7-114">Application</span></span> | <span data-ttu-id="5f6d7-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f6d7-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f6d7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f6d7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/extensionProperties
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f6d7-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5f6d7-117">Optional query parameters</span></span>

<span data-ttu-id="5f6d7-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5f6d7-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5f6d7-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="5f6d7-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f6d7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f6d7-120">Request headers</span></span>

| <span data-ttu-id="5f6d7-121">名称</span><span class="sxs-lookup"><span data-stu-id="5f6d7-121">Name</span></span>       | <span data-ttu-id="5f6d7-122">说明</span><span class="sxs-lookup"><span data-stu-id="5f6d7-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="5f6d7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f6d7-123">Authorization</span></span>  | <span data-ttu-id="5f6d7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5f6d7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5f6d7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f6d7-126">Request body</span></span>

<span data-ttu-id="5f6d7-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5f6d7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f6d7-128">响应</span><span class="sxs-lookup"><span data-stu-id="5f6d7-128">Response</span></span>

<span data-ttu-id="5f6d7-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[extensionProperty](../resources/extensionproperty.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="5f6d7-129">If successful, this method returns a `200 OK` response code and a collection of [extensionProperty](../resources/extensionproperty.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5f6d7-130">示例</span><span class="sxs-lookup"><span data-stu-id="5f6d7-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5f6d7-131">请求</span><span class="sxs-lookup"><span data-stu-id="5f6d7-131">Request</span></span>

<span data-ttu-id="5f6d7-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5f6d7-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5f6d7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f6d7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_extensionproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/{id}/extensionProperties
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5f6d7-134">C#</span><span class="sxs-lookup"><span data-stu-id="5f6d7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-extensionproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5f6d7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f6d7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-extensionproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5f6d7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f6d7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-extensionproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5f6d7-137">Java</span><span class="sxs-lookup"><span data-stu-id="5f6d7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-extensionproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5f6d7-138">响应</span><span class="sxs-lookup"><span data-stu-id="5f6d7-138">Response</span></span>

<span data-ttu-id="5f6d7-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5f6d7-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.extensionProperty",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "a2c459db-f5dc-4328-ae9b-118e88d04d19",
            "deletedDateTime": null,
            "appDisplayName": "Display name",
            "name": "extension_b3efaf8f68a44275abcff28ef86b2ee3_extensionName",
            "dataType": "String",
            "isSyncedFromOnPremises": false,
            "targetObjects": [
                "Application"
            ]
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List extensionProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
