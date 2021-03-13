---
title: tag： asHierarchy
description: 以层次结构形式返回标记列表。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 34834c8ee010c8365a68b587b333bdaae6abe1fd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772532"
---
# <a name="tag-ashierarchy"></a><span data-ttu-id="2fe71-103">tag： asHierarchy</span><span class="sxs-lookup"><span data-stu-id="2fe71-103">tag: asHierarchy</span></span>

<span data-ttu-id="2fe71-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="2fe71-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fe71-105">返回层次结构 [窗体中的标记](../resources/ediscovery-tag.md) 对象列表</span><span class="sxs-lookup"><span data-stu-id="2fe71-105">Return a list of [tag](../resources/ediscovery-tag.md) objects in hierarchial form</span></span>

## <a name="permissions"></a><span data-ttu-id="2fe71-106">权限</span><span class="sxs-lookup"><span data-stu-id="2fe71-106">Permissions</span></span>

<span data-ttu-id="2fe71-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2fe71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fe71-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2fe71-109">Permission type</span></span>|<span data-ttu-id="2fe71-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2fe71-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fe71-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2fe71-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2fe71-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fe71-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="2fe71-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2fe71-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fe71-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2fe71-114">Not supported.</span></span>|
|<span data-ttu-id="2fe71-115">Application</span><span class="sxs-lookup"><span data-stu-id="2fe71-115">Application</span></span>|<span data-ttu-id="2fe71-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2fe71-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fe71-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2fe71-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/tags/asHierarchy
```

## <a name="request-headers"></a><span data-ttu-id="2fe71-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2fe71-118">Request headers</span></span>

|<span data-ttu-id="2fe71-119">名称</span><span class="sxs-lookup"><span data-stu-id="2fe71-119">Name</span></span>|<span data-ttu-id="2fe71-120">说明</span><span class="sxs-lookup"><span data-stu-id="2fe71-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2fe71-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fe71-121">Authorization</span></span>|<span data-ttu-id="2fe71-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2fe71-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fe71-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="2fe71-124">Request body</span></span>

<span data-ttu-id="2fe71-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2fe71-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2fe71-126">响应</span><span class="sxs-lookup"><span data-stu-id="2fe71-126">Response</span></span>

<span data-ttu-id="2fe71-127">如果成功，此函数在响应正文中返回 响应代码和 `200 OK` [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="2fe71-127">If successful, this function returns a `200 OK` response code and a [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2fe71-128">示例</span><span class="sxs-lookup"><span data-stu-id="2fe71-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2fe71-129">请求</span><span class="sxs-lookup"><span data-stu-id="2fe71-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2fe71-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="2fe71-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tag_ashierarchy"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/asHierarchy
```
# <a name="c"></a>[<span data-ttu-id="2fe71-131">C#</span><span class="sxs-lookup"><span data-stu-id="2fe71-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tag-ashierarchy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2fe71-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2fe71-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tag-ashierarchy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2fe71-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2fe71-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tag-ashierarchy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2fe71-134">Java</span><span class="sxs-lookup"><span data-stu-id="2fe71-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tag-ashierarchy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2fe71-135">响应</span><span class="sxs-lookup"><span data-stu-id="2fe71-135">Response</span></span>

<span data-ttu-id="2fe71-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2fe71-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.tag)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ediscovery.tag",
      "id": "String (identifier)",
      "displayName": "String",
      "description": "String",
      "childSelectability": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "String (timestamp)"
    }
  ]
}
```
