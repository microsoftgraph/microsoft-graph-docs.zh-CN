---
title: 更新 synchronizationTemplate
description: Update （override）与给定应用程序关联的同步模板。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: afc5e0e557f89866f14507314f3673d92df76d7e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471129"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="7a558-103">更新 synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="7a558-103">Update synchronizationTemplate</span></span>

<span data-ttu-id="7a558-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a558-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a558-105">Update （override）与给定应用程序关联的同步模板。</span><span class="sxs-lookup"><span data-stu-id="7a558-105">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a558-106">权限</span><span class="sxs-lookup"><span data-stu-id="7a558-106">Permissions</span></span>
<span data-ttu-id="7a558-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7a558-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a558-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7a558-109">Permission type</span></span>                        | <span data-ttu-id="7a558-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7a558-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a558-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7a558-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="7a558-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a558-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="7a558-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7a558-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="7a558-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a558-114">Not supported.</span></span>|
|<span data-ttu-id="7a558-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7a558-115">Application</span></span>                            |<span data-ttu-id="7a558-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a558-116">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="7a558-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7a558-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="7a558-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7a558-118">Request headers</span></span>

| <span data-ttu-id="7a558-119">名称</span><span class="sxs-lookup"><span data-stu-id="7a558-119">Name</span></span>           | <span data-ttu-id="7a558-120">类型</span><span class="sxs-lookup"><span data-stu-id="7a558-120">Type</span></span>    | <span data-ttu-id="7a558-121">说明</span><span class="sxs-lookup"><span data-stu-id="7a558-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="7a558-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a558-122">Authorization</span></span>  | <span data-ttu-id="7a558-123">string</span><span class="sxs-lookup"><span data-stu-id="7a558-123">string</span></span>  | <span data-ttu-id="7a558-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7a558-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a558-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7a558-126">Request body</span></span>

<span data-ttu-id="7a558-127">在请求正文中，提供[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)对象以替换现有模板。</span><span class="sxs-lookup"><span data-stu-id="7a558-127">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="7a558-128">请确保提供所有属性。</span><span class="sxs-lookup"><span data-stu-id="7a558-128">Make sure all properties are provided.</span></span> <span data-ttu-id="7a558-129">缺少的属性将被清除。</span><span class="sxs-lookup"><span data-stu-id="7a558-129">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="7a558-130">响应</span><span class="sxs-lookup"><span data-stu-id="7a558-130">Response</span></span>

<span data-ttu-id="7a558-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7a558-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="7a558-133">示例</span><span class="sxs-lookup"><span data-stu-id="7a558-133">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="7a558-134">请求</span><span class="sxs-lookup"><span data-stu-id="7a558-134">Request</span></span>
<span data-ttu-id="7a558-135">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="7a558-135">The following is an example of a request.</span></span> 

><span data-ttu-id="7a558-136">**注意：** 为了提高可读性，此处显示的请求对象已缩短。</span><span class="sxs-lookup"><span data-stu-id="7a558-136">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="7a558-137">在实际调用中包括所有属性。</span><span class="sxs-lookup"><span data-stu-id="7a558-137">Include all the properties in an actual call.</span></span>

# <a name="http"></a>[<span data-ttu-id="7a558-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a558-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7a558-139">C#</span><span class="sxs-lookup"><span data-stu-id="7a558-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a558-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a558-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a558-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a558-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7a558-142">响应</span><span class="sxs-lookup"><span data-stu-id="7a558-142">Response</span></span>
<span data-ttu-id="7a558-143">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="7a558-143">The following is an example of a response.</span></span>
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
