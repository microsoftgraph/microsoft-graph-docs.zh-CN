---
title: 列出 directorySettingTemplates
description: 此操作检索可用 directorySettingTemplates 对象的列表。
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 13462b4a4d980d42667fee1252c8ded94b0a7ea8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436601"
---
# <a name="list-directorysettingtemplates"></a><span data-ttu-id="bc97b-103">列出 directorySettingTemplates</span><span class="sxs-lookup"><span data-stu-id="bc97b-103">List directorySettingTemplates</span></span>

<span data-ttu-id="bc97b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc97b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc97b-105">目录设置模板表示目录设置的一组模板，可以在租户中创建和使用的目录设置。</span><span class="sxs-lookup"><span data-stu-id="bc97b-105">Directory setting templates represents a set of templates of directory settings, from which directory settings may be created and used within a tenant.</span></span>  <span data-ttu-id="bc97b-106">此操作检索可用 **directorySettingTemplates 对象** 的列表。</span><span class="sxs-lookup"><span data-stu-id="bc97b-106">This operation retrieves the list of available **directorySettingTemplates** objects.</span></span>

> <span data-ttu-id="bc97b-107">**注意**：此 API 的 /beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="bc97b-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="bc97b-108">此 API 的 /v1.0 版本已重命名为 *List groupSettingTemplate。*</span><span class="sxs-lookup"><span data-stu-id="bc97b-108">The /v1.0 version of this API has been renamed to *List groupSettingTemplate*.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc97b-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="bc97b-109">Permissions</span></span>
<span data-ttu-id="bc97b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bc97b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc97b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc97b-112">Permission type</span></span>      | <span data-ttu-id="bc97b-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bc97b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc97b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc97b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="bc97b-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bc97b-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bc97b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc97b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc97b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc97b-117">Not supported.</span></span>    |
|<span data-ttu-id="bc97b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc97b-118">Application</span></span> | <span data-ttu-id="bc97b-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc97b-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc97b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc97b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directorySettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bc97b-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bc97b-121">Optional query parameters</span></span>
<span data-ttu-id="bc97b-122">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bc97b-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc97b-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc97b-123">Request headers</span></span>
| <span data-ttu-id="bc97b-124">名称</span><span class="sxs-lookup"><span data-stu-id="bc97b-124">Name</span></span>      |<span data-ttu-id="bc97b-125">说明</span><span class="sxs-lookup"><span data-stu-id="bc97b-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bc97b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc97b-126">Authorization</span></span>  | <span data-ttu-id="bc97b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bc97b-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc97b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc97b-129">Request body</span></span>
<span data-ttu-id="bc97b-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bc97b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc97b-131">响应</span><span class="sxs-lookup"><span data-stu-id="bc97b-131">Response</span></span>

<span data-ttu-id="bc97b-132">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [directorySettingTemplate](../resources/directorysettingtemplate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bc97b-132">If successful, this method returns a `200 OK` response code and collection of [directorySettingTemplate](../resources/directorysettingtemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bc97b-133">示例</span><span class="sxs-lookup"><span data-stu-id="bc97b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc97b-134">请求</span><span class="sxs-lookup"><span data-stu-id="bc97b-134">Request</span></span>
<span data-ttu-id="bc97b-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bc97b-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bc97b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc97b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directorysettingtemplates"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directorySettingTemplates
```
# <a name="c"></a>[<span data-ttu-id="bc97b-137">C#</span><span class="sxs-lookup"><span data-stu-id="bc97b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directorysettingtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc97b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc97b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directorysettingtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc97b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc97b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directorysettingtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bc97b-140">Java</span><span class="sxs-lookup"><span data-stu-id="bc97b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directorysettingtemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bc97b-141">响应</span><span class="sxs-lookup"><span data-stu-id="bc97b-141">Response</span></span>
<span data-ttu-id="bc97b-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bc97b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->


