---
title: 更新 printSettings
description: 更新通用打印服务的租户范围设置。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 232296196ccdee3124d79e0347dde20f5f8aeee8
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873575"
---
# <a name="update-printsettings"></a><span data-ttu-id="e025e-103">更新 printSettings</span><span class="sxs-lookup"><span data-stu-id="e025e-103">Update printSettings</span></span>

<span data-ttu-id="e025e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e025e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e025e-105">更新通用打印服务的租户范围设置。</span><span class="sxs-lookup"><span data-stu-id="e025e-105">Update tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="e025e-106">权限</span><span class="sxs-lookup"><span data-stu-id="e025e-106">Permissions</span></span>
<span data-ttu-id="e025e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e025e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e025e-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="e025e-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="e025e-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="e025e-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="e025e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e025e-111">Permission type</span></span> | <span data-ttu-id="e025e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e025e-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e025e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e025e-113">Delegated (work or school account)</span></span>| <span data-ttu-id="e025e-114">PrintSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e025e-114">PrintSettings.ReadWrite.All</span></span> |
|<span data-ttu-id="e025e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e025e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e025e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e025e-116">Not Supported.</span></span>|
|<span data-ttu-id="e025e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e025e-117">Application</span></span>|<span data-ttu-id="e025e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e025e-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e025e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e025e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/settings
```

## <a name="optional-request-headers"></a><span data-ttu-id="e025e-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="e025e-120">Optional request headers</span></span>
| <span data-ttu-id="e025e-121">名称</span><span class="sxs-lookup"><span data-stu-id="e025e-121">Name</span></span>       | <span data-ttu-id="e025e-122">说明</span><span class="sxs-lookup"><span data-stu-id="e025e-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e025e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e025e-123">Authorization</span></span> | <span data-ttu-id="e025e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e025e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e025e-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="e025e-126">Content-type</span></span>  | <span data-ttu-id="e025e-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e025e-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e025e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e025e-129">Request body</span></span>
<span data-ttu-id="e025e-130">在请求正文中，提供应更新的相关 [printSettings](../resources/printsettings.md) 字段的值。</span><span class="sxs-lookup"><span data-stu-id="e025e-130">In the request body, supply the values for the relevant [printSettings](../resources/printsettings.md) fields that should be updated.</span></span> <span data-ttu-id="e025e-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="e025e-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e025e-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="e025e-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e025e-133">属性</span><span class="sxs-lookup"><span data-stu-id="e025e-133">Property</span></span>     | <span data-ttu-id="e025e-134">类型</span><span class="sxs-lookup"><span data-stu-id="e025e-134">Type</span></span>        | <span data-ttu-id="e025e-135">Description</span><span class="sxs-lookup"><span data-stu-id="e025e-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e025e-136">documentConversionEnabled</span><span class="sxs-lookup"><span data-stu-id="e025e-136">documentConversionEnabled</span></span>|<span data-ttu-id="e025e-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="e025e-137">Boolean</span></span>|<span data-ttu-id="e025e-138">指定是否对租户启用文档转换。</span><span class="sxs-lookup"><span data-stu-id="e025e-138">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="e025e-139">如果启用文档转换，通用打印服务将自动将文档转换为与打印机设备兼容的格式 (例如，XPS 转换为 PDF) 时。</span><span class="sxs-lookup"><span data-stu-id="e025e-139">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (for example, XPS to PDF) when needed.</span></span>|

## <a name="response"></a><span data-ttu-id="e025e-140">响应</span><span class="sxs-lookup"><span data-stu-id="e025e-140">Response</span></span>
<span data-ttu-id="e025e-141">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="e025e-141">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="e025e-142">示例</span><span class="sxs-lookup"><span data-stu-id="e025e-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e025e-143">请求</span><span class="sxs-lookup"><span data-stu-id="e025e-143">Request</span></span>
<span data-ttu-id="e025e-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e025e-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e025e-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="e025e-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e025e-146">C#</span><span class="sxs-lookup"><span data-stu-id="e025e-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e025e-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e025e-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e025e-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e025e-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e025e-149">Java</span><span class="sxs-lookup"><span data-stu-id="e025e-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e025e-150">响应</span><span class="sxs-lookup"><span data-stu-id="e025e-150">Response</span></span>
<span data-ttu-id="e025e-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e025e-151">The following is an example of the response.</span></span> 
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
