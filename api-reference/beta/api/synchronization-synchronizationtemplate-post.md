---
title: 创建 synchronizationTemplate
description: 创建新的同步模板给定应用程序。
ms.openlocfilehash: 1c7bc08eee4088796123d3c7fa2cac5c83becac2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043422"
---
# <a name="create-synchronizationtemplate"></a><span data-ttu-id="9143b-103">创建 synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="9143b-103">Create synchronizationTemplate</span></span>

> <span data-ttu-id="9143b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9143b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9143b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9143b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9143b-106">创建新的同步模板给定应用程序。</span><span class="sxs-lookup"><span data-stu-id="9143b-106">Create a new synchronization template for a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="9143b-107">权限</span><span class="sxs-lookup"><span data-stu-id="9143b-107">Permissions</span></span>
<span data-ttu-id="9143b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9143b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9143b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9143b-110">Permission type</span></span>                        | <span data-ttu-id="9143b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9143b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9143b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9143b-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="9143b-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9143b-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="9143b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9143b-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="9143b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9143b-115">Not supported.</span></span>|
|<span data-ttu-id="9143b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9143b-116">Application</span></span>                            |<span data-ttu-id="9143b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9143b-117">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="9143b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9143b-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a><span data-ttu-id="9143b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9143b-119">Request headers</span></span>

| <span data-ttu-id="9143b-120">名称</span><span class="sxs-lookup"><span data-stu-id="9143b-120">Name</span></span>           | <span data-ttu-id="9143b-121">类型</span><span class="sxs-lookup"><span data-stu-id="9143b-121">Type</span></span>    | <span data-ttu-id="9143b-122">说明</span><span class="sxs-lookup"><span data-stu-id="9143b-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="9143b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9143b-123">Authorization</span></span>  | <span data-ttu-id="9143b-124">string</span><span class="sxs-lookup"><span data-stu-id="9143b-124">string</span></span>  | <span data-ttu-id="9143b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9143b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9143b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9143b-127">Request body</span></span>

<span data-ttu-id="9143b-128">在请求正文中，提供要创建的[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9143b-128">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to be created.</span></span> <span data-ttu-id="9143b-129">`id`，`applicationId`和`factoryTag`，需要属性。</span><span class="sxs-lookup"><span data-stu-id="9143b-129">The `id`, `applicationId` and `factoryTag` properties are required.</span></span> <span data-ttu-id="9143b-130">如果没有`schema`提供的默认架构与模板，关联`factoryTag`将使用属性。</span><span class="sxs-lookup"><span data-stu-id="9143b-130">When no `schema` is provided with the template, the default schema associated with the `factoryTag` property will be used.</span></span>

### <a name="response"></a><span data-ttu-id="9143b-131">响应</span><span class="sxs-lookup"><span data-stu-id="9143b-131">Response</span></span>

<span data-ttu-id="9143b-132">如果成功，此方法返回`201 Created`响应代码和响应正文中的[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9143b-132">If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="9143b-133">示例</span><span class="sxs-lookup"><span data-stu-id="9143b-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9143b-134">请求</span><span class="sxs-lookup"><span data-stu-id="9143b-134">Request</span></span>
<span data-ttu-id="9143b-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9143b-135">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="9143b-136">响应</span><span class="sxs-lookup"><span data-stu-id="9143b-136">Response</span></span>
<span data-ttu-id="9143b-137">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="9143b-137">The following is an example of a response.</span></span>
><span data-ttu-id="9143b-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9143b-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9143b-139">将返回实际呼叫中的所有属性。</span><span class="sxs-lookup"><span data-stu-id="9143b-139">All the properties will be returned in an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->