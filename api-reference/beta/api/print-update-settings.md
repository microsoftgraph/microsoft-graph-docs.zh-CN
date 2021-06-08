---
title: 更新 printSettings
description: 更新通用打印服务的租户范围设置。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 000e8513bd4c1bfff047d50dad1fd8d1dc7fa4fa
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787607"
---
# <a name="update-printsettings"></a><span data-ttu-id="2b6e2-103">更新 printSettings</span><span class="sxs-lookup"><span data-stu-id="2b6e2-103">Update printSettings</span></span>

<span data-ttu-id="2b6e2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b6e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b6e2-105">更新通用打印服务的租户范围设置。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-105">Update tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b6e2-106">权限</span><span class="sxs-lookup"><span data-stu-id="2b6e2-106">Permissions</span></span>
<span data-ttu-id="2b6e2-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2b6e2-109">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="2b6e2-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="2b6e2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b6e2-111">Permission type</span></span> | <span data-ttu-id="2b6e2-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2b6e2-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="2b6e2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b6e2-113">Delegated (work or school account)</span></span>| <span data-ttu-id="2b6e2-114">PrintSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b6e2-114">PrintSettings.ReadWrite.All</span></span> |
|<span data-ttu-id="2b6e2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b6e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b6e2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-116">Not Supported.</span></span>|
|<span data-ttu-id="2b6e2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b6e2-117">Application</span></span>|<span data-ttu-id="2b6e2-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b6e2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b6e2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/settings
```

## <a name="optional-request-headers"></a><span data-ttu-id="2b6e2-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="2b6e2-120">Optional request headers</span></span>
| <span data-ttu-id="2b6e2-121">名称</span><span class="sxs-lookup"><span data-stu-id="2b6e2-121">Name</span></span>       | <span data-ttu-id="2b6e2-122">说明</span><span class="sxs-lookup"><span data-stu-id="2b6e2-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2b6e2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b6e2-123">Authorization</span></span> | <span data-ttu-id="2b6e2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2b6e2-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="2b6e2-126">Content-type</span></span>  | <span data-ttu-id="2b6e2-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2b6e2-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b6e2-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b6e2-129">Request body</span></span>
<span data-ttu-id="2b6e2-130">在请求正文中，提供应更新的相关 [printSettings](../resources/printsettings.md) 字段的值。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-130">In the request body, supply the values for the relevant [printSettings](../resources/printsettings.md) fields that should be updated.</span></span> <span data-ttu-id="2b6e2-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2b6e2-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2b6e2-133">属性</span><span class="sxs-lookup"><span data-stu-id="2b6e2-133">Property</span></span>     | <span data-ttu-id="2b6e2-134">类型</span><span class="sxs-lookup"><span data-stu-id="2b6e2-134">Type</span></span>        | <span data-ttu-id="2b6e2-135">说明</span><span class="sxs-lookup"><span data-stu-id="2b6e2-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2b6e2-136">documentConversionEnabled</span><span class="sxs-lookup"><span data-stu-id="2b6e2-136">documentConversionEnabled</span></span>|<span data-ttu-id="2b6e2-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b6e2-137">Boolean</span></span>|<span data-ttu-id="2b6e2-138">指定是否对租户启用文档转换。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-138">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="2b6e2-139">如果启用文档转换，则通用打印服务将自动将文档转换为与打印机模式兼容的格式 (例如，XPS 转换为 PDF) 进行打印。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-139">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (for example, XPS to PDF) when needed.</span></span>|

## <a name="response"></a><span data-ttu-id="2b6e2-140">响应</span><span class="sxs-lookup"><span data-stu-id="2b6e2-140">Response</span></span>
<span data-ttu-id="2b6e2-141">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-141">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b6e2-142">示例</span><span class="sxs-lookup"><span data-stu-id="2b6e2-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b6e2-143">请求</span><span class="sxs-lookup"><span data-stu-id="2b6e2-143">Request</span></span>
<span data-ttu-id="2b6e2-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2b6e2-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b6e2-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2b6e2-146">C#</span><span class="sxs-lookup"><span data-stu-id="2b6e2-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b6e2-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b6e2-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b6e2-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b6e2-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b6e2-149">Java</span><span class="sxs-lookup"><span data-stu-id="2b6e2-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2b6e2-150">响应</span><span class="sxs-lookup"><span data-stu-id="2b6e2-150">Response</span></span>
<span data-ttu-id="2b6e2-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2b6e2-151">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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
