---
title: 更新 synchronizationTemplate
description: Update (override) 与给定应用程序关联的同步模板。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 132bc669122cae84acbd85163c80bb035520a8a8
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409614"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="001b2-103">更新 synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="001b2-103">Update synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="001b2-104">Update (override) 与给定应用程序关联的同步模板。</span><span class="sxs-lookup"><span data-stu-id="001b2-104">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="001b2-105">权限</span><span class="sxs-lookup"><span data-stu-id="001b2-105">Permissions</span></span>
<span data-ttu-id="001b2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="001b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="001b2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="001b2-108">Permission type</span></span>                        | <span data-ttu-id="001b2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="001b2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="001b2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="001b2-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="001b2-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="001b2-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="001b2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="001b2-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="001b2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="001b2-113">Not supported.</span></span>|
|<span data-ttu-id="001b2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="001b2-114">Application</span></span>                            |<span data-ttu-id="001b2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="001b2-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="001b2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="001b2-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="001b2-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="001b2-117">Request headers</span></span>

| <span data-ttu-id="001b2-118">名称</span><span class="sxs-lookup"><span data-stu-id="001b2-118">Name</span></span>           | <span data-ttu-id="001b2-119">类型</span><span class="sxs-lookup"><span data-stu-id="001b2-119">Type</span></span>    | <span data-ttu-id="001b2-120">说明</span><span class="sxs-lookup"><span data-stu-id="001b2-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="001b2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="001b2-121">Authorization</span></span>  | <span data-ttu-id="001b2-122">string</span><span class="sxs-lookup"><span data-stu-id="001b2-122">string</span></span>  | <span data-ttu-id="001b2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="001b2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="001b2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="001b2-125">Request body</span></span>

<span data-ttu-id="001b2-126">在请求正文中, 提供[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)对象以替换现有模板。</span><span class="sxs-lookup"><span data-stu-id="001b2-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="001b2-127">请确保提供所有属性。</span><span class="sxs-lookup"><span data-stu-id="001b2-127">Make sure all properties are provided.</span></span> <span data-ttu-id="001b2-128">缺少的属性将被清除。</span><span class="sxs-lookup"><span data-stu-id="001b2-128">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="001b2-129">响应</span><span class="sxs-lookup"><span data-stu-id="001b2-129">Response</span></span>

<span data-ttu-id="001b2-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="001b2-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="001b2-132">示例</span><span class="sxs-lookup"><span data-stu-id="001b2-132">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="001b2-133">请求</span><span class="sxs-lookup"><span data-stu-id="001b2-133">Request</span></span>
<span data-ttu-id="001b2-134">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="001b2-134">The following is an example of a request.</span></span> 

><span data-ttu-id="001b2-135">**注意:** 为了提高可读性, 此处显示的请求对象已缩短。</span><span class="sxs-lookup"><span data-stu-id="001b2-135">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="001b2-136">在实际调用中包括所有属性。</span><span class="sxs-lookup"><span data-stu-id="001b2-136">Include all the properties in an actual call.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="001b2-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="001b2-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_synchronizationtemplate"
}-->
```http
PUT https://graph.microsoft.com/beta/applications/{id}/synchronization/templates/{templateId}
Authorization: Bearer <token>
Content-type: application/json

{
    "id": "Slack",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="001b2-138">C#</span><span class="sxs-lookup"><span data-stu-id="001b2-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="001b2-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="001b2-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="001b2-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="001b2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="001b2-141">响应</span><span class="sxs-lookup"><span data-stu-id="001b2-141">Response</span></span>
<span data-ttu-id="001b2-142">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="001b2-142">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update synchronizationtemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
