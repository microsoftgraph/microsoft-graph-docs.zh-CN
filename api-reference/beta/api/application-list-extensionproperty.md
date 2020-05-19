---
title: 列出 extensionProperties
description: 检索 extensionproperty 对象的列表。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4e7a1eed267d98381250fbf3d3bf581e195700b9
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289332"
---
# <a name="list-extensionproperties"></a><span data-ttu-id="85f01-103">列出 extensionProperties</span><span class="sxs-lookup"><span data-stu-id="85f01-103">List extensionProperties</span></span>

<span data-ttu-id="85f01-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85f01-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85f01-105">检索应用程序上的[extensionProperty](../resources/extensionproperty.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="85f01-105">Retrieve the list of [extensionProperty](../resources/extensionproperty.md) objects on an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="85f01-106">权限</span><span class="sxs-lookup"><span data-stu-id="85f01-106">Permissions</span></span>

<span data-ttu-id="85f01-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85f01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85f01-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="85f01-109">Permission type</span></span>      | <span data-ttu-id="85f01-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="85f01-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85f01-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85f01-111">Delegated (work or school account)</span></span> | <span data-ttu-id="85f01-112">"Application"、"all"、"Directory.accessasuser.all"、"全部"、"全部"、"全部"、"全部"、"所有"</span><span class="sxs-lookup"><span data-stu-id="85f01-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="85f01-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85f01-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85f01-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="85f01-114">Not supported.</span></span>    |
|<span data-ttu-id="85f01-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="85f01-115">Application</span></span> | <span data-ttu-id="85f01-116">"Application.readwrite.ownedby"、"全部"、"全部"、"全部"、"全部"、"全部"、"全部"、"全部"、"目录"</span><span class="sxs-lookup"><span data-stu-id="85f01-116">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="85f01-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85f01-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/extensionProperties
```

## <a name="optional-query-parameters"></a><span data-ttu-id="85f01-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="85f01-118">Optional query parameters</span></span>

<span data-ttu-id="85f01-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="85f01-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="85f01-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="85f01-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="85f01-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="85f01-121">Request headers</span></span>

| <span data-ttu-id="85f01-122">名称</span><span class="sxs-lookup"><span data-stu-id="85f01-122">Name</span></span>       | <span data-ttu-id="85f01-123">说明</span><span class="sxs-lookup"><span data-stu-id="85f01-123">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="85f01-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="85f01-124">Authorization</span></span>  | <span data-ttu-id="85f01-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="85f01-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="85f01-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="85f01-127">Request body</span></span>

<span data-ttu-id="85f01-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="85f01-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85f01-129">响应</span><span class="sxs-lookup"><span data-stu-id="85f01-129">Response</span></span>

<span data-ttu-id="85f01-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[extensionProperty](../resources/extensionproperty.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="85f01-130">If successful, this method returns a `200 OK` response code and a collection of [extensionProperty](../resources/extensionproperty.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="85f01-131">示例</span><span class="sxs-lookup"><span data-stu-id="85f01-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="85f01-132">请求</span><span class="sxs-lookup"><span data-stu-id="85f01-132">Request</span></span>

<span data-ttu-id="85f01-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="85f01-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="85f01-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="85f01-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_extensionproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/extensionProperties
```
# <a name="c"></a>[<span data-ttu-id="85f01-135">C#</span><span class="sxs-lookup"><span data-stu-id="85f01-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-extensionproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85f01-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85f01-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-extensionproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85f01-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85f01-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-extensionproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="85f01-138">响应</span><span class="sxs-lookup"><span data-stu-id="85f01-138">Response</span></span>

<span data-ttu-id="85f01-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="85f01-139">The following is an example of the response.</span></span>

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
