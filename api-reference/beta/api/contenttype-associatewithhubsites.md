---
author: swapnil1993
title: contentType：associateWithHubSites
description: 将内容类型与中心网站列表关联。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 89d80568ea0d0099e54d2d912bb7acb32c31f307
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439460"
---
# <a name="contenttype-associatewithhubsites"></a><span data-ttu-id="6fcd4-103">contentType：associateWithHubSites</span><span class="sxs-lookup"><span data-stu-id="6fcd4-103">contentType: associateWithHubSites</span></span>

<span data-ttu-id="6fcd4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fcd4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="6fcd4-105">将 [内容类型][contentType] 与中心网站列表关联。</span><span class="sxs-lookup"><span data-stu-id="6fcd4-105">Associate a [content type][contentType] with a list of hub sites.</span></span>

><span data-ttu-id="6fcd4-106">**注意：** 此功能仅限于拥有许可证的SharePoint Syntex租户。</span><span class="sxs-lookup"><span data-stu-id="6fcd4-106">**Note:** This feature is limited to tenants that have a SharePoint Syntex license.</span></span>
  

## <a name="permissions"></a><span data-ttu-id="6fcd4-107">权限</span><span class="sxs-lookup"><span data-stu-id="6fcd4-107">Permissions</span></span>  

<span data-ttu-id="6fcd4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6fcd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="6fcd4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6fcd4-110">Permission type</span></span> | <span data-ttu-id="6fcd4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6fcd4-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------
|<span data-ttu-id="6fcd4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6fcd4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6fcd4-113">Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="6fcd4-113">Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="6fcd4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6fcd4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fcd4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6fcd4-115">Not supported.</span></span> |
|<span data-ttu-id="6fcd4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6fcd4-116">Application</span></span> | <span data-ttu-id="6fcd4-117">Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="6fcd4-117">Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="6fcd4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6fcd4-118">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
POST /sites/{siteId}/contentTypes/{contentTypeId}/associateWithHubSites
```

## <a name="request-headers"></a><span data-ttu-id="6fcd4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6fcd4-119">Request headers</span></span>
|<span data-ttu-id="6fcd4-120">名称</span><span class="sxs-lookup"><span data-stu-id="6fcd4-120">Name</span></span>|<span data-ttu-id="6fcd4-121">说明</span><span class="sxs-lookup"><span data-stu-id="6fcd4-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6fcd4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fcd4-122">Authorization</span></span>|<span data-ttu-id="6fcd4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6fcd4-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6fcd4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6fcd4-125">Content-Type</span></span>|<span data-ttu-id="6fcd4-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6fcd4-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fcd4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6fcd4-128">Request body</span></span>
<span data-ttu-id="6fcd4-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fcd4-129">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="6fcd4-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="6fcd4-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6fcd4-131">参数</span><span class="sxs-lookup"><span data-stu-id="6fcd4-131">Parameter</span></span>|<span data-ttu-id="6fcd4-132">类型</span><span class="sxs-lookup"><span data-stu-id="6fcd4-132">Type</span></span>|<span data-ttu-id="6fcd4-133">说明</span><span class="sxs-lookup"><span data-stu-id="6fcd4-133">Description</span></span>|
|-|-|-|
|<span data-ttu-id="6fcd4-134">hubSiteUrls</span><span class="sxs-lookup"><span data-stu-id="6fcd4-134">hubSiteUrls</span></span>| <span data-ttu-id="6fcd4-135">集合 (字符串) </span><span class="sxs-lookup"><span data-stu-id="6fcd4-135">Collection(string)</span></span> |<span data-ttu-id="6fcd4-136">需要强制执行内容类型的中心网站的主要 URL 列表。</span><span class="sxs-lookup"><span data-stu-id="6fcd4-136">List of cannonical URLs to the hub sites where the content type needs to be enforced.</span></span> <span data-ttu-id="6fcd4-137">必需项。</span><span class="sxs-lookup"><span data-stu-id="6fcd4-137">Required.</span></span>|
|<span data-ttu-id="6fcd4-138">propagateToExistingLists</span><span class="sxs-lookup"><span data-stu-id="6fcd4-138">propagateToExistingLists</span></span>| <span data-ttu-id="6fcd4-139">布尔</span><span class="sxs-lookup"><span data-stu-id="6fcd4-139">Boolean</span></span> |<span data-ttu-id="6fcd4-140">如果为 ，内容类型将强制应用于中心网站中的现有列表;否则，将 `true` 仅应用于新创建的列表。</span><span class="sxs-lookup"><span data-stu-id="6fcd4-140">If `true`, content types will be enforced on existing lists in the hub sites; otherwise, it will be applied only to newly created lists.</span></span> 

## <a name="response"></a><span data-ttu-id="6fcd4-141">响应</span><span class="sxs-lookup"><span data-stu-id="6fcd4-141">Response</span></span>

<span data-ttu-id="6fcd4-142">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6fcd4-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6fcd4-143">示例</span><span class="sxs-lookup"><span data-stu-id="6fcd4-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fcd4-144">请求</span><span class="sxs-lookup"><span data-stu-id="6fcd4-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6fcd4-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fcd4-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_associatewithhubsites"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/id/contentTypes/id/associateWithHubSites
Content-Type: application/json

{
   "hubSiteUrls":[
      "https://graph.microsoft.com/beta/sites/id"
   ],
   "propagateToExistingLists":false
}
```
# <a name="c"></a>[<span data-ttu-id="6fcd4-146">C#</span><span class="sxs-lookup"><span data-stu-id="6fcd4-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-associatewithhubsites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6fcd4-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fcd4-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-associatewithhubsites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6fcd4-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6fcd4-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-associatewithhubsites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6fcd4-149">Java</span><span class="sxs-lookup"><span data-stu-id="6fcd4-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-associatewithhubsites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a><span data-ttu-id="6fcd4-150">响应</span><span class="sxs-lookup"><span data-stu-id="6fcd4-150">Response</span></span>


<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

  

[contentType]: ../resources/contentType.md
