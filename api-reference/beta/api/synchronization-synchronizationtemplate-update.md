---
title: 更新 synchronizationTemplate
description: Update (override) 与给定应用程序关联的同步模板。
localization_priority: Normal
ms.openlocfilehash: 155e8c15abd8cac9b017bdaa0276561272cbbf15
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458134"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="81362-103">更新 synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="81362-103">Update synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81362-104">Update (override) 与给定应用程序关联的同步模板。</span><span class="sxs-lookup"><span data-stu-id="81362-104">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="81362-105">权限</span><span class="sxs-lookup"><span data-stu-id="81362-105">Permissions</span></span>
<span data-ttu-id="81362-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="81362-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81362-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="81362-108">Permission type</span></span>                        | <span data-ttu-id="81362-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="81362-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="81362-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="81362-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="81362-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81362-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="81362-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="81362-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="81362-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="81362-113">Not supported.</span></span>|
|<span data-ttu-id="81362-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="81362-114">Application</span></span>                            |<span data-ttu-id="81362-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="81362-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="81362-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="81362-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="81362-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="81362-117">Request headers</span></span>

| <span data-ttu-id="81362-118">名称</span><span class="sxs-lookup"><span data-stu-id="81362-118">Name</span></span>           | <span data-ttu-id="81362-119">类型</span><span class="sxs-lookup"><span data-stu-id="81362-119">Type</span></span>    | <span data-ttu-id="81362-120">说明</span><span class="sxs-lookup"><span data-stu-id="81362-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="81362-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="81362-121">Authorization</span></span>  | <span data-ttu-id="81362-122">string</span><span class="sxs-lookup"><span data-stu-id="81362-122">string</span></span>  | <span data-ttu-id="81362-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="81362-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81362-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="81362-125">Request body</span></span>

<span data-ttu-id="81362-126">在请求正文中, 提供[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)对象以替换现有模板。</span><span class="sxs-lookup"><span data-stu-id="81362-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="81362-127">请确保提供所有属性。</span><span class="sxs-lookup"><span data-stu-id="81362-127">Make sure all properties are provided.</span></span> <span data-ttu-id="81362-128">缺少的属性将被清除。</span><span class="sxs-lookup"><span data-stu-id="81362-128">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="81362-129">响应</span><span class="sxs-lookup"><span data-stu-id="81362-129">Response</span></span>

<span data-ttu-id="81362-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="81362-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="81362-132">示例</span><span class="sxs-lookup"><span data-stu-id="81362-132">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="81362-133">请求</span><span class="sxs-lookup"><span data-stu-id="81362-133">Request</span></span>
<span data-ttu-id="81362-134">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="81362-134">The following is an example of a request.</span></span> 

><span data-ttu-id="81362-135">**注意:** 为了提高可读性, 此处显示的请求对象已缩短。</span><span class="sxs-lookup"><span data-stu-id="81362-135">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="81362-136">在实际调用中包括所有属性。</span><span class="sxs-lookup"><span data-stu-id="81362-136">Include all the properties in an actual call.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="81362-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="81362-137">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="81362-138">C#</span><span class="sxs-lookup"><span data-stu-id="81362-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="81362-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="81362-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="81362-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="81362-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="81362-141">响应</span><span class="sxs-lookup"><span data-stu-id="81362-141">Response</span></span>
<span data-ttu-id="81362-142">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="81362-142">The following is an example of a response.</span></span>
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
