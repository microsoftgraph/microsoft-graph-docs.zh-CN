---
title: 更新 synchronizationTemplate
description: 更新 （覆盖） 与给定应用程序关联的同步模板。
localization_priority: Normal
ms.openlocfilehash: ea4dfdc418d04467a6060a8c3d7d83423ba16e38
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816735"
---
# <a name="update-synchronizationtemplate"></a><span data-ttu-id="785dd-103">更新 synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="785dd-103">Update synchronizationTemplate</span></span>

> <span data-ttu-id="785dd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="785dd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="785dd-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="785dd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="785dd-106">更新 （覆盖） 与给定应用程序关联的同步模板。</span><span class="sxs-lookup"><span data-stu-id="785dd-106">Update (override) the synchronization template associated with a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="785dd-107">权限</span><span class="sxs-lookup"><span data-stu-id="785dd-107">Permissions</span></span>
<span data-ttu-id="785dd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="785dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="785dd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="785dd-110">Permission type</span></span>                        | <span data-ttu-id="785dd-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="785dd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="785dd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="785dd-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="785dd-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="785dd-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="785dd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="785dd-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="785dd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="785dd-115">Not supported.</span></span>|
|<span data-ttu-id="785dd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="785dd-116">Application</span></span>                            |<span data-ttu-id="785dd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="785dd-117">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="785dd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="785dd-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT application/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a><span data-ttu-id="785dd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="785dd-119">Request headers</span></span>

| <span data-ttu-id="785dd-120">名称</span><span class="sxs-lookup"><span data-stu-id="785dd-120">Name</span></span>           | <span data-ttu-id="785dd-121">类型</span><span class="sxs-lookup"><span data-stu-id="785dd-121">Type</span></span>    | <span data-ttu-id="785dd-122">说明</span><span class="sxs-lookup"><span data-stu-id="785dd-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="785dd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="785dd-123">Authorization</span></span>  | <span data-ttu-id="785dd-124">string</span><span class="sxs-lookup"><span data-stu-id="785dd-124">string</span></span>  | <span data-ttu-id="785dd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="785dd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="785dd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="785dd-127">Request body</span></span>

<span data-ttu-id="785dd-128">在请求正文中，提供要替换现有模板的[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="785dd-128">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to replace the existing template.</span></span> <span data-ttu-id="785dd-129">确保提供了所有属性。</span><span class="sxs-lookup"><span data-stu-id="785dd-129">Make sure all properties are provided.</span></span> <span data-ttu-id="785dd-130">缺少的属性将被清除。</span><span class="sxs-lookup"><span data-stu-id="785dd-130">Missing properties will be erased.</span></span>

### <a name="response"></a><span data-ttu-id="785dd-131">响应</span><span class="sxs-lookup"><span data-stu-id="785dd-131">Response</span></span>

<span data-ttu-id="785dd-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="785dd-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="examples"></a><span data-ttu-id="785dd-134">示例</span><span class="sxs-lookup"><span data-stu-id="785dd-134">Examples</span></span>

##### <a name="request"></a><span data-ttu-id="785dd-135">请求</span><span class="sxs-lookup"><span data-stu-id="785dd-135">Request</span></span>
<span data-ttu-id="785dd-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="785dd-136">The following is an example of a request.</span></span> 

><span data-ttu-id="785dd-137">**注意：** 为便于阅读将被截如下所示的请求对象。</span><span class="sxs-lookup"><span data-stu-id="785dd-137">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="785dd-138">在实际呼叫中包含的所有属性。</span><span class="sxs-lookup"><span data-stu-id="785dd-138">Include all the properties in an actual call.</span></span>
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

##### <a name="response"></a><span data-ttu-id="785dd-139">响应</span><span class="sxs-lookup"><span data-stu-id="785dd-139">Response</span></span>
<span data-ttu-id="785dd-140">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="785dd-140">The following is an example of a response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update synchronizationtemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
