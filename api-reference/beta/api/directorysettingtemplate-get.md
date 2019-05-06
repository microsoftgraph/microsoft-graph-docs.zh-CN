---
title: 获取目录设置模板
description: 目录设置模板代表可在租户中创建设置的一种设置模板。 此操作允许检索 directorySettingTemplate 对象的属性, 包括可用的设置及其默认值。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7c419be1bb9934b235c361112e9f79129fea6828
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589498"
---
# <a name="get-a-directory-setting-template"></a><span data-ttu-id="50ef5-104">获取目录设置模板</span><span class="sxs-lookup"><span data-stu-id="50ef5-104">Get a directory setting template</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50ef5-105">目录设置模板代表可在租户中创建设置的一种设置模板。</span><span class="sxs-lookup"><span data-stu-id="50ef5-105">A directory setting template represents a template of settings from which settings may be created within a tenant.</span></span> <span data-ttu-id="50ef5-106">此操作允许检索 directorySettingTemplate 对象的属性, 包括可用的设置及其默认值。</span><span class="sxs-lookup"><span data-stu-id="50ef5-106">This operation allows retrieval of the properties of the directorySettingTemplate object, including the available settings and their defaults.</span></span>

> <span data-ttu-id="50ef5-107">**注意**: 此 API 的/beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="50ef5-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="50ef5-108">此 API 的/v1.0 版本已重命名为*Get groupSettingTemplate*。</span><span class="sxs-lookup"><span data-stu-id="50ef5-108">The /v1.0 version of this API has been renamed to *Get groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="50ef5-109">权限</span><span class="sxs-lookup"><span data-stu-id="50ef5-109">Permissions</span></span>
<span data-ttu-id="50ef5-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50ef5-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50ef5-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="50ef5-112">Permission type</span></span>      | <span data-ttu-id="50ef5-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50ef5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50ef5-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50ef5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="50ef5-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="50ef5-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="50ef5-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50ef5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50ef5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="50ef5-117">Not supported.</span></span>    |
|<span data-ttu-id="50ef5-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="50ef5-118">Application</span></span> | <span data-ttu-id="50ef5-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50ef5-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="50ef5-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50ef5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="50ef5-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="50ef5-121">Optional query parameters</span></span>
<span data-ttu-id="50ef5-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="50ef5-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50ef5-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="50ef5-123">Request headers</span></span>
| <span data-ttu-id="50ef5-124">名称</span><span class="sxs-lookup"><span data-stu-id="50ef5-124">Name</span></span>      |<span data-ttu-id="50ef5-125">说明</span><span class="sxs-lookup"><span data-stu-id="50ef5-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="50ef5-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="50ef5-126">Authorization</span></span>  | <span data-ttu-id="50ef5-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="50ef5-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="50ef5-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="50ef5-129">Request body</span></span>
<span data-ttu-id="50ef5-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="50ef5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50ef5-131">响应</span><span class="sxs-lookup"><span data-stu-id="50ef5-131">Response</span></span>

<span data-ttu-id="50ef5-132">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[directorySettingTemplate](../resources/directorysettingtemplate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="50ef5-132">If successful, this method returns a `200 OK` response code and [directorySettingTemplate](../resources/directorysettingtemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="50ef5-133">示例</span><span class="sxs-lookup"><span data-stu-id="50ef5-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50ef5-134">请求</span><span class="sxs-lookup"><span data-stu-id="50ef5-134">Request</span></span>
<span data-ttu-id="50ef5-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50ef5-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplate"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="50ef5-136">响应</span><span class="sxs-lookup"><span data-stu-id="50ef5-136">Response</span></span>
<span data-ttu-id="50ef5-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="50ef5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="50ef5-140">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="50ef5-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="50ef5-141">语言</span><span class="sxs-lookup"><span data-stu-id="50ef5-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directorysettingtemplate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="50ef5-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="50ef5-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directorysettingtemplate-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/directorysettingtemplate-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directorysettingtemplate-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
