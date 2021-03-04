---
author: swapnil1993
title: contentType：associateWithHubSites
description: 将内容类型与中心网站列表关联。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8049eb6db5975c2e5c8600a654b6cc533124217f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446135"
---
# <a name="contenttype-associatewithhubsites"></a><span data-ttu-id="8a924-103">contentType：associateWithHubSites</span><span class="sxs-lookup"><span data-stu-id="8a924-103">contentType: associateWithHubSites</span></span>

<span data-ttu-id="8a924-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a924-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="8a924-105">将 [内容类型][contentType] 与中心网站列表关联。</span><span class="sxs-lookup"><span data-stu-id="8a924-105">Associate a [content type][contentType] with a list of hub sites.</span></span>

><span data-ttu-id="8a924-106">**注意：** 此功能仅限于拥有 SharePoint Syntex 许可证的租户。</span><span class="sxs-lookup"><span data-stu-id="8a924-106">**Note:** This feature is limited to tenants that have a SharePoint Syntex license.</span></span>
  

## <a name="permissions"></a><span data-ttu-id="8a924-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="8a924-107">Permissions</span></span>  

<span data-ttu-id="8a924-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8a924-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="8a924-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a924-110">Permission type</span></span> | <span data-ttu-id="8a924-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a924-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------
|<span data-ttu-id="8a924-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a924-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8a924-113">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="8a924-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="8a924-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a924-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a924-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a924-115">Not supported.</span></span> |
|<span data-ttu-id="8a924-116">Application</span><span class="sxs-lookup"><span data-stu-id="8a924-116">Application</span></span> | <span data-ttu-id="8a924-117">Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="8a924-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="8a924-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a924-118">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
POST /sites/id/contentTypes/id/associateWithHubSites
```

## <a name="request-headers"></a><span data-ttu-id="8a924-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a924-119">Request headers</span></span>
|<span data-ttu-id="8a924-120">名称</span><span class="sxs-lookup"><span data-stu-id="8a924-120">Name</span></span>|<span data-ttu-id="8a924-121">说明</span><span class="sxs-lookup"><span data-stu-id="8a924-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8a924-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a924-122">Authorization</span></span>|<span data-ttu-id="8a924-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8a924-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8a924-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a924-125">Content-Type</span></span>|<span data-ttu-id="8a924-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8a924-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a924-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a924-128">Request body</span></span>
<span data-ttu-id="8a924-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a924-129">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="8a924-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="8a924-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8a924-131">参数</span><span class="sxs-lookup"><span data-stu-id="8a924-131">Parameter</span></span>|<span data-ttu-id="8a924-132">类型</span><span class="sxs-lookup"><span data-stu-id="8a924-132">Type</span></span>|<span data-ttu-id="8a924-133">说明</span><span class="sxs-lookup"><span data-stu-id="8a924-133">Description</span></span>|
|-|-|-|
|<span data-ttu-id="8a924-134">hubSiteUrls</span><span class="sxs-lookup"><span data-stu-id="8a924-134">hubSiteUrls</span></span>| <span data-ttu-id="8a924-135">集合 (字符串) </span><span class="sxs-lookup"><span data-stu-id="8a924-135">Collection(string)</span></span> |<span data-ttu-id="8a924-136">需要强制执行内容类型的中心网站的主要 URL 列表。</span><span class="sxs-lookup"><span data-stu-id="8a924-136">List of cannonical URLs to the hub sites where the content type needs to be enforced.</span></span> <span data-ttu-id="8a924-137">必需。</span><span class="sxs-lookup"><span data-stu-id="8a924-137">Required.</span></span>|
|<span data-ttu-id="8a924-138">propagateToExistingLists</span><span class="sxs-lookup"><span data-stu-id="8a924-138">propagateToExistingLists</span></span>| <span data-ttu-id="8a924-139">布尔</span><span class="sxs-lookup"><span data-stu-id="8a924-139">Boolean</span></span> |<span data-ttu-id="8a924-140">如果 ，内容类型将在中心网站中的现有列表上强制执行;否则，它将仅应用于 `true` 新创建的列表。</span><span class="sxs-lookup"><span data-stu-id="8a924-140">If `true`, content types will be enforced on existing lists in the hub sites; otherwise, it will be applied only to newly created lists.</span></span> 

## <a name="response"></a><span data-ttu-id="8a924-141">响应</span><span class="sxs-lookup"><span data-stu-id="8a924-141">Response</span></span>

<span data-ttu-id="8a924-142">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8a924-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8a924-143">示例</span><span class="sxs-lookup"><span data-stu-id="8a924-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a924-144">请求</span><span class="sxs-lookup"><span data-stu-id="8a924-144">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "contenttype_associatewithhubsites"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/id/contentTypes/id/associateWithHubSites
Content-Type: application/json

{
  "hubSiteUrls":
    [
      "https://graph.microsoft.com/beta/sites/id"
      
    ],
    "propagateToExistingLists": false
}
```



### <a name="response"></a><span data-ttu-id="8a924-145">响应</span><span class="sxs-lookup"><span data-stu-id="8a924-145">Response</span></span>


<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content

```

  

[contentType]: ../resources/contentType.md
