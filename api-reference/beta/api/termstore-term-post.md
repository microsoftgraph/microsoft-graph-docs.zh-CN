---
title: 创建术语
description: 创建一个新的术语对象。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 2d2c18f802d9dfe68aa17b46c4dc196a31e3f93c
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539214"
---
# <a name="create-term"></a><span data-ttu-id="f7797-103">创建术语</span><span class="sxs-lookup"><span data-stu-id="f7797-103">Create term</span></span>
<span data-ttu-id="f7797-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="f7797-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7797-105">创建一个新的[术语](../resources/termstore-term.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f7797-105">Create a new [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7797-106">权限</span><span class="sxs-lookup"><span data-stu-id="f7797-106">Permissions</span></span>
<span data-ttu-id="f7797-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7797-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7797-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7797-109">Permission type</span></span>|<span data-ttu-id="f7797-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f7797-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7797-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7797-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f7797-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7797-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="f7797-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7797-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7797-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7797-114">Not supported.</span></span>    |
|<span data-ttu-id="f7797-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7797-115">Application</span></span> | <span data-ttu-id="f7797-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7797-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="f7797-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7797-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
} -->

``` http
POST /termStore/sets/{setId}/children
POST /termStore/sets/{setId}/terms/{termId}/children
```

## <a name="request-headers"></a><span data-ttu-id="f7797-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7797-118">Request headers</span></span>
|<span data-ttu-id="f7797-119">名称</span><span class="sxs-lookup"><span data-stu-id="f7797-119">Name</span></span>|<span data-ttu-id="f7797-120">说明</span><span class="sxs-lookup"><span data-stu-id="f7797-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f7797-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7797-121">Authorization</span></span>|<span data-ttu-id="f7797-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7797-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f7797-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7797-124">Content-Type</span></span>|<span data-ttu-id="f7797-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f7797-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7797-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7797-127">Request body</span></span>
<span data-ttu-id="f7797-128">在请求正文中，提供[term](../resources/termstore-term.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7797-128">In the request body, supply a JSON representation of the [term](../resources/termstore-term.md) object.</span></span>

<span data-ttu-id="f7797-129">下表显示创建[术语](../resources/termstore-term.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f7797-129">The following table shows the properties that are required when you create the [term](../resources/termstore-term.md).</span></span>

|<span data-ttu-id="f7797-130">属性</span><span class="sxs-lookup"><span data-stu-id="f7797-130">Property</span></span>|<span data-ttu-id="f7797-131">类型</span><span class="sxs-lookup"><span data-stu-id="f7797-131">Type</span></span>|<span data-ttu-id="f7797-132">说明</span><span class="sxs-lookup"><span data-stu-id="f7797-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7797-133">标题</span><span class="sxs-lookup"><span data-stu-id="f7797-133">labels</span></span>|<span data-ttu-id="f7797-134">[termStore](../resources/termstore-localizedlabel.md)集合的 localizedLabel</span><span class="sxs-lookup"><span data-stu-id="f7797-134">[microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md) collection</span></span>|<span data-ttu-id="f7797-135">要创建的术语的标签</span><span class="sxs-lookup"><span data-stu-id="f7797-135">Label for the term to be created</span></span>|



## <a name="response"></a><span data-ttu-id="f7797-136">响应</span><span class="sxs-lookup"><span data-stu-id="f7797-136">Response</span></span>

<span data-ttu-id="f7797-137">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[term](../resources/termstore-term.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f7797-137">If successful, this method returns a `201 Created` response code and a [term](../resources/termstore-term.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7797-138">示例</span><span class="sxs-lookup"><span data-stu-id="f7797-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7797-139">请求</span><span class="sxs-lookup"><span data-stu-id="f7797-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_term_from_"
} -->

``` http
POST https://graph.microsoft.com/beta/termStore/sets/{setId}/terms
Content-Type: application/json
Content-length: 366

{
  "labels": [
    {
      "languageTag" : "en-US",
      "name" : "Car",
      "isDefault" : true
    }
  ]
}
```


### <a name="response"></a><span data-ttu-id="f7797-140">响应</span><span class="sxs-lookup"><span data-stu-id="f7797-140">Response</span></span>
<span data-ttu-id="f7797-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f7797-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.term"
}-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "createdDateTime": "2019-06-21T20:01:37Z",
  "id": "8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f",
  "labels" : [
      {
          "name" : "Car",
          "languageTag" : "en-US",
          "isDefault" : true
      }
  ],
  "lastModifiedDateTime": "2019-06-21T20:01:37Z"
}
```

[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Post term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Post term",
  "suppressions": [
  ]
}
-->
