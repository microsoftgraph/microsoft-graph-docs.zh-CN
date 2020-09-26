---
title: 创建关系
description: 创建新的 relation 对象。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8c44856d97ceb0986e6cab71d4be4d0ef62ee0b6
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288691"
---
# <a name="create-relation"></a><span data-ttu-id="8949b-103">创建关系</span><span class="sxs-lookup"><span data-stu-id="8949b-103">Create relation</span></span>
<span data-ttu-id="8949b-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="8949b-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8949b-105">创建新的 [relation](../resources/termstore-relation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8949b-105">Create a new [relation](../resources/termstore-relation.md) object.</span></span> <span data-ttu-id="8949b-106">这些关系用于在术语之间或术语和 set 之间创建固定的和重用的关系。</span><span class="sxs-lookup"><span data-stu-id="8949b-106">These are used to create pinned and reused relations between terms or between a term and set.</span></span> <span data-ttu-id="8949b-107">在术语和 set 之间创建固定/重用术语时，在帖子正文中 fromTerm 必须为 null。</span><span class="sxs-lookup"><span data-stu-id="8949b-107">When creating a pinned/reused term between term and set then fromTerm in the post body must be null.</span></span>

## <a name="permissions"></a><span data-ttu-id="8949b-108">权限</span><span class="sxs-lookup"><span data-stu-id="8949b-108">Permissions</span></span>
<span data-ttu-id="8949b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8949b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8949b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8949b-111">Permission type</span></span>|<span data-ttu-id="8949b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8949b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8949b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8949b-113">Delegated (work or school account)</span></span> |<span data-ttu-id="8949b-114">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8949b-114">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="8949b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8949b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8949b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8949b-116">Not supported.</span></span>    |
|<span data-ttu-id="8949b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8949b-117">Application</span></span> | <span data-ttu-id="8949b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="8949b-118">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="8949b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8949b-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /termStore/sets/{setId}/terms/{termId}/relations
```

## <a name="request-headers"></a><span data-ttu-id="8949b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8949b-120">Request headers</span></span>
|<span data-ttu-id="8949b-121">名称</span><span class="sxs-lookup"><span data-stu-id="8949b-121">Name</span></span>|<span data-ttu-id="8949b-122">说明</span><span class="sxs-lookup"><span data-stu-id="8949b-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8949b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8949b-123">Authorization</span></span>|<span data-ttu-id="8949b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8949b-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8949b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8949b-126">Content-Type</span></span>|<span data-ttu-id="8949b-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8949b-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8949b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8949b-129">Request body</span></span>
<span data-ttu-id="8949b-130">在请求正文中，提供 [relation](../resources/termstore-relation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8949b-130">In the request body, supply a JSON representation of the [relation](../resources/termstore-relation.md) object.</span></span>

<span data-ttu-id="8949b-131">下表显示创建 [关系](../resources/termstore-relation.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8949b-131">The following table shows the properties that are required when you create the [relation](../resources/termstore-relation.md).</span></span>

|<span data-ttu-id="8949b-132">属性</span><span class="sxs-lookup"><span data-stu-id="8949b-132">Property</span></span>|<span data-ttu-id="8949b-133">类型</span><span class="sxs-lookup"><span data-stu-id="8949b-133">Type</span></span>|<span data-ttu-id="8949b-134">说明</span><span class="sxs-lookup"><span data-stu-id="8949b-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8949b-135">关系</span><span class="sxs-lookup"><span data-stu-id="8949b-135">relationship</span></span>|<span data-ttu-id="8949b-136">relationType</span><span class="sxs-lookup"><span data-stu-id="8949b-136">relationType</span></span>|<span data-ttu-id="8949b-137">要创建的关系类型。</span><span class="sxs-lookup"><span data-stu-id="8949b-137">Type of relation to be created.</span></span> <span data-ttu-id="8949b-138">可取值为：`pin`、`reuse`。</span><span class="sxs-lookup"><span data-stu-id="8949b-138">Possible values are: `pin`, `reuse`.</span></span>|
|<span data-ttu-id="8949b-139">set</span><span class="sxs-lookup"><span data-stu-id="8949b-139">set</span></span>| [<span data-ttu-id="8949b-140">termstore 设置</span><span class="sxs-lookup"><span data-stu-id="8949b-140">microsoft.graph.termstore.set</span></span>](../resources/termstore-set.md)| <span data-ttu-id="8949b-141">需要在其中创建关系的集合。</span><span class="sxs-lookup"><span data-stu-id="8949b-141">The set where the relationship needs to be created.</span></span>
|<span data-ttu-id="8949b-142">fromTerm</span><span class="sxs-lookup"><span data-stu-id="8949b-142">fromTerm</span></span>| [<span data-ttu-id="8949b-143">microsoft termstore</span><span class="sxs-lookup"><span data-stu-id="8949b-143">microsoft.graph.termstore.term</span></span>](../resources/termstore-term.md) | <span data-ttu-id="8949b-144">需要创建关系的术语。</span><span class="sxs-lookup"><span data-stu-id="8949b-144">The term with which the relationship needs to be created.</span></span>



## <a name="response"></a><span data-ttu-id="8949b-145">响应</span><span class="sxs-lookup"><span data-stu-id="8949b-145">Response</span></span>

<span data-ttu-id="8949b-146">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [relation](../resources/termstore-relation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8949b-146">If successful, this method returns a `201 Created` response code and a [relation](../resources/termstore-relation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8949b-147">示例</span><span class="sxs-lookup"><span data-stu-id="8949b-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8949b-148">请求</span><span class="sxs-lookup"><span data-stu-id="8949b-148">Request</span></span>

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


### <a name="response"></a><span data-ttu-id="8949b-149">响应</span><span class="sxs-lookup"><span data-stu-id="8949b-149">Response</span></span>
<span data-ttu-id="8949b-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8949b-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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


