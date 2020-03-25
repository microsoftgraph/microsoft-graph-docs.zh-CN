---
title: 更新设置
description: 更新通用打印服务的租户范围设置。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: d9e17edaf303c1e62aef4211e080cbdf5d2d00cc
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948199"
---
# <a name="update-settings"></a><span data-ttu-id="d0c15-103">更新设置</span><span class="sxs-lookup"><span data-stu-id="d0c15-103">Update settings</span></span>

<span data-ttu-id="d0c15-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0c15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0c15-105">更新通用打印服务的租户范围设置。</span><span class="sxs-lookup"><span data-stu-id="d0c15-105">Update tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0c15-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d0c15-106">Permissions</span></span>
<span data-ttu-id="d0c15-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0c15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d0c15-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="d0c15-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="d0c15-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0c15-110">Permission type</span></span> | <span data-ttu-id="d0c15-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0c15-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="d0c15-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0c15-112">Delegated (work or school account)</span></span>| <span data-ttu-id="d0c15-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="d0c15-113">Users.Read.All</span></span> |
|<span data-ttu-id="d0c15-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0c15-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0c15-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0c15-115">Not Supported.</span></span>|
|<span data-ttu-id="d0c15-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0c15-116">Application</span></span>|<span data-ttu-id="d0c15-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0c15-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0c15-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0c15-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/settings
```

## <a name="optional-request-headers"></a><span data-ttu-id="d0c15-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="d0c15-119">Optional request headers</span></span>
| <span data-ttu-id="d0c15-120">名称</span><span class="sxs-lookup"><span data-stu-id="d0c15-120">Name</span></span>       | <span data-ttu-id="d0c15-121">说明</span><span class="sxs-lookup"><span data-stu-id="d0c15-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d0c15-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0c15-122">Authorization</span></span> | <span data-ttu-id="d0c15-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d0c15-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d0c15-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="d0c15-125">Content-type</span></span>  | <span data-ttu-id="d0c15-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d0c15-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0c15-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0c15-128">Request body</span></span>
<span data-ttu-id="d0c15-129">在请求正文中，提供应更新的相关[printSettings](../resources/printsettings.md)字段的值。</span><span class="sxs-lookup"><span data-stu-id="d0c15-129">In the request body, supply the values for the relevant [printSettings](../resources/printsettings.md) fields that should be updated.</span></span> <span data-ttu-id="d0c15-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="d0c15-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d0c15-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d0c15-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d0c15-132">属性</span><span class="sxs-lookup"><span data-stu-id="d0c15-132">Property</span></span>     | <span data-ttu-id="d0c15-133">类型</span><span class="sxs-lookup"><span data-stu-id="d0c15-133">Type</span></span>        | <span data-ttu-id="d0c15-134">说明</span><span class="sxs-lookup"><span data-stu-id="d0c15-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d0c15-135">documentConversionEnabled</span><span class="sxs-lookup"><span data-stu-id="d0c15-135">documentConversionEnabled</span></span>|<span data-ttu-id="d0c15-136">布尔</span><span class="sxs-lookup"><span data-stu-id="d0c15-136">Boolean</span></span>|<span data-ttu-id="d0c15-137">指定是否为租户启用文档转换。</span><span class="sxs-lookup"><span data-stu-id="d0c15-137">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="d0c15-138">如果启用了文档转换，则通用打印服务会在需要时自动将文档转换为与打印机兼容的格式（例如，XPS 转换为 PDF）。</span><span class="sxs-lookup"><span data-stu-id="d0c15-138">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (for example, XPS to PDF) when needed.</span></span>|

## <a name="response"></a><span data-ttu-id="d0c15-139">响应</span><span class="sxs-lookup"><span data-stu-id="d0c15-139">Response</span></span>
<span data-ttu-id="d0c15-140">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="d0c15-140">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0c15-141">示例</span><span class="sxs-lookup"><span data-stu-id="d0c15-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0c15-142">请求</span><span class="sxs-lookup"><span data-stu-id="d0c15-142">Request</span></span>
<span data-ttu-id="d0c15-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d0c15-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d0c15-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0c15-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_settings"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/settings
Content-type: application/json

{
  "documentConversionEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="d0c15-145">C#</span><span class="sxs-lookup"><span data-stu-id="d0c15-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0c15-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0c15-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0c15-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0c15-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d0c15-148">响应</span><span class="sxs-lookup"><span data-stu-id="d0c15-148">Response</span></span>
<span data-ttu-id="d0c15-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d0c15-149">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printSettings"
} -->
```http
HTTP/1.1 204 NoContent
Content-length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
