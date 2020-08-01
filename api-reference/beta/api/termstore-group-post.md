---
title: 创建组
description: 创建新的 group 对象。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: c81a095a14599622fa273973a1f3581b5b84921f
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539240"
---
# <a name="create-group"></a><span data-ttu-id="d5dab-103">创建组</span><span class="sxs-lookup"><span data-stu-id="d5dab-103">Create group</span></span>
<span data-ttu-id="d5dab-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="d5dab-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5dab-105">创建新的[group](../resources/termstore-group.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d5dab-105">Create a new [group](../resources/termstore-group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5dab-106">权限</span><span class="sxs-lookup"><span data-stu-id="d5dab-106">Permissions</span></span>
<span data-ttu-id="d5dab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5dab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5dab-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5dab-109">Permission type</span></span>|<span data-ttu-id="d5dab-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d5dab-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5dab-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5dab-111">Delegated (work or school account)</span></span> |<span data-ttu-id="d5dab-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5dab-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="d5dab-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5dab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5dab-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5dab-114">Not supported.</span></span>    |
|<span data-ttu-id="d5dab-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5dab-115">Application</span></span> | <span data-ttu-id="d5dab-116">不支持</span><span class="sxs-lookup"><span data-stu-id="d5dab-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5dab-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5dab-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /termStore/groups
```

## <a name="request-headers"></a><span data-ttu-id="d5dab-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5dab-118">Request headers</span></span>
|<span data-ttu-id="d5dab-119">名称</span><span class="sxs-lookup"><span data-stu-id="d5dab-119">Name</span></span>|<span data-ttu-id="d5dab-120">说明</span><span class="sxs-lookup"><span data-stu-id="d5dab-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d5dab-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5dab-121">Authorization</span></span>|<span data-ttu-id="d5dab-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d5dab-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d5dab-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d5dab-124">Content-Type</span></span>|<span data-ttu-id="d5dab-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d5dab-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5dab-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5dab-127">Request body</span></span>
<span data-ttu-id="d5dab-128">在请求正文中，提供[group](../resources/termstore-group.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5dab-128">In the request body, supply a JSON representation of the [group](../resources/termstore-group.md) object.</span></span>

<span data-ttu-id="d5dab-129">下表显示创建[组](../resources/termstore-group.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d5dab-129">The following table shows the properties that are required when you create the [group](../resources/termstore-group.md).</span></span>

|<span data-ttu-id="d5dab-130">属性</span><span class="sxs-lookup"><span data-stu-id="d5dab-130">Property</span></span>|<span data-ttu-id="d5dab-131">类型</span><span class="sxs-lookup"><span data-stu-id="d5dab-131">Type</span></span>|<span data-ttu-id="d5dab-132">说明</span><span class="sxs-lookup"><span data-stu-id="d5dab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5dab-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d5dab-133">displayName</span></span>|<span data-ttu-id="d5dab-134">String</span><span class="sxs-lookup"><span data-stu-id="d5dab-134">String</span></span>|<span data-ttu-id="d5dab-135">要创建的组的名称。</span><span class="sxs-lookup"><span data-stu-id="d5dab-135">Name of the group to be created.</span></span>|



## <a name="response"></a><span data-ttu-id="d5dab-136">响应</span><span class="sxs-lookup"><span data-stu-id="d5dab-136">Response</span></span>

<span data-ttu-id="d5dab-137">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [group](../resources/termstore-group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d5dab-137">If successful, this method returns a `201 Created` response code and a [group](../resources/termstore-group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d5dab-138">示例</span><span class="sxs-lookup"><span data-stu-id="d5dab-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d5dab-139">请求</span><span class="sxs-lookup"><span data-stu-id="d5dab-139">Request</span></span>
<!-- {
  "blockType": "request",
  "displayName": "myGroup"
}-->

``` http
POST https://graph.microsoft.com/beta/termStore/groups
Content-Type: application/json
Content-length: 135

{
  "displayName" : "myGroup"
}
```


### <a name="response"></a><span data-ttu-id="d5dab-140">响应</span><span class="sxs-lookup"><span data-stu-id="d5dab-140">Response</span></span>
<span data-ttu-id="d5dab-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d5dab-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.group"
}-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "85825593-5593-8582-9355-828593558285",
  "createdDateTime": "2019-06-21T20:01:37Z",
  "description": "My term group",
  "scope" : "global",
  "displayName": "myGroup"  
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Create a termGroup entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Create termGroup",
  "suppressions": [
  ]
}
-->
