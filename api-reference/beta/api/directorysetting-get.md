---
title: 获取目录设置
description: 检索特定目录设置对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0f90b9511b86e4c1c30b26bc66e97d19f433231e
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655850"
---
# <a name="get-a-directory-setting"></a><span data-ttu-id="d8582-103">获取目录设置</span><span class="sxs-lookup"><span data-stu-id="d8582-103">Get a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8582-104">检索特定目录设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d8582-104">Retrieve the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="d8582-105">**注意**: 此 API 的/beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="d8582-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="d8582-106">此 API 的/v1.0 版本已重命名为*Get groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="d8582-106">The /v1.0 version of this API has been renamed to *Get groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8582-107">权限</span><span class="sxs-lookup"><span data-stu-id="d8582-107">Permissions</span></span>
<span data-ttu-id="d8582-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8582-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8582-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8582-110">Permission type</span></span>      | <span data-ttu-id="d8582-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d8582-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8582-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8582-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d8582-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d8582-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d8582-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8582-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8582-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8582-115">Not supported.</span></span>    |
|<span data-ttu-id="d8582-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8582-116">Application</span></span> | <span data-ttu-id="d8582-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8582-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8582-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8582-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="d8582-119">获取特定的租户范围或组设置</span><span class="sxs-lookup"><span data-stu-id="d8582-119">Get a specific tenant-wide or group setting</span></span>
```http
GET /settings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d8582-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d8582-120">Optional query parameters</span></span>
<span data-ttu-id="d8582-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d8582-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d8582-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8582-122">Request headers</span></span>
| <span data-ttu-id="d8582-123">名称</span><span class="sxs-lookup"><span data-stu-id="d8582-123">Name</span></span>      |<span data-ttu-id="d8582-124">说明</span><span class="sxs-lookup"><span data-stu-id="d8582-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d8582-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8582-125">Authorization</span></span>  | <span data-ttu-id="d8582-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d8582-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8582-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8582-128">Request body</span></span>
<span data-ttu-id="d8582-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d8582-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8582-130">响应</span><span class="sxs-lookup"><span data-stu-id="d8582-130">Response</span></span>

<span data-ttu-id="d8582-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[directorySetting](../resources/directorysetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d8582-131">If successful, this method returns a `200 OK` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d8582-132">示例</span><span class="sxs-lookup"><span data-stu-id="d8582-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d8582-133">请求</span><span class="sxs-lookup"><span data-stu-id="d8582-133">Request</span></span>
<span data-ttu-id="d8582-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d8582-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}-->
```http
GET https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="d8582-135">响应</span><span class="sxs-lookup"><span data-stu-id="d8582-135">Response</span></span>
<span data-ttu-id="d8582-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d8582-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 198

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
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d8582-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d8582-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d8582-140">C#</span><span class="sxs-lookup"><span data-stu-id="d8582-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directorysetting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d8582-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="d8582-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directorysetting-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directorysetting-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
