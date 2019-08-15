---
title: 创建 synchronizationTemplate
description: 为给定应用程序创建新的同步模板。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0be0c119d1a0d0a38030dcc9cfacbff16561c997
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409600"
---
# <a name="create-synchronizationtemplate"></a><span data-ttu-id="80abe-103">创建 synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="80abe-103">Create synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80abe-104">为给定应用程序创建新的同步模板。</span><span class="sxs-lookup"><span data-stu-id="80abe-104">Create a new synchronization template for a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="80abe-105">权限</span><span class="sxs-lookup"><span data-stu-id="80abe-105">Permissions</span></span>
<span data-ttu-id="80abe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80abe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80abe-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="80abe-108">Permission type</span></span>                        | <span data-ttu-id="80abe-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80abe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="80abe-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80abe-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="80abe-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80abe-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="80abe-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80abe-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="80abe-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="80abe-113">Not supported.</span></span>|
|<span data-ttu-id="80abe-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="80abe-114">Application</span></span>                            |<span data-ttu-id="80abe-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="80abe-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="80abe-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80abe-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a><span data-ttu-id="80abe-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="80abe-117">Request headers</span></span>

| <span data-ttu-id="80abe-118">名称</span><span class="sxs-lookup"><span data-stu-id="80abe-118">Name</span></span>           | <span data-ttu-id="80abe-119">类型</span><span class="sxs-lookup"><span data-stu-id="80abe-119">Type</span></span>    | <span data-ttu-id="80abe-120">说明</span><span class="sxs-lookup"><span data-stu-id="80abe-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="80abe-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="80abe-121">Authorization</span></span>  | <span data-ttu-id="80abe-122">string</span><span class="sxs-lookup"><span data-stu-id="80abe-122">string</span></span>  | <span data-ttu-id="80abe-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="80abe-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80abe-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="80abe-125">Request body</span></span>

<span data-ttu-id="80abe-126">在请求正文中, 提供要创建的[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="80abe-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to be created.</span></span> <span data-ttu-id="80abe-127">和属性是必需的`id` `applicationId` `factoryTag`</span><span class="sxs-lookup"><span data-stu-id="80abe-127">The `id`, `applicationId` and `factoryTag` properties are required.</span></span> <span data-ttu-id="80abe-128">如果模板`schema`未提供, 则将使用与该`factoryTag`属性相关联的默认架构。</span><span class="sxs-lookup"><span data-stu-id="80abe-128">When no `schema` is provided with the template, the default schema associated with the `factoryTag` property will be used.</span></span>

### <a name="response"></a><span data-ttu-id="80abe-129">响应</span><span class="sxs-lookup"><span data-stu-id="80abe-129">Response</span></span>

<span data-ttu-id="80abe-130">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="80abe-130">If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="80abe-131">示例</span><span class="sxs-lookup"><span data-stu-id="80abe-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="80abe-132">请求</span><span class="sxs-lookup"><span data-stu-id="80abe-132">Request</span></span>
<span data-ttu-id="80abe-133">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="80abe-133">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="80abe-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="80abe-134">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="80abe-135">C#</span><span class="sxs-lookup"><span data-stu-id="80abe-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationtemplate-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="80abe-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80abe-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationtemplate-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="80abe-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="80abe-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationtemplate-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="80abe-138">响应</span><span class="sxs-lookup"><span data-stu-id="80abe-138">Response</span></span>
<span data-ttu-id="80abe-139">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="80abe-139">The following is an example of a response.</span></span>
><span data-ttu-id="80abe-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="80abe-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="80abe-141">所有属性将在实际调用中返回。</span><span class="sxs-lookup"><span data-stu-id="80abe-141">All the properties will be returned in an actual call.</span></span>
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
