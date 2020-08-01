---
title: 获取术语
description: 读取术语对象的属性和关系。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: c6530a688b0cbad9a5d4108e49e37d352362ce4b
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539228"
---
# <a name="get-term"></a><span data-ttu-id="be3d3-103">获取术语</span><span class="sxs-lookup"><span data-stu-id="be3d3-103">Get term</span></span>
<span data-ttu-id="be3d3-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="be3d3-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be3d3-105">读取[术语](../resources/termstore-term.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="be3d3-105">Read the properties and relationships of a [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="be3d3-106">权限</span><span class="sxs-lookup"><span data-stu-id="be3d3-106">Permissions</span></span>
<span data-ttu-id="be3d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be3d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be3d3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="be3d3-109">Permission type</span></span>|<span data-ttu-id="be3d3-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="be3d3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be3d3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be3d3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="be3d3-112">TermStore、TermStore 和所有</span><span class="sxs-lookup"><span data-stu-id="be3d3-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="be3d3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be3d3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be3d3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="be3d3-114">Not supported.</span></span>    |
|<span data-ttu-id="be3d3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="be3d3-115">Application</span></span> | <span data-ttu-id="be3d3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="be3d3-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="be3d3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be3d3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
} -->

``` http
GET /termStore/groups/{groupId}/sets/{setId}/terms/{termId}
GET /termStore/sets/{setId}/terms/{termId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be3d3-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="be3d3-118">Optional query parameters</span></span>
<span data-ttu-id="be3d3-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="be3d3-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="be3d3-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="be3d3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="be3d3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="be3d3-121">Request headers</span></span>
|<span data-ttu-id="be3d3-122">名称</span><span class="sxs-lookup"><span data-stu-id="be3d3-122">Name</span></span>|<span data-ttu-id="be3d3-123">说明</span><span class="sxs-lookup"><span data-stu-id="be3d3-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="be3d3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="be3d3-124">Authorization</span></span>|<span data-ttu-id="be3d3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="be3d3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="be3d3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="be3d3-127">Request body</span></span>
<span data-ttu-id="be3d3-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="be3d3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be3d3-129">响应</span><span class="sxs-lookup"><span data-stu-id="be3d3-129">Response</span></span>

<span data-ttu-id="be3d3-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[term](../resources/termstore-term.md)对象。</span><span class="sxs-lookup"><span data-stu-id="be3d3-130">If successful, this method returns a `200 OK` response code and a [term](../resources/termstore-term.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be3d3-131">示例</span><span class="sxs-lookup"><span data-stu-id="be3d3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="be3d3-132">请求</span><span class="sxs-lookup"><span data-stu-id="be3d3-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_term"
} -->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}/sets/{setId}/terms/{termId}
```


### <a name="response"></a><span data-ttu-id="be3d3-133">响应</span><span class="sxs-lookup"><span data-stu-id="be3d3-133">Response</span></span>
<span data-ttu-id="be3d3-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="be3d3-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.term"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "81be9856-9856-81be-5698-be815698be81",
  "createdDateTime": "2019-06-21T20:01:37Z",
  "labels" : [
    {
        "name" : "Copy of myTerm",
        "languageTag" : "en-US",
        "isDefault" : true
    }
  ],
  "lastModifiedDateTime": "2019-06-21T20:01:37Z"
}
```

[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Get term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get term",
  "suppressions": [
  ]
}
-->

