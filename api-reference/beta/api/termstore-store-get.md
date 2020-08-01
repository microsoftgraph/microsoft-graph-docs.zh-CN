---
title: 获取存储区
description: 读取 store 对象的属性和关系。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 19dca69d42daac2a39d96d91d228895c99ff7d6d
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539213"
---
# <a name="get-store"></a><span data-ttu-id="4bcd6-103">获取存储区</span><span class="sxs-lookup"><span data-stu-id="4bcd6-103">Get store</span></span>
<span data-ttu-id="4bcd6-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="4bcd6-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bcd6-105">读取[store](../resources/termstore-store.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4bcd6-105">Read the properties and relationships of a [store](../resources/termstore-store.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4bcd6-106">权限</span><span class="sxs-lookup"><span data-stu-id="4bcd6-106">Permissions</span></span>
<span data-ttu-id="4bcd6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4bcd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bcd6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4bcd6-109">Permission type</span></span>|<span data-ttu-id="4bcd6-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4bcd6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bcd6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4bcd6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4bcd6-112">TermStore、TermStore 和所有</span><span class="sxs-lookup"><span data-stu-id="4bcd6-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="4bcd6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4bcd6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bcd6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4bcd6-114">Not supported.</span></span>    |
|<span data-ttu-id="4bcd6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4bcd6-115">Application</span></span> | <span data-ttu-id="4bcd6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4bcd6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bcd6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4bcd6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore
```

## <a name="request-headers"></a><span data-ttu-id="4bcd6-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4bcd6-118">Request headers</span></span>
|<span data-ttu-id="4bcd6-119">名称</span><span class="sxs-lookup"><span data-stu-id="4bcd6-119">Name</span></span>|<span data-ttu-id="4bcd6-120">说明</span><span class="sxs-lookup"><span data-stu-id="4bcd6-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4bcd6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bcd6-121">Authorization</span></span>|<span data-ttu-id="4bcd6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4bcd6-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="4bcd6-124">响应</span><span class="sxs-lookup"><span data-stu-id="4bcd6-124">Response</span></span>

<span data-ttu-id="4bcd6-125">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[store](../resources/termstore-store.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4bcd6-125">If successful, this method returns a `200 OK` response code and a [store](../resources/termstore-store.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4bcd6-126">示例</span><span class="sxs-lookup"><span data-stu-id="4bcd6-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4bcd6-127">请求</span><span class="sxs-lookup"><span data-stu-id="4bcd6-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_store"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore
```


### <a name="response"></a><span data-ttu-id="4bcd6-128">响应</span><span class="sxs-lookup"><span data-stu-id="4bcd6-128">Response</span></span>
<span data-ttu-id="4bcd6-129">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4bcd6-129">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.store"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{  
  "id": "dad13b4b-3b4b-dad1-4b3b-d1da4b3bd1da",
  "defaultLanguageTag" : "en-US",
  "languageTags" : ["en-US", "de-DE", "fr-FR"]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get termStore entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get termStore",
  "suppressions": []
}
-->
