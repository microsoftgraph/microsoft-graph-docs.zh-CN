---
title: 列出目录设置
description: 检索目录设置对象的列表。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6e20256be2dc02e8dcfaa0de25bd7275aa3f016f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260562"
---
# <a name="list-directory-settings"></a><span data-ttu-id="e8c97-103">列出目录设置</span><span class="sxs-lookup"><span data-stu-id="e8c97-103">List directory settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8c97-104">检索目录设置对象的列表。</span><span class="sxs-lookup"><span data-stu-id="e8c97-104">Retrieve a list of directory setting objects.</span></span>

> <span data-ttu-id="e8c97-105">**注意**: 此 API 的/beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="e8c97-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="e8c97-106">此 API 的/v1.0 版本已重命名为*List groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="e8c97-106">The /v1.0 version of this API has been renamed to *List groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8c97-107">权限</span><span class="sxs-lookup"><span data-stu-id="e8c97-107">Permissions</span></span>
<span data-ttu-id="e8c97-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8c97-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8c97-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8c97-110">Permission type</span></span>      | <span data-ttu-id="e8c97-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8c97-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8c97-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8c97-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e8c97-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e8c97-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e8c97-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8c97-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8c97-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8c97-115">Not supported.</span></span>    |
|<span data-ttu-id="e8c97-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8c97-116">Application</span></span> | <span data-ttu-id="e8c97-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8c97-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8c97-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8c97-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="e8c97-119">列出租户范围或组设置</span><span class="sxs-lookup"><span data-stu-id="e8c97-119">List tenant-wide or group settings</span></span>
```http
GET /settings
GET /group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e8c97-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e8c97-120">Optional query parameters</span></span>
<span data-ttu-id="e8c97-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e8c97-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8c97-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8c97-122">Request headers</span></span>
| <span data-ttu-id="e8c97-123">名称</span><span class="sxs-lookup"><span data-stu-id="e8c97-123">Name</span></span>      |<span data-ttu-id="e8c97-124">说明</span><span class="sxs-lookup"><span data-stu-id="e8c97-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e8c97-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8c97-125">Authorization</span></span>  | <span data-ttu-id="e8c97-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e8c97-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8c97-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8c97-128">Request body</span></span>
<span data-ttu-id="e8c97-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e8c97-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8c97-130">响应</span><span class="sxs-lookup"><span data-stu-id="e8c97-130">Response</span></span>

<span data-ttu-id="e8c97-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[directorySetting](../resources/directorysetting.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="e8c97-131">If successful, this method returns a `200 OK` response code and collection of [directorySetting](../resources/directorysetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e8c97-132">示例</span><span class="sxs-lookup"><span data-stu-id="e8c97-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8c97-133">请求</span><span class="sxs-lookup"><span data-stu-id="e8c97-133">Request</span></span>
<span data-ttu-id="e8c97-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e8c97-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->
```http
GET https://graph.microsoft.com/beta/settings
```
##### <a name="response"></a><span data-ttu-id="e8c97-135">响应</span><span class="sxs-lookup"><span data-stu-id="e8c97-135">Response</span></span>
<span data-ttu-id="e8c97-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e8c97-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "id": "id-value",
      "displayName": "displayName-value",
      "settingTemplateId": "settingTemplateId-value",
      "values": [
        {
          "name": "name-value",
          "value": "value-value"
        }
      ]
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e8c97-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e8c97-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e8c97-140">C#</span><span class="sxs-lookup"><span data-stu-id="e8c97-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_settings-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8c97-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="e8c97-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_settings-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e8c97-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="e8c97-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_settings-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directorysetting-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directorysetting-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
