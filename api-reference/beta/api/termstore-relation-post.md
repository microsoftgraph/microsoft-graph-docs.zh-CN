---
title: 创建关系
description: 创建新的 relation 对象。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8008abbfa10bbc0c7267384c66afc7c7c1c1c328
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055718"
---
# <a name="create-relation"></a><span data-ttu-id="e097d-103">创建关系</span><span class="sxs-lookup"><span data-stu-id="e097d-103">Create relation</span></span>
<span data-ttu-id="e097d-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="e097d-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e097d-105">创建新的 [relation](../resources/termstore-relation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e097d-105">Create a new [relation](../resources/termstore-relation.md) object.</span></span> <span data-ttu-id="e097d-106">这些用于在术语之间或术语和 set 之间创建固定的和 resued 的关系。</span><span class="sxs-lookup"><span data-stu-id="e097d-106">These are used to create pinned and resued relations between terms or between a term and set.</span></span> <span data-ttu-id="e097d-107">在术语和 set 之间创建固定/重用术语时，在帖子正文中 fromTerm 必须为 null。</span><span class="sxs-lookup"><span data-stu-id="e097d-107">When creating a pinned/reused term between term and set then fromTerm in the post body must be null.</span></span>

## <a name="permissions"></a><span data-ttu-id="e097d-108">权限</span><span class="sxs-lookup"><span data-stu-id="e097d-108">Permissions</span></span>
<span data-ttu-id="e097d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e097d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e097d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e097d-111">Permission type</span></span>|<span data-ttu-id="e097d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e097d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e097d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e097d-113">Delegated (work or school account)</span></span> |<span data-ttu-id="e097d-114">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e097d-114">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="e097d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e097d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e097d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e097d-116">Not supported.</span></span>    |
|<span data-ttu-id="e097d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e097d-117">Application</span></span> | <span data-ttu-id="e097d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e097d-118">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="e097d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e097d-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /termStore/sets/{setId}/terms/{termId}/relations
```

## <a name="request-headers"></a><span data-ttu-id="e097d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e097d-120">Request headers</span></span>
|<span data-ttu-id="e097d-121">名称</span><span class="sxs-lookup"><span data-stu-id="e097d-121">Name</span></span>|<span data-ttu-id="e097d-122">说明</span><span class="sxs-lookup"><span data-stu-id="e097d-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e097d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e097d-123">Authorization</span></span>|<span data-ttu-id="e097d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e097d-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e097d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e097d-126">Content-Type</span></span>|<span data-ttu-id="e097d-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e097d-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e097d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e097d-129">Request body</span></span>
<span data-ttu-id="e097d-130">在请求正文中，提供 [relation](../resources/termstore-relation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e097d-130">In the request body, supply a JSON representation of the [relation](../resources/termstore-relation.md) object.</span></span>

<span data-ttu-id="e097d-131">下表显示创建 [关系](../resources/termstore-relation.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e097d-131">The following table shows the properties that are required when you create the [relation](../resources/termstore-relation.md).</span></span>

|<span data-ttu-id="e097d-132">属性</span><span class="sxs-lookup"><span data-stu-id="e097d-132">Property</span></span>|<span data-ttu-id="e097d-133">类型</span><span class="sxs-lookup"><span data-stu-id="e097d-133">Type</span></span>|<span data-ttu-id="e097d-134">说明</span><span class="sxs-lookup"><span data-stu-id="e097d-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e097d-135">关系</span><span class="sxs-lookup"><span data-stu-id="e097d-135">relationship</span></span>|<span data-ttu-id="e097d-136">relationType</span><span class="sxs-lookup"><span data-stu-id="e097d-136">relationType</span></span>|<span data-ttu-id="e097d-137">要创建的关系类型。</span><span class="sxs-lookup"><span data-stu-id="e097d-137">Type of relation to be created.</span></span> <span data-ttu-id="e097d-138">可取值为：`pin`、`reuse`。</span><span class="sxs-lookup"><span data-stu-id="e097d-138">Possible values are: `pin`, `reuse`.</span></span>|
|<span data-ttu-id="e097d-139">set</span><span class="sxs-lookup"><span data-stu-id="e097d-139">set</span></span>| [<span data-ttu-id="e097d-140">termstore 设置</span><span class="sxs-lookup"><span data-stu-id="e097d-140">microsoft.graph.termstore.set</span></span>](../resources/termstore-set.md)| <span data-ttu-id="e097d-141">需要在其中创建关系的集合。</span><span class="sxs-lookup"><span data-stu-id="e097d-141">The set where the relationship needs to be created.</span></span>
|<span data-ttu-id="e097d-142">fromTerm</span><span class="sxs-lookup"><span data-stu-id="e097d-142">fromTerm</span></span>| [<span data-ttu-id="e097d-143">microsoft termstore</span><span class="sxs-lookup"><span data-stu-id="e097d-143">microsoft.graph.termstore.term</span></span>](../resources/termstore-term.md) | <span data-ttu-id="e097d-144">需要创建关系的术语。</span><span class="sxs-lookup"><span data-stu-id="e097d-144">The term with which the relationship needs to be created.</span></span>



## <a name="response"></a><span data-ttu-id="e097d-145">响应</span><span class="sxs-lookup"><span data-stu-id="e097d-145">Response</span></span>

<span data-ttu-id="e097d-146">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [relation](../resources/termstore-relation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e097d-146">If successful, this method returns a `201 Created` response code and a [relation](../resources/termstore-relation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e097d-147">示例</span><span class="sxs-lookup"><span data-stu-id="e097d-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e097d-148">请求</span><span class="sxs-lookup"><span data-stu-id="e097d-148">Request</span></span>

``` http
POST https://graph.microsoft.com/beta/termStore/sets/{setId}/terms/{termId}/relations
Content-Type: application/json
Content-length: 89

{
  "@odata.type": "#microsoft.graph.termStore.relation",
  "relationship": "pin",
  "fromTerm" : {
    "id" : "b49f64b3-4722-4336-9a5c-56c326b344d4"
  },
  "set" : {
    "id": "95e553ae-a91a-4670-a139-67a6cea285b3"
  }
}
```


### <a name="response"></a><span data-ttu-id="e097d-149">响应</span><span class="sxs-lookup"><span data-stu-id="e097d-149">Response</span></span>
<span data-ttu-id="e097d-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e097d-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termstore.relation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.termStore.relation",
  "id": "052c749c-749c-052c-9c74-2c059c742c05",
  "relationship": "pin",
  "fromTerm" : {
      "id" : "b49f64b3-4722-4336-9a5c-56c326b344d4"
  },
  "toTerm" : {
      "id" : "226e8ee3-f4b6-49d7-92d5-ec9d5475eec5"
  },
  "set" : {
      "id" : "95e553ae-a91a-4670-a139-67a6cea285b3"
  }
}
```

[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft.graph.termStore.term]: ../resources/termstore-term.md
[microsoft.graph.termStore.relation]: ../resources/termstore-relation.md


<!--
{
  "type": "#page.annotation",
  "description": "Create a pinned term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Pinned term",
  "suppressions": [
  ]
}
-->


