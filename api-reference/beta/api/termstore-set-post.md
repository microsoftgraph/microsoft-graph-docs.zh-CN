---
title: 创建集
description: 创建新的 set 对象。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: ecf1327333ddd9a38d3199c01a0c6b2436eb27a2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064586"
---
# <a name="create-set"></a><span data-ttu-id="58aca-103">创建集</span><span class="sxs-lookup"><span data-stu-id="58aca-103">Create set</span></span>
<span data-ttu-id="58aca-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="58aca-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58aca-105">创建新的 [set](../resources/termstore-set.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="58aca-105">Create a new [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="58aca-106">权限</span><span class="sxs-lookup"><span data-stu-id="58aca-106">Permissions</span></span>
<span data-ttu-id="58aca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="58aca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58aca-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="58aca-109">Permission type</span></span>|<span data-ttu-id="58aca-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="58aca-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58aca-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58aca-111">Delegated (work or school account)</span></span> |<span data-ttu-id="58aca-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58aca-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="58aca-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58aca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58aca-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="58aca-114">Not supported.</span></span>    |
|<span data-ttu-id="58aca-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="58aca-115">Application</span></span> | <span data-ttu-id="58aca-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="58aca-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="58aca-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58aca-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /termStore/sets
```

## <a name="request-headers"></a><span data-ttu-id="58aca-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="58aca-118">Request headers</span></span>
|<span data-ttu-id="58aca-119">名称</span><span class="sxs-lookup"><span data-stu-id="58aca-119">Name</span></span>|<span data-ttu-id="58aca-120">说明</span><span class="sxs-lookup"><span data-stu-id="58aca-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="58aca-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="58aca-121">Authorization</span></span>|<span data-ttu-id="58aca-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="58aca-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="58aca-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="58aca-124">Content-Type</span></span>|<span data-ttu-id="58aca-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="58aca-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="58aca-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="58aca-127">Request body</span></span>
<span data-ttu-id="58aca-128">在请求正文中，提供 [set](../resources/termstore-set.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58aca-128">In the request body, supply a JSON representation of the [set](../resources/termstore-set.md) object.</span></span>

<span data-ttu-id="58aca-129">下表显示创建 [集](../resources/termstore-set.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="58aca-129">The following table shows the properties that are required when you create the [set](../resources/termstore-set.md).</span></span>

|<span data-ttu-id="58aca-130">属性</span><span class="sxs-lookup"><span data-stu-id="58aca-130">Property</span></span>|<span data-ttu-id="58aca-131">类型</span><span class="sxs-lookup"><span data-stu-id="58aca-131">Type</span></span>|<span data-ttu-id="58aca-132">说明</span><span class="sxs-lookup"><span data-stu-id="58aca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58aca-133">localizedNames</span><span class="sxs-lookup"><span data-stu-id="58aca-133">localizedNames</span></span>|<span data-ttu-id="58aca-134">[termstore](../resources/termstore-localizedname.md) 集合的 localizedName</span><span class="sxs-lookup"><span data-stu-id="58aca-134">[microsoft.graph.termstore.localizedName](../resources/termstore-localizedname.md) collection</span></span>|<span data-ttu-id="58aca-135">要创建的集的名称</span><span class="sxs-lookup"><span data-stu-id="58aca-135">Name of the set to be created</span></span>|
|<span data-ttu-id="58aca-136">parentGroup</span><span class="sxs-lookup"><span data-stu-id="58aca-136">parentGroup</span></span>|[<span data-ttu-id="58aca-137">termstore 的组</span><span class="sxs-lookup"><span data-stu-id="58aca-137">microsoft.graph.termstore.group</span></span>](../resources/termstore-group.md)|<span data-ttu-id="58aca-138">需要在其下创建集的 termstore 组</span><span class="sxs-lookup"><span data-stu-id="58aca-138">termstore-group under which the set needs to be created</span></span>|



## <a name="response"></a><span data-ttu-id="58aca-139">响应</span><span class="sxs-lookup"><span data-stu-id="58aca-139">Response</span></span>

<span data-ttu-id="58aca-140">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [set](../resources/termstore-set.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="58aca-140">If successful, this method returns a `201 Created` response code and a [set](../resources/termstore-set.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="58aca-141">示例</span><span class="sxs-lookup"><span data-stu-id="58aca-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="58aca-142">请求</span><span class="sxs-lookup"><span data-stu-id="58aca-142">Request</span></span>
``` http
POST https://graph.microsoft.com/beta/termStore/sets
Content-Type: application/json
Content-length: 288

{
  "@odata.type": "#microsoft.graph.termStore.set",
  "parentGroup":{
      "id": "fc733b51-10f1-40fd-b784-dc6d1e42804b"
   },
   "localizedNames" : [
      {
        "languageTag" : "en-US",
        "name" : "Department"
      }
  ]
}
```


### <a name="response"></a><span data-ttu-id="58aca-143">响应</span><span class="sxs-lookup"><span data-stu-id="58aca-143">Response</span></span>
<span data-ttu-id="58aca-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="58aca-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termstore.set"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.termStore.set",
  "id": "3607e9f9-e9f9-3607-f9e9-0736f9e90736",
  "localizedNames" : [
      {
        "languageTag" : "en-US",
        "name" : "Department"
      }
  ]
}
```


[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft.graph.termStore.group]: ../resources/termstore-group.md
[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Create termSet",
  "suppressions": [
  ]
}
-->


