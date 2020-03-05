---
title: 获取目录设置
description: 检索特定目录设置对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: df98499099bb26cc0d50564ecaf4a9aa556313f6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42433991"
---
# <a name="get-a-directory-setting"></a><span data-ttu-id="1b8ee-103">获取目录设置</span><span class="sxs-lookup"><span data-stu-id="1b8ee-103">Get a directory setting</span></span>

<span data-ttu-id="1b8ee-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1b8ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b8ee-105">检索特定目录设置对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1b8ee-105">Retrieve the properties of a specific directory setting object.</span></span>

> <span data-ttu-id="1b8ee-106">**注意**：此 API 的/beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="1b8ee-106">**Note**: The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="1b8ee-107">此 API 的/v1.0 版本已重命名为*Get groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="1b8ee-107">The /v1.0 version of this API has been renamed to *Get groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b8ee-108">权限</span><span class="sxs-lookup"><span data-stu-id="1b8ee-108">Permissions</span></span>
<span data-ttu-id="1b8ee-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b8ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b8ee-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b8ee-111">Permission type</span></span>      | <span data-ttu-id="1b8ee-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1b8ee-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b8ee-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b8ee-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1b8ee-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1b8ee-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1b8ee-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b8ee-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b8ee-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b8ee-116">Not supported.</span></span>    |
|<span data-ttu-id="1b8ee-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b8ee-117">Application</span></span> | <span data-ttu-id="1b8ee-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b8ee-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b8ee-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b8ee-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="1b8ee-120">获取特定的租户范围或组设置</span><span class="sxs-lookup"><span data-stu-id="1b8ee-120">Get a specific tenant-wide or group setting</span></span>
```http
GET /settings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1b8ee-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1b8ee-121">Optional query parameters</span></span>
<span data-ttu-id="1b8ee-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1b8ee-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b8ee-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b8ee-123">Request headers</span></span>
| <span data-ttu-id="1b8ee-124">名称</span><span class="sxs-lookup"><span data-stu-id="1b8ee-124">Name</span></span>      |<span data-ttu-id="1b8ee-125">说明</span><span class="sxs-lookup"><span data-stu-id="1b8ee-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1b8ee-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b8ee-126">Authorization</span></span>  | <span data-ttu-id="1b8ee-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1b8ee-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b8ee-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="1b8ee-129">Request body</span></span>
<span data-ttu-id="1b8ee-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1b8ee-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b8ee-131">响应</span><span class="sxs-lookup"><span data-stu-id="1b8ee-131">Response</span></span>

<span data-ttu-id="1b8ee-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[directorySetting](../resources/directorysetting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1b8ee-132">If successful, this method returns a `200 OK` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1b8ee-133">示例</span><span class="sxs-lookup"><span data-stu-id="1b8ee-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b8ee-134">请求</span><span class="sxs-lookup"><span data-stu-id="1b8ee-134">Request</span></span>
<span data-ttu-id="1b8ee-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1b8ee-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1b8ee-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b8ee-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/settings/{id}
```
# <a name="c"></a>[<span data-ttu-id="1b8ee-137">C#</span><span class="sxs-lookup"><span data-stu-id="1b8ee-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b8ee-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b8ee-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b8ee-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b8ee-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1b8ee-140">响应</span><span class="sxs-lookup"><span data-stu-id="1b8ee-140">Response</span></span>
<span data-ttu-id="1b8ee-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1b8ee-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
