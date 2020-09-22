---
title: 创建 synchronizationTemplate
description: 为给定应用程序创建新的同步模板。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f1477643bec6d7ca70eaec1a0c9ba000ff93db1d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087878"
---
# <a name="create-synchronizationtemplate"></a><span data-ttu-id="5877f-103">创建 synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="5877f-103">Create synchronizationTemplate</span></span>

<span data-ttu-id="5877f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5877f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5877f-105">为给定应用程序创建新的同步模板。</span><span class="sxs-lookup"><span data-stu-id="5877f-105">Create a new synchronization template for a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="5877f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="5877f-106">Permissions</span></span>
<span data-ttu-id="5877f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5877f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5877f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5877f-109">Permission type</span></span>                        | <span data-ttu-id="5877f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5877f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5877f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5877f-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="5877f-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5877f-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="5877f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5877f-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="5877f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5877f-114">Not supported.</span></span>|
|<span data-ttu-id="5877f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5877f-115">Application</span></span>                            |<span data-ttu-id="5877f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5877f-116">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="5877f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5877f-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a><span data-ttu-id="5877f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5877f-118">Request headers</span></span>

| <span data-ttu-id="5877f-119">名称</span><span class="sxs-lookup"><span data-stu-id="5877f-119">Name</span></span>           | <span data-ttu-id="5877f-120">类型</span><span class="sxs-lookup"><span data-stu-id="5877f-120">Type</span></span>    | <span data-ttu-id="5877f-121">说明</span><span class="sxs-lookup"><span data-stu-id="5877f-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="5877f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5877f-122">Authorization</span></span>  | <span data-ttu-id="5877f-123">string</span><span class="sxs-lookup"><span data-stu-id="5877f-123">string</span></span>  | <span data-ttu-id="5877f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5877f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5877f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5877f-126">Request body</span></span>

<span data-ttu-id="5877f-127">在请求正文中，提供要创建的 [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5877f-127">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to be created.</span></span> <span data-ttu-id="5877f-128">`id` `applicationId` 和 `factoryTag` 属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="5877f-128">The `id`, `applicationId` and `factoryTag` properties are required.</span></span> <span data-ttu-id="5877f-129">如果 `schema` 模板未提供，则将使用与该属性相关联的默认架构 `factoryTag` 。</span><span class="sxs-lookup"><span data-stu-id="5877f-129">When no `schema` is provided with the template, the default schema associated with the `factoryTag` property will be used.</span></span>

### <a name="response"></a><span data-ttu-id="5877f-130">响应</span><span class="sxs-lookup"><span data-stu-id="5877f-130">Response</span></span>

<span data-ttu-id="5877f-131">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5877f-131">If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="5877f-132">示例</span><span class="sxs-lookup"><span data-stu-id="5877f-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5877f-133">请求</span><span class="sxs-lookup"><span data-stu-id="5877f-133">Request</span></span>
<span data-ttu-id="5877f-134">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="5877f-134">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5877f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5877f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_synchronizationtemplate_from_synchronization"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/synchronization/templates
Content-type: application/json

{ 
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```
# <a name="c"></a>[<span data-ttu-id="5877f-136">C#</span><span class="sxs-lookup"><span data-stu-id="5877f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationtemplate-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5877f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5877f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationtemplate-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5877f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5877f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationtemplate-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5877f-139">响应</span><span class="sxs-lookup"><span data-stu-id="5877f-139">Response</span></span>
<span data-ttu-id="5877f-140">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="5877f-140">The following is an example of a response.</span></span>
><span data-ttu-id="5877f-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5877f-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5877f-142">所有属性将在实际调用中返回。</span><span class="sxs-lookup"><span data-stu-id="5877f-142">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 201 Created

{
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


