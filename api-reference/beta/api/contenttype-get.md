---
author: swapnil1993
title: 获取 contentType
description: 获取网站或列表中的内容类型。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 70b8ab5db2af4dd391df468dab31adbd26adc13e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446125"
---
# <a name="get-contenttype"></a><span data-ttu-id="7dc4c-103">获取 contentType</span><span class="sxs-lookup"><span data-stu-id="7dc4c-103">Get contentType</span></span>
<span data-ttu-id="7dc4c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dc4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dc4c-105">检索网站或[列表中][contentType]内容[类型的][][元数据][]。</span><span class="sxs-lookup"><span data-stu-id="7dc4c-105">Retrieve the metadata for a [content type][contentType] in a [site][] or a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="7dc4c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7dc4c-106">Permissions</span></span>

<span data-ttu-id="7dc4c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7dc4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dc4c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7dc4c-109">Permission type</span></span>      | <span data-ttu-id="7dc4c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7dc4c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7dc4c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7dc4c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7dc4c-112">Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="7dc4c-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="7dc4c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7dc4c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dc4c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7dc4c-114">Not supported.</span></span>    |
|<span data-ttu-id="7dc4c-115">Application</span><span class="sxs-lookup"><span data-stu-id="7dc4c-115">Application</span></span> | <span data-ttu-id="7dc4c-116">Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="7dc4c-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7dc4c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7dc4c-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /sites/{site-id}/contentTypes/{contentType-id}

GET /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7dc4c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7dc4c-118">Optional query parameters</span></span>
<span data-ttu-id="7dc4c-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7dc4c-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7dc4c-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="7dc4c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7dc4c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7dc4c-121">Request headers</span></span>
|<span data-ttu-id="7dc4c-122">名称</span><span class="sxs-lookup"><span data-stu-id="7dc4c-122">Name</span></span>|<span data-ttu-id="7dc4c-123">说明</span><span class="sxs-lookup"><span data-stu-id="7dc4c-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7dc4c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7dc4c-124">Authorization</span></span>|<span data-ttu-id="7dc4c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7dc4c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dc4c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7dc4c-127">Request body</span></span>
<span data-ttu-id="7dc4c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7dc4c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7dc4c-129">响应</span><span class="sxs-lookup"><span data-stu-id="7dc4c-129">Response</span></span>

<span data-ttu-id="7dc4c-130">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [contentType](../resources/contenttype.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7dc4c-130">If successful, this method returns a `200 OK` response code and a [contentType](../resources/contenttype.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="7dc4c-131">示例</span><span class="sxs-lookup"><span data-stu-id="7dc4c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7dc4c-132">请求</span><span class="sxs-lookup"><span data-stu-id="7dc4c-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contenttype"
}
-->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}
```

### <a name="response"></a><span data-ttu-id="7dc4c-133">响应</span><span class="sxs-lookup"><span data-stu-id="7dc4c-133">Response</span></span>
><span data-ttu-id="7dc4c-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7dc4c-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id":"0x0120D520",
  "description":"Create a document set when you want to manage multiple documents as a single work product.",
  "group":"Document Set Content Types",
  "hidden":false,
  "name":"Document Set",
  "base": {
        "name": "Document Set",
        "id": "0x0120D520"
   }
}
```

[contentType]: ../resources/contentType.md
[网站]: ../resources/site.md
[site]: ../resources/site.md
[列表]: ../resources/list.md
[list]: ../resources/list.md
