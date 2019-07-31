---
title: 列出目录设置
description: 检索目录设置对象的列表。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9475acfdbe802978a513481a47ccc2973ae89542
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957575"
---
# <a name="list-directory-settings"></a><span data-ttu-id="7a450-103">列出目录设置</span><span class="sxs-lookup"><span data-stu-id="7a450-103">List directory settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a450-104">检索目录设置对象的列表。</span><span class="sxs-lookup"><span data-stu-id="7a450-104">Retrieve a list of directory setting objects.</span></span>

> <span data-ttu-id="7a450-105">**注意**: 此 API 的/beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="7a450-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="7a450-106">此 API 的/v1.0 版本已重命名为*List groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="7a450-106">The /v1.0 version of this API has been renamed to *List groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a450-107">权限</span><span class="sxs-lookup"><span data-stu-id="7a450-107">Permissions</span></span>
<span data-ttu-id="7a450-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7a450-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a450-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7a450-110">Permission type</span></span>      | <span data-ttu-id="7a450-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7a450-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a450-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7a450-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7a450-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7a450-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7a450-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7a450-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a450-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a450-115">Not supported.</span></span>    |
|<span data-ttu-id="7a450-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7a450-116">Application</span></span> | <span data-ttu-id="7a450-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a450-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a450-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7a450-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="7a450-119">列出租户范围或组设置</span><span class="sxs-lookup"><span data-stu-id="7a450-119">List tenant-wide or group settings</span></span>
```http
GET /settings
GET /group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7a450-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7a450-120">Optional query parameters</span></span>
<span data-ttu-id="7a450-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7a450-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a450-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="7a450-122">Request headers</span></span>
| <span data-ttu-id="7a450-123">名称</span><span class="sxs-lookup"><span data-stu-id="7a450-123">Name</span></span>      |<span data-ttu-id="7a450-124">说明</span><span class="sxs-lookup"><span data-stu-id="7a450-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7a450-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a450-125">Authorization</span></span>  | <span data-ttu-id="7a450-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7a450-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a450-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="7a450-128">Request body</span></span>
<span data-ttu-id="7a450-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7a450-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a450-130">响应</span><span class="sxs-lookup"><span data-stu-id="7a450-130">Response</span></span>

<span data-ttu-id="7a450-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[directorySetting](../resources/directorysetting.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="7a450-131">If successful, this method returns a `200 OK` response code and collection of [directorySetting](../resources/directorysetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7a450-132">示例</span><span class="sxs-lookup"><span data-stu-id="7a450-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a450-133">请求</span><span class="sxs-lookup"><span data-stu-id="7a450-133">Request</span></span>
<span data-ttu-id="7a450-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7a450-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7a450-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="7a450-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->
```http
GET https://graph.microsoft.com/beta/settings
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7a450-136">C#</span><span class="sxs-lookup"><span data-stu-id="7a450-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7a450-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="7a450-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7a450-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="7a450-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7a450-139">Java</span><span class="sxs-lookup"><span data-stu-id="7a450-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7a450-140">响应</span><span class="sxs-lookup"><span data-stu-id="7a450-140">Response</span></span>
<span data-ttu-id="7a450-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7a450-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
