---
title: 列出 directorySettingTemplates
description: 目录设置模板代表目录设置的一组模板, 在租户中可以创建和使用目录设置。  此操作将检索可用的 directorySettingTemplates 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bb5bedbb01527894edc712b71a531b1ddcbbc6d5
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260499"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="8da8a-104">列出 directorySettingTemplates</span><span class="sxs-lookup"><span data-stu-id="8da8a-104">List directorySettingTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8da8a-105">目录设置模板代表目录设置的一组模板, 在租户中可以创建和使用目录设置。</span><span class="sxs-lookup"><span data-stu-id="8da8a-105">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="8da8a-106">此操作将检索可用的 directorySettingTemplates 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="8da8a-106">This operation retrieves the list of available directorySettingTemplates objects.</span></span>

> <span data-ttu-id="8da8a-107">**注意**: 此 API 的/beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="8da8a-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="8da8a-108">此 API 的/v1.0 版本已重命名为*List groupSettingTemplate*。</span><span class="sxs-lookup"><span data-stu-id="8da8a-108">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="8da8a-109">权限</span><span class="sxs-lookup"><span data-stu-id="8da8a-109">Permissions</span></span>
<span data-ttu-id="8da8a-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8da8a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8da8a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="8da8a-112">Permission type</span></span>      | <span data-ttu-id="8da8a-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8da8a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8da8a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8da8a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8da8a-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8da8a-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8da8a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8da8a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8da8a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8da8a-117">Not supported.</span></span>    |
|<span data-ttu-id="8da8a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="8da8a-118">Application</span></span> | <span data-ttu-id="8da8a-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8da8a-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8da8a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8da8a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8da8a-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8da8a-121">Optional query parameters</span></span>
<span data-ttu-id="8da8a-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8da8a-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8da8a-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="8da8a-123">Request headers</span></span>
| <span data-ttu-id="8da8a-124">名称</span><span class="sxs-lookup"><span data-stu-id="8da8a-124">Name</span></span>      |<span data-ttu-id="8da8a-125">说明</span><span class="sxs-lookup"><span data-stu-id="8da8a-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8da8a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8da8a-126">Authorization</span></span>  | <span data-ttu-id="8da8a-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8da8a-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8da8a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8da8a-129">Request body</span></span>
<span data-ttu-id="8da8a-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8da8a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8da8a-131">响应</span><span class="sxs-lookup"><span data-stu-id="8da8a-131">Response</span></span>

<span data-ttu-id="8da8a-132">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[directorySettingTemplate](../resources/directorysettingtemplate.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="8da8a-132">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8da8a-133">示例</span><span class="sxs-lookup"><span data-stu-id="8da8a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8da8a-134">请求</span><span class="sxs-lookup"><span data-stu-id="8da8a-134">Request</span></span>
<span data-ttu-id="8da8a-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8da8a-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```http
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
##### <a name="response"></a><span data-ttu-id="8da8a-136">响应</span><span class="sxs-lookup"><span data-stu-id="8da8a-136">Response</span></span>
<span data-ttu-id="8da8a-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8da8a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 343

{
  "value": [
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
      ]
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8da8a-140">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="8da8a-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8da8a-141">C#</span><span class="sxs-lookup"><span data-stu-id="8da8a-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directorysettingtemplates-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8da8a-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="8da8a-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directorysettingtemplates-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8da8a-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="8da8a-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_directorysettingtemplates-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directorySettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysettingtemplate-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directorysettingtemplate-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directorysettingtemplate-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
