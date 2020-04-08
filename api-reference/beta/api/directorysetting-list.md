---
title: 列出目录设置
description: 检索目录设置对象的列表。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 46765047bfa5e24bb8ccd14b95986f9c3878909e
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43180782"
---
# <a name="list-directory-settings"></a><span data-ttu-id="0d7fb-103">列出目录设置</span><span class="sxs-lookup"><span data-stu-id="0d7fb-103">List directory settings</span></span>

<span data-ttu-id="0d7fb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d7fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d7fb-105">检索目录设置对象的列表。</span><span class="sxs-lookup"><span data-stu-id="0d7fb-105">Retrieve a list of directory setting objects.</span></span>

> <span data-ttu-id="0d7fb-106">**注意**：此 API 的/beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="0d7fb-106">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="0d7fb-107">此 API 的/v1.0 版本已重命名为*List groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="0d7fb-107">The /v1.0 version of this API has been renamed to *List groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d7fb-108">权限</span><span class="sxs-lookup"><span data-stu-id="0d7fb-108">Permissions</span></span>
<span data-ttu-id="0d7fb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d7fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d7fb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d7fb-111">Permission type</span></span>      | <span data-ttu-id="0d7fb-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d7fb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d7fb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d7fb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0d7fb-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0d7fb-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0d7fb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d7fb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d7fb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d7fb-116">Not supported.</span></span>    |
|<span data-ttu-id="0d7fb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d7fb-117">Application</span></span> | <span data-ttu-id="0d7fb-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d7fb-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d7fb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d7fb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="0d7fb-120">列出租户范围或组设置</span><span class="sxs-lookup"><span data-stu-id="0d7fb-120">List tenant-wide or group settings</span></span>
```http
GET /settings
GET /group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0d7fb-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0d7fb-121">Optional query parameters</span></span>
<span data-ttu-id="0d7fb-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0d7fb-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d7fb-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d7fb-123">Request headers</span></span>
| <span data-ttu-id="0d7fb-124">名称</span><span class="sxs-lookup"><span data-stu-id="0d7fb-124">Name</span></span>      |<span data-ttu-id="0d7fb-125">说明</span><span class="sxs-lookup"><span data-stu-id="0d7fb-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0d7fb-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d7fb-126">Authorization</span></span>  | <span data-ttu-id="0d7fb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0d7fb-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d7fb-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d7fb-129">Request body</span></span>
<span data-ttu-id="0d7fb-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0d7fb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d7fb-131">响应</span><span class="sxs-lookup"><span data-stu-id="0d7fb-131">Response</span></span>

<span data-ttu-id="0d7fb-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[directorySetting](../resources/directorysetting.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="0d7fb-132">If successful, this method returns a `200 OK` response code and collection of [directorySetting](../resources/directorysetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0d7fb-133">示例</span><span class="sxs-lookup"><span data-stu-id="0d7fb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d7fb-134">请求</span><span class="sxs-lookup"><span data-stu-id="0d7fb-134">Request</span></span>
<span data-ttu-id="0d7fb-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0d7fb-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0d7fb-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d7fb-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/settings
```
# <a name="c"></a>[<span data-ttu-id="0d7fb-137">C#</span><span class="sxs-lookup"><span data-stu-id="0d7fb-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d7fb-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d7fb-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d7fb-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d7fb-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0d7fb-140">响应</span><span class="sxs-lookup"><span data-stu-id="0d7fb-140">Response</span></span>
<span data-ttu-id="0d7fb-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0d7fb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
