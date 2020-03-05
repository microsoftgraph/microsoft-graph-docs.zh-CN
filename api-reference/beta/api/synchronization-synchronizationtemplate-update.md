---
title: 更新 synchronizationTemplate
description: Update （override）与给定应用程序关联的同步模板。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4327da9f4eb54c0e740370338806dc4078f2672c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452874"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="ccddb-103">更新 synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="ccddb-103">Update synchronizationTemplate</span></span>

<span data-ttu-id="ccddb-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ccddb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccddb-105">Update （override）与给定应用程序关联的同步模板。</span><span class="sxs-lookup"><span data-stu-id="ccddb-105">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccddb-106">权限</span><span class="sxs-lookup"><span data-stu-id="ccddb-106">Permissions</span></span>
<span data-ttu-id="ccddb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ccddb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccddb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ccddb-109">Permission type</span></span>                        | <span data-ttu-id="ccddb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ccddb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccddb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ccddb-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="ccddb-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccddb-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="ccddb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ccddb-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="ccddb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ccddb-114">Not supported.</span></span>|
|<span data-ttu-id="ccddb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ccddb-115">Application</span></span>                            |<span data-ttu-id="ccddb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ccddb-116">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="ccddb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ccddb-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="ccddb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ccddb-118">Request headers</span></span>

| <span data-ttu-id="ccddb-119">名称</span><span class="sxs-lookup"><span data-stu-id="ccddb-119">Name</span></span>           | <span data-ttu-id="ccddb-120">类型</span><span class="sxs-lookup"><span data-stu-id="ccddb-120">Type</span></span>    | <span data-ttu-id="ccddb-121">说明</span><span class="sxs-lookup"><span data-stu-id="ccddb-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="ccddb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccddb-122">Authorization</span></span>  | <span data-ttu-id="ccddb-123">string</span><span class="sxs-lookup"><span data-stu-id="ccddb-123">string</span></span>  | <span data-ttu-id="ccddb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ccddb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ccddb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ccddb-126">Request body</span></span>

<span data-ttu-id="ccddb-127">在请求正文中，提供[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)对象以替换现有模板。</span><span class="sxs-lookup"><span data-stu-id="ccddb-127">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="ccddb-128">请确保提供所有属性。</span><span class="sxs-lookup"><span data-stu-id="ccddb-128">Make sure all properties are provided.</span></span> <span data-ttu-id="ccddb-129">缺少的属性将被清除。</span><span class="sxs-lookup"><span data-stu-id="ccddb-129">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="ccddb-130">响应</span><span class="sxs-lookup"><span data-stu-id="ccddb-130">Response</span></span>

<span data-ttu-id="ccddb-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ccddb-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="ccddb-133">示例</span><span class="sxs-lookup"><span data-stu-id="ccddb-133">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="ccddb-134">请求</span><span class="sxs-lookup"><span data-stu-id="ccddb-134">Request</span></span>
<span data-ttu-id="ccddb-135">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="ccddb-135">The following is an example of a request.</span></span> 

><span data-ttu-id="ccddb-136">**注意：** 为了提高可读性，此处显示的请求对象已缩短。</span><span class="sxs-lookup"><span data-stu-id="ccddb-136">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="ccddb-137">在实际调用中包括所有属性。</span><span class="sxs-lookup"><span data-stu-id="ccddb-137">Include all the properties in an actual call.</span></span>

# <a name="http"></a>[<span data-ttu-id="ccddb-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccddb-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ccddb-139">C#</span><span class="sxs-lookup"><span data-stu-id="ccddb-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccddb-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccddb-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccddb-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccddb-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ccddb-142">响应</span><span class="sxs-lookup"><span data-stu-id="ccddb-142">Response</span></span>
<span data-ttu-id="ccddb-143">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="ccddb-143">The following is an example of a response.</span></span>
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
