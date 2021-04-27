---
title: 获取目录设置模板
description: 允许检索 directorySettingTemplate 对象的属性，包括可用设置及其默认值。
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 55b3d9d2f5a4bc141a6d8af177d30aa882a8e090
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046557"
---
# <a name="get-a-directory-setting-template"></a><span data-ttu-id="f8d37-103">获取目录设置模板</span><span class="sxs-lookup"><span data-stu-id="f8d37-103">Get a directory setting template</span></span>

<span data-ttu-id="f8d37-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8d37-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8d37-105">目录设置模板表示可以在租户中创建设置的模板。</span><span class="sxs-lookup"><span data-stu-id="f8d37-105">A directory setting template represents a template of settings from which settings may be created within a tenant.</span></span> <span data-ttu-id="f8d37-106">此操作允许检索 **directorySettingTemplate** 对象的属性，包括可用设置及其默认值。</span><span class="sxs-lookup"><span data-stu-id="f8d37-106">This operation allows retrieval of the properties of the **directorySettingTemplate** object, including the available settings and their defaults.</span></span>

> <span data-ttu-id="f8d37-107">**注意**：此 API 的 /beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="f8d37-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="f8d37-108">此 API 的 /v1.0 版本已重命名为 *Get groupSettingTemplate*。</span><span class="sxs-lookup"><span data-stu-id="f8d37-108">The /v1.0 version of this API has been renamed to *Get groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8d37-109">权限</span><span class="sxs-lookup"><span data-stu-id="f8d37-109">Permissions</span></span>
<span data-ttu-id="f8d37-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8d37-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8d37-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8d37-112">Permission type</span></span>      | <span data-ttu-id="f8d37-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8d37-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8d37-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8d37-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f8d37-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f8d37-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f8d37-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8d37-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8d37-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8d37-117">Not supported.</span></span>    |
|<span data-ttu-id="f8d37-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8d37-118">Application</span></span> | <span data-ttu-id="f8d37-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8d37-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8d37-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8d37-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f8d37-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f8d37-121">Optional query parameters</span></span>
<span data-ttu-id="f8d37-122">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f8d37-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8d37-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8d37-123">Request headers</span></span>
| <span data-ttu-id="f8d37-124">名称</span><span class="sxs-lookup"><span data-stu-id="f8d37-124">Name</span></span>      |<span data-ttu-id="f8d37-125">说明</span><span class="sxs-lookup"><span data-stu-id="f8d37-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f8d37-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8d37-126">Authorization</span></span>  | <span data-ttu-id="f8d37-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8d37-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8d37-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8d37-129">Request body</span></span>
<span data-ttu-id="f8d37-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f8d37-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8d37-131">响应</span><span class="sxs-lookup"><span data-stu-id="f8d37-131">Response</span></span>

<span data-ttu-id="f8d37-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [directorySettingTemplate](../resources/directorysettingtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f8d37-132">If successful, this method returns a `200 OK` response code and [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f8d37-133">示例</span><span class="sxs-lookup"><span data-stu-id="f8d37-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f8d37-134">请求</span><span class="sxs-lookup"><span data-stu-id="f8d37-134">Request</span></span>
<span data-ttu-id="f8d37-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f8d37-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f8d37-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8d37-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directorySettingTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="f8d37-137">C#</span><span class="sxs-lookup"><span data-stu-id="f8d37-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysettingtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8d37-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8d37-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysettingtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8d37-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8d37-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysettingtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f8d37-140">Java</span><span class="sxs-lookup"><span data-stu-id="f8d37-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directorysettingtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f8d37-141">响应</span><span class="sxs-lookup"><span data-stu-id="f8d37-141">Response</span></span>
<span data-ttu-id="f8d37-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f8d37-142">Here is an example of the response.</span></span> <span data-ttu-id="f8d37-143">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f8d37-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySettingTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 270

{
  "id": "id-value",
  "displayName": "displayName-value",
  "description": "description-value",
  "values": [
    {
      "name": "name-value",
      "type": "type-value",
      "defaultValue": "defaultValue-value",
      "description": "description-value"
    }
  ],
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directorySettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


