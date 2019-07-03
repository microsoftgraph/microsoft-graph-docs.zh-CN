---
title: 获取目录设置模板
description: 目录设置模板代表可在租户中创建设置的一种设置模板。 此操作允许检索 directorySettingTemplate 对象的属性, 包括可用的设置及其默认值。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d706c08e8c94eceb8a1eaa1d5615766aaa9ae3af
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436744"
---
# <a name="get-a-directory-setting-template"></a><span data-ttu-id="6e01c-104">获取目录设置模板</span><span class="sxs-lookup"><span data-stu-id="6e01c-104">Get a directory setting template</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e01c-105">目录设置模板代表可在租户中创建设置的一种设置模板。</span><span class="sxs-lookup"><span data-stu-id="6e01c-105">A directory setting template represents a template of settings from which settings may be created within a tenant.</span></span> <span data-ttu-id="6e01c-106">此操作允许检索 directorySettingTemplate 对象的属性, 包括可用的设置及其默认值。</span><span class="sxs-lookup"><span data-stu-id="6e01c-106">This operation allows retrieval of the properties of the directorySettingTemplate object, including the available settings and their defaults.</span></span>

> <span data-ttu-id="6e01c-107">**注意**: 此 API 的/beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="6e01c-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="6e01c-108">此 API 的/v1.0 版本已重命名为*Get groupSettingTemplate*。</span><span class="sxs-lookup"><span data-stu-id="6e01c-108">The /v1.0 version of this API has been renamed to *Get groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e01c-109">权限</span><span class="sxs-lookup"><span data-stu-id="6e01c-109">Permissions</span></span>
<span data-ttu-id="6e01c-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e01c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e01c-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e01c-112">Permission type</span></span>      | <span data-ttu-id="6e01c-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e01c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e01c-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e01c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6e01c-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6e01c-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6e01c-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e01c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e01c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e01c-117">Not supported.</span></span>    |
|<span data-ttu-id="6e01c-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e01c-118">Application</span></span> | <span data-ttu-id="6e01c-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e01c-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e01c-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e01c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6e01c-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6e01c-121">Optional query parameters</span></span>
<span data-ttu-id="6e01c-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6e01c-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e01c-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e01c-123">Request headers</span></span>
| <span data-ttu-id="6e01c-124">名称</span><span class="sxs-lookup"><span data-stu-id="6e01c-124">Name</span></span>      |<span data-ttu-id="6e01c-125">说明</span><span class="sxs-lookup"><span data-stu-id="6e01c-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6e01c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e01c-126">Authorization</span></span>  | <span data-ttu-id="6e01c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e01c-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e01c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e01c-129">Request body</span></span>
<span data-ttu-id="6e01c-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6e01c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e01c-131">响应</span><span class="sxs-lookup"><span data-stu-id="6e01c-131">Response</span></span>

<span data-ttu-id="6e01c-132">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[directorySettingTemplate](../resources/directorysettingtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6e01c-132">If successful, this method returns a `200 OK` response code and [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6e01c-133">示例</span><span class="sxs-lookup"><span data-stu-id="6e01c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6e01c-134">请求</span><span class="sxs-lookup"><span data-stu-id="6e01c-134">Request</span></span>
<span data-ttu-id="6e01c-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6e01c-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6e01c-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="6e01c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6e01c-137">C#</span><span class="sxs-lookup"><span data-stu-id="6e01c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysettingtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6e01c-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="6e01c-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysettingtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6e01c-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="6e01c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysettingtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6e01c-140">响应</span><span class="sxs-lookup"><span data-stu-id="6e01c-140">Response</span></span>
<span data-ttu-id="6e01c-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6e01c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
