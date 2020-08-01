---
title: 更新存储
description: 更新 store 对象的属性。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: cf0c8dfb1eb5915e1a5c7b2b2538959b21cbe0d3
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539216"
---
# <a name="update-store"></a><span data-ttu-id="d7bef-103">更新存储</span><span class="sxs-lookup"><span data-stu-id="d7bef-103">Update store</span></span>
<span data-ttu-id="d7bef-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="d7bef-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7bef-105">更新[store](../resources/termstore-store.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d7bef-105">Update the properties of a [store](../resources/termstore-store.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7bef-106">权限</span><span class="sxs-lookup"><span data-stu-id="d7bef-106">Permissions</span></span>
<span data-ttu-id="d7bef-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d7bef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7bef-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d7bef-109">Permission type</span></span>|<span data-ttu-id="d7bef-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d7bef-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7bef-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7bef-111">Delegated (work or school account)</span></span> |<span data-ttu-id="d7bef-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7bef-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="d7bef-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7bef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7bef-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7bef-114">Not supported.</span></span>    |
|<span data-ttu-id="d7bef-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d7bef-115">Application</span></span> | <span data-ttu-id="d7bef-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7bef-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7bef-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7bef-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}-->

``` http
PATCH /termStore
```

## <a name="request-headers"></a><span data-ttu-id="d7bef-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7bef-118">Request headers</span></span>
|<span data-ttu-id="d7bef-119">名称</span><span class="sxs-lookup"><span data-stu-id="d7bef-119">Name</span></span>|<span data-ttu-id="d7bef-120">说明</span><span class="sxs-lookup"><span data-stu-id="d7bef-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d7bef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7bef-121">Authorization</span></span>|<span data-ttu-id="d7bef-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d7bef-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d7bef-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d7bef-124">Content-Type</span></span>|<span data-ttu-id="d7bef-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d7bef-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7bef-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d7bef-127">Request body</span></span>
<span data-ttu-id="d7bef-128">在请求正文中，提供[store](../resources/termstore-store.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7bef-128">In the request body, supply a JSON representation of the [store](../resources/termstore-store.md) object.</span></span>

<span data-ttu-id="d7bef-129">下表显示了可以为[存储区](../resources/termstore-store.md)编辑的属性。</span><span class="sxs-lookup"><span data-stu-id="d7bef-129">The following table shows the properties that can be edited for the [store](../resources/termstore-store.md).</span></span>

|<span data-ttu-id="d7bef-130">属性</span><span class="sxs-lookup"><span data-stu-id="d7bef-130">Property</span></span>|<span data-ttu-id="d7bef-131">类型</span><span class="sxs-lookup"><span data-stu-id="d7bef-131">Type</span></span>|<span data-ttu-id="d7bef-132">说明</span><span class="sxs-lookup"><span data-stu-id="d7bef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7bef-133">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="d7bef-133">defaultLanguageTag</span></span>|<span data-ttu-id="d7bef-134">String</span><span class="sxs-lookup"><span data-stu-id="d7bef-134">String</span></span>|<span data-ttu-id="d7bef-135">[Termstore](../resources/termstore-store.md)的默认语言。</span><span class="sxs-lookup"><span data-stu-id="d7bef-135">Default language of the [microsoft.graph.termstore.store](../resources/termstore-store.md)</span></span>|
|<span data-ttu-id="d7bef-136">languageTags</span><span class="sxs-lookup"><span data-stu-id="d7bef-136">languageTags</span></span>|<span data-ttu-id="d7bef-137">String collection</span><span class="sxs-lookup"><span data-stu-id="d7bef-137">String collection</span></span>|<span data-ttu-id="d7bef-138">[Termstore](../resources/termstore-store.md)中可用的语言</span><span class="sxs-lookup"><span data-stu-id="d7bef-138">Available languages in the [microsoft.graph.termstore.store](../resources/termstore-store.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d7bef-139">响应</span><span class="sxs-lookup"><span data-stu-id="d7bef-139">Response</span></span>

<span data-ttu-id="d7bef-140">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[store](../resources/termstore-store.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d7bef-140">If successful, this method returns a `200 OK` response code and an updated [store](../resources/termstore-store.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d7bef-141">示例</span><span class="sxs-lookup"><span data-stu-id="d7bef-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d7bef-142">请求</span><span class="sxs-lookup"><span data-stu-id="d7bef-142">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_store"
} -->

``` http
PATCH https://graph.microsoft.com/beta/termStore
Content-Type: application/json
Content-length: 133

{
  "defaultLanguageTag": "en-US"
}
```


### <a name="response"></a><span data-ttu-id="d7bef-143">响应</span><span class="sxs-lookup"><span data-stu-id="d7bef-143">Response</span></span>
<span data-ttu-id="d7bef-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d7bef-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "defaultLanguageTag": "en-US",
  "languageTags": [
    "en-US", 
    "fr-FR"
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Update termstore",
  "suppressions": [
  ]
}
-->

