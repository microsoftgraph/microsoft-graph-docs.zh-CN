---
author: swapnil1993
title: 列出列表中的 contentTypes
description: 列出列表中的内容类型
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: ff6ecd580a654c9b9bff6005317b586f9bf105d9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965048"
---
# <a name="list-contenttypes-in-a-list"></a><span data-ttu-id="32069-103">列出列表中的 contentTypes</span><span class="sxs-lookup"><span data-stu-id="32069-103">List contentTypes in a list</span></span>
<span data-ttu-id="32069-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32069-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="32069-105">获取列表中的 [contentType][contentType] 资源 [的集合][]。</span><span class="sxs-lookup"><span data-stu-id="32069-105">Get the collection of [contentType][contentType] resources in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="32069-106">权限</span><span class="sxs-lookup"><span data-stu-id="32069-106">Permissions</span></span>

<span data-ttu-id="32069-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="32069-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="32069-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="32069-109">Permission type</span></span>      | <span data-ttu-id="32069-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="32069-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32069-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32069-111">Delegated (work or school account)</span></span> | <span data-ttu-id="32069-112">Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="32069-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="32069-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32069-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32069-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="32069-114">Not supported.</span></span>    |
|<span data-ttu-id="32069-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="32069-115">Application</span></span> | <span data-ttu-id="32069-116">Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="32069-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="32069-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32069-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /sites/{site-id}/lists/{list-id}/contentTypes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="32069-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="32069-118">Optional query parameters</span></span>

<span data-ttu-id="32069-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="32069-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="32069-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="32069-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="32069-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="32069-121">Request headers</span></span>
|<span data-ttu-id="32069-122">名称</span><span class="sxs-lookup"><span data-stu-id="32069-122">Name</span></span>|<span data-ttu-id="32069-123">说明</span><span class="sxs-lookup"><span data-stu-id="32069-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="32069-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="32069-124">Authorization</span></span>|<span data-ttu-id="32069-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="32069-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="32069-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="32069-127">Request body</span></span>
<span data-ttu-id="32069-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="32069-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32069-129">响应</span><span class="sxs-lookup"><span data-stu-id="32069-129">Response</span></span>

<span data-ttu-id="32069-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [contentType](../resources/contenttype.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="32069-130">If successful, this method returns a `200 OK` response code and a collection of [contentType](../resources/contenttype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32069-131">示例</span><span class="sxs-lookup"><span data-stu-id="32069-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="32069-132">请求</span><span class="sxs-lookup"><span data-stu-id="32069-132">Request</span></span>

<!-- { "blockType": "request", "name": "enum_contentTypes"} -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/contentTypes
```

### <a name="response"></a><span data-ttu-id="32069-133">响应</span><span class="sxs-lookup"><span data-stu-id="32069-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.contentType)"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
        "id":"0x",
        "description":"",
        "group":"_Hidden",
        "hidden":false,
        "name":"System",
        "base": {
            "name": "System",
            "id": "0x"
        }
    },
    {
        "id":"0x00A7470EADF4194E2E9ED1031B61DA0884",
        "name": "docSet",
        "description": "custom docset",
        "hidden":false,
        "base": {
            "name": "Document Set",
            "id": "0x0120D520"
        },
        "group": "Custom Content Types"
    }
  ]
}
```


[contentType]: ../resources/contentType.md
[列表]: ../resources/list.md
[list]: ../resources/list.md
