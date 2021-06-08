---
title: 更新 printSettings
description: 更新通用打印服务的租户范围设置。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 2d68bed903409fcc20b333e95245e8e15764b348
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787612"
---
# <a name="update-printsettings"></a><span data-ttu-id="2cffd-103">更新 printSettings</span><span class="sxs-lookup"><span data-stu-id="2cffd-103">Update printSettings</span></span>
<span data-ttu-id="2cffd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cffd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="2cffd-105">更新通用打印服务的租户范围设置。</span><span class="sxs-lookup"><span data-stu-id="2cffd-105">Update tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="2cffd-106">权限</span><span class="sxs-lookup"><span data-stu-id="2cffd-106">Permissions</span></span>
<span data-ttu-id="2cffd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2cffd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2cffd-109">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="2cffd-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="2cffd-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="2cffd-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="2cffd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2cffd-111">Permission type</span></span> | <span data-ttu-id="2cffd-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2cffd-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="2cffd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2cffd-113">Delegated (work or school account)</span></span>| <span data-ttu-id="2cffd-114">PrintSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cffd-114">PrintSettings.ReadWrite.All</span></span> |
|<span data-ttu-id="2cffd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2cffd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cffd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2cffd-116">Not Supported.</span></span>|
|<span data-ttu-id="2cffd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2cffd-117">Application</span></span>|<span data-ttu-id="2cffd-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2cffd-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cffd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2cffd-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/settings
```

## <a name="request-headers"></a><span data-ttu-id="2cffd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2cffd-120">Request headers</span></span>
|<span data-ttu-id="2cffd-121">名称</span><span class="sxs-lookup"><span data-stu-id="2cffd-121">Name</span></span>|<span data-ttu-id="2cffd-122">说明</span><span class="sxs-lookup"><span data-stu-id="2cffd-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2cffd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cffd-123">Authorization</span></span>|<span data-ttu-id="2cffd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2cffd-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2cffd-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2cffd-126">Content-Type</span></span>|<span data-ttu-id="2cffd-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2cffd-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cffd-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="2cffd-129">Request body</span></span>
<span data-ttu-id="2cffd-130">在请求正文中，提供应更新的相关 [printSettings](../resources/printsettings.md) 字段的值。</span><span class="sxs-lookup"><span data-stu-id="2cffd-130">In the request body, supply the values for the relevant [printSettings](../resources/printsettings.md) fields that should be updated.</span></span> <span data-ttu-id="2cffd-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="2cffd-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2cffd-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="2cffd-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2cffd-133">属性</span><span class="sxs-lookup"><span data-stu-id="2cffd-133">Property</span></span>     | <span data-ttu-id="2cffd-134">类型</span><span class="sxs-lookup"><span data-stu-id="2cffd-134">Type</span></span>        | <span data-ttu-id="2cffd-135">说明</span><span class="sxs-lookup"><span data-stu-id="2cffd-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2cffd-136">documentConversionEnabled</span><span class="sxs-lookup"><span data-stu-id="2cffd-136">documentConversionEnabled</span></span>|<span data-ttu-id="2cffd-137">布尔值</span><span class="sxs-lookup"><span data-stu-id="2cffd-137">Boolean</span></span>|<span data-ttu-id="2cffd-138">指定是否对租户启用文档转换。</span><span class="sxs-lookup"><span data-stu-id="2cffd-138">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="2cffd-139">如果启用文档转换，则通用打印服务将自动将文档转换为与打印机模式兼容的格式 (例如，XPS 转换为 PDF) 进行打印。</span><span class="sxs-lookup"><span data-stu-id="2cffd-139">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (for example, XPS to PDF) when needed.</span></span>|

## <a name="response"></a><span data-ttu-id="2cffd-140">响应</span><span class="sxs-lookup"><span data-stu-id="2cffd-140">Response</span></span>

<span data-ttu-id="2cffd-141">如果成功，此方法将返回 `204 No Content` 响应代码和空响应正文。</span><span class="sxs-lookup"><span data-stu-id="2cffd-141">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2cffd-142">示例</span><span class="sxs-lookup"><span data-stu-id="2cffd-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2cffd-143">请求</span><span class="sxs-lookup"><span data-stu-id="2cffd-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2cffd-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="2cffd-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/settings
Content-type: application/json

{
  "documentConversionEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="2cffd-145">C#</span><span class="sxs-lookup"><span data-stu-id="2cffd-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2cffd-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2cffd-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2cffd-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2cffd-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2cffd-148">Java</span><span class="sxs-lookup"><span data-stu-id="2cffd-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-printsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2cffd-149">响应</span><span class="sxs-lookup"><span data-stu-id="2cffd-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

