---
title: 获取目录设置模板
description: 目录设置模板代表可在租户中创建设置的一种设置模板。 此操作允许检索 directorySettingTemplate 对象的属性，包括可用的设置及其默认值。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8c648064f182453c3ffeccad885b7cba44ebb6de
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42433837"
---
# <a name="get-a-directory-setting-template"></a><span data-ttu-id="f0029-104">获取目录设置模板</span><span class="sxs-lookup"><span data-stu-id="f0029-104">Get a directory setting template</span></span>

<span data-ttu-id="f0029-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f0029-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0029-106">目录设置模板代表可在租户中创建设置的一种设置模板。</span><span class="sxs-lookup"><span data-stu-id="f0029-106">A directory setting template represents a template of settings from which settings may be created within a tenant.</span></span> <span data-ttu-id="f0029-107">此操作允许检索 directorySettingTemplate 对象的属性，包括可用的设置及其默认值。</span><span class="sxs-lookup"><span data-stu-id="f0029-107">This operation allows retrieval of the properties of the directorySettingTemplate object, including the available settings and their defaults.</span></span>

> <span data-ttu-id="f0029-108">**注意**：此 API 的/beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="f0029-108">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="f0029-109">此 API 的/v1.0 版本已重命名为*Get groupSettingTemplate*。</span><span class="sxs-lookup"><span data-stu-id="f0029-109">The /v1.0 version of this API has been renamed to *Get groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0029-110">权限</span><span class="sxs-lookup"><span data-stu-id="f0029-110">Permissions</span></span>
<span data-ttu-id="f0029-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f0029-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0029-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0029-113">Permission type</span></span>      | <span data-ttu-id="f0029-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f0029-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0029-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0029-115">Delegated (work or school account)</span></span> | <span data-ttu-id="f0029-116">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f0029-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f0029-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0029-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0029-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0029-118">Not supported.</span></span>    |
|<span data-ttu-id="f0029-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0029-119">Application</span></span> | <span data-ttu-id="f0029-120">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0029-120">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0029-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0029-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f0029-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f0029-122">Optional query parameters</span></span>
<span data-ttu-id="f0029-123">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f0029-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0029-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0029-124">Request headers</span></span>
| <span data-ttu-id="f0029-125">名称</span><span class="sxs-lookup"><span data-stu-id="f0029-125">Name</span></span>      |<span data-ttu-id="f0029-126">说明</span><span class="sxs-lookup"><span data-stu-id="f0029-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f0029-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0029-127">Authorization</span></span>  | <span data-ttu-id="f0029-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f0029-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0029-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0029-130">Request body</span></span>
<span data-ttu-id="f0029-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f0029-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0029-132">响应</span><span class="sxs-lookup"><span data-stu-id="f0029-132">Response</span></span>

<span data-ttu-id="f0029-133">如果成功，此方法在响应`200 OK`正文中返回响应代码和[directorySettingTemplate](../resources/directorysettingtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f0029-133">If successful, this method returns a `200 OK` response code and [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f0029-134">示例</span><span class="sxs-lookup"><span data-stu-id="f0029-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0029-135">请求</span><span class="sxs-lookup"><span data-stu-id="f0029-135">Request</span></span>
<span data-ttu-id="f0029-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f0029-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f0029-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0029-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directorySettingTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="f0029-138">C#</span><span class="sxs-lookup"><span data-stu-id="f0029-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysettingtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0029-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0029-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysettingtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0029-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0029-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysettingtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f0029-141">响应</span><span class="sxs-lookup"><span data-stu-id="f0029-141">Response</span></span>
<span data-ttu-id="f0029-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f0029-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
