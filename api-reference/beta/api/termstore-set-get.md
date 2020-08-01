---
title: Get set
description: 读取 set 对象的属性和关系。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 02f61201db78e2c4e2d8a7dbef4bc0776071f1f0
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539206"
---
# <a name="get-set"></a><span data-ttu-id="7bd8b-103">Get set</span><span class="sxs-lookup"><span data-stu-id="7bd8b-103">Get set</span></span>
<span data-ttu-id="7bd8b-104">命名空间： termStore[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="7bd8b-104">Namespace: microsoft.graph.termStore [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="7bd8b-105">读取[set](../resources/termstore-set.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7bd8b-105">Read the properties and relationships of a [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bd8b-106">权限</span><span class="sxs-lookup"><span data-stu-id="7bd8b-106">Permissions</span></span>
<span data-ttu-id="7bd8b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7bd8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bd8b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7bd8b-109">Permission type</span></span>|<span data-ttu-id="7bd8b-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7bd8b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bd8b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7bd8b-111">Delegated (work or school account)</span></span> |<span data-ttu-id="7bd8b-112">TermStore、TermStore 和所有</span><span class="sxs-lookup"><span data-stu-id="7bd8b-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="7bd8b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7bd8b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bd8b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7bd8b-114">Not supported.</span></span>    |
|<span data-ttu-id="7bd8b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7bd8b-115">Application</span></span> | <span data-ttu-id="7bd8b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7bd8b-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="7bd8b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7bd8b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/sets/{setId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7bd8b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7bd8b-118">Optional query parameters</span></span>
<span data-ttu-id="7bd8b-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7bd8b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7bd8b-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="7bd8b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7bd8b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7bd8b-121">Request headers</span></span>
|<span data-ttu-id="7bd8b-122">名称</span><span class="sxs-lookup"><span data-stu-id="7bd8b-122">Name</span></span>|<span data-ttu-id="7bd8b-123">说明</span><span class="sxs-lookup"><span data-stu-id="7bd8b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7bd8b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bd8b-124">Authorization</span></span>|<span data-ttu-id="7bd8b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7bd8b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bd8b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7bd8b-127">Request body</span></span>
<span data-ttu-id="7bd8b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7bd8b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bd8b-129">响应</span><span class="sxs-lookup"><span data-stu-id="7bd8b-129">Response</span></span>

<span data-ttu-id="7bd8b-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[set](../resources/termstore-set.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7bd8b-130">If successful, this method returns a `200 OK` response code and a [set](../resources/termstore-set.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7bd8b-131">示例</span><span class="sxs-lookup"><span data-stu-id="7bd8b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7bd8b-132">请求</span><span class="sxs-lookup"><span data-stu-id="7bd8b-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_set"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/sets/{setId}
```


### <a name="response"></a><span data-ttu-id="7bd8b-133">响应</span><span class="sxs-lookup"><span data-stu-id="7bd8b-133">Response</span></span>
<span data-ttu-id="7bd8b-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7bd8b-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.set"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{

  "createdDateTime": "2019-06-21T20:01:37Z",  
  "description": "Starting term Set",
  "id": "8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f",
  "localizedNames" : [
    {
      "languageTag" : "en-US",
      "name" : "Department"
    }
  ]
}
```

[microsoft.graph.termStore.group]: ../resources/termstore-group.md
[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft.graph.termStore.store]: ../resources/termstore-store.md

<!--
{
  "type": "#page.annotation",
  "description": "Get termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get termSet",
  "suppressions": [
  ]
}
-->
