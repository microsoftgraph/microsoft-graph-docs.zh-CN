---
title: 列出 accessPackageResources
description: 检索 accesspackageresource 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: be2ad10b946574ca48b93ada1d7833262f127059
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048559"
---
# <a name="list-accesspackageresources"></a><span data-ttu-id="f4669-103">列出 accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="f4669-103">List accessPackageResources</span></span>

<span data-ttu-id="f4669-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4669-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4669-105">在[accessPackageCatalog](../resources/accesspackagecatalog.md)中检索[accessPackageResource](../resources/accesspackageresource.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="f4669-105">Retrieve a list of [accessPackageResource](../resources/accesspackageresource.md) objects in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>  <span data-ttu-id="f4669-106">若要请求添加或删除 [accessPackageResource](../resources/accesspackageresource.md)，请使用 [create accessPackageResourceRequest](accesspackageresourcerequest-post.md)。</span><span class="sxs-lookup"><span data-stu-id="f4669-106">To request to add or remove an [accessPackageResource](../resources/accesspackageresource.md), use [create accessPackageResourceRequest](accesspackageresourcerequest-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f4669-107">权限</span><span class="sxs-lookup"><span data-stu-id="f4669-107">Permissions</span></span>

<span data-ttu-id="f4669-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4669-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f4669-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4669-110">Permission type</span></span>                        | <span data-ttu-id="f4669-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f4669-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f4669-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4669-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f4669-113">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4669-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="f4669-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4669-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4669-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4669-115">Not supported.</span></span> |
| <span data-ttu-id="f4669-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4669-116">Application</span></span>                            | <span data-ttu-id="f4669-117">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4669-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4669-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4669-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f4669-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f4669-119">Optional query parameters</span></span>

<span data-ttu-id="f4669-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f4669-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f4669-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f4669-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4669-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4669-122">Request headers</span></span>

| <span data-ttu-id="f4669-123">名称</span><span class="sxs-lookup"><span data-stu-id="f4669-123">Name</span></span>      |<span data-ttu-id="f4669-124">说明</span><span class="sxs-lookup"><span data-stu-id="f4669-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f4669-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4669-125">Authorization</span></span> | <span data-ttu-id="f4669-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="f4669-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4669-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4669-128">Request body</span></span>

<span data-ttu-id="f4669-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f4669-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4669-130">响应</span><span class="sxs-lookup"><span data-stu-id="f4669-130">Response</span></span>

<span data-ttu-id="f4669-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessPackageResource](../resources/accesspackageresource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f4669-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResource](../resources/accesspackageresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f4669-132">示例</span><span class="sxs-lookup"><span data-stu-id="f4669-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f4669-133">请求</span><span class="sxs-lookup"><span data-stu-id="f4669-133">Request</span></span>

<span data-ttu-id="f4669-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f4669-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f4669-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4669-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```
# <a name="c"></a>[<span data-ttu-id="f4669-136">C#</span><span class="sxs-lookup"><span data-stu-id="f4669-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4669-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4669-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4669-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4669-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4669-139">Java</span><span class="sxs-lookup"><span data-stu-id="f4669-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f4669-140">响应</span><span class="sxs-lookup"><span data-stu-id="f4669-140">Response</span></span>

<span data-ttu-id="f4669-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f4669-141">The following is an example of the response.</span></span>

> <span data-ttu-id="f4669-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f4669-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "400279ff-8e85-4dcf-b1d6-d3a6be372951",
      "displayName": "Faculty cafeteria ordering",
      "description": "Example application",
      "url": "https://myapps.microsoft.com/example.com/signin/Faculty%20cafeteria%20ordering/f1e3b407-942d-4934-9a3f-cef1975cb988/",
      "resourceType": "Application",
      "originId": "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


