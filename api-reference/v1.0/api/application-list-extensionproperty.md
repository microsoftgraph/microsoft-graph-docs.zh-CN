---
title: 列出 extensionProperties
description: 检索 extensionproperty 对象的列表。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3496db47e12786b91579c440501c39d43580918b
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291137"
---
# <a name="list-extensionproperties"></a><span data-ttu-id="b199d-103">列出 extensionProperties</span><span class="sxs-lookup"><span data-stu-id="b199d-103">List extensionProperties</span></span>

<span data-ttu-id="b199d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b199d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b199d-105">检索应用程序上的[extensionProperty](../resources/extensionproperty.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="b199d-105">Retrieve the list of [extensionProperty](../resources/extensionproperty.md) objects on an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="b199d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b199d-106">Permissions</span></span>

<span data-ttu-id="b199d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b199d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b199d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b199d-109">Permission type</span></span>      | <span data-ttu-id="b199d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b199d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b199d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b199d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b199d-112">应用程序。全部，全部读取全部，全部</span><span class="sxs-lookup"><span data-stu-id="b199d-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |
|<span data-ttu-id="b199d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b199d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b199d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b199d-114">Not supported.</span></span>    |
|<span data-ttu-id="b199d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b199d-115">Application</span></span> | <span data-ttu-id="b199d-116">应用程序。全部，全部读取全部，全部</span><span class="sxs-lookup"><span data-stu-id="b199d-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b199d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b199d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/extensionProperties
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b199d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b199d-118">Optional query parameters</span></span>

<span data-ttu-id="b199d-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b199d-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b199d-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="b199d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b199d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b199d-121">Request headers</span></span>

| <span data-ttu-id="b199d-122">名称</span><span class="sxs-lookup"><span data-stu-id="b199d-122">Name</span></span>       | <span data-ttu-id="b199d-123">说明</span><span class="sxs-lookup"><span data-stu-id="b199d-123">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="b199d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b199d-124">Authorization</span></span>  | <span data-ttu-id="b199d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b199d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b199d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b199d-127">Request body</span></span>

<span data-ttu-id="b199d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b199d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b199d-129">响应</span><span class="sxs-lookup"><span data-stu-id="b199d-129">Response</span></span>

<span data-ttu-id="b199d-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[extensionProperty](../resources/extensionproperty.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="b199d-130">If successful, this method returns a `200 OK` response code and a collection of [extensionProperty](../resources/extensionproperty.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b199d-131">示例</span><span class="sxs-lookup"><span data-stu-id="b199d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b199d-132">请求</span><span class="sxs-lookup"><span data-stu-id="b199d-132">Request</span></span>

<span data-ttu-id="b199d-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b199d-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b199d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b199d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_extensionproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/{id}/extensionProperties
```
# <a name="c"></a>[<span data-ttu-id="b199d-135">C#</span><span class="sxs-lookup"><span data-stu-id="b199d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-extensionproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b199d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b199d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-extensionproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b199d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b199d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-extensionproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b199d-138">Java</span><span class="sxs-lookup"><span data-stu-id="b199d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-extensionproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b199d-139">响应</span><span class="sxs-lookup"><span data-stu-id="b199d-139">Response</span></span>

<span data-ttu-id="b199d-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b199d-140">The following is an example of the response.</span></span>

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
