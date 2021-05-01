---
title: 'educationAssignment：getResourcesFolderUrl (已弃) '
description: '此函数返回 OneDrive URL，其中所有基于文件的资源 (Word、Excel 等) 上载。  '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 44c7caec25b4d96b225598041f59bfcaa3f5d3ac
ms.sourcegitcommit: 40a8e4b9e344811267025e23c372a6e60e31a1b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/01/2021
ms.locfileid: "52119003"
---
# <a name="educationassignment-getresourcesfolderurl-deprecated"></a><span data-ttu-id="982c0-103">educationAssignment：getResourcesFolderUrl (已弃) </span><span class="sxs-lookup"><span data-stu-id="982c0-103">educationAssignment: getResourcesFolderUrl (deprecated)</span></span>

<span data-ttu-id="982c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="982c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 [!CAUTION] <span data-ttu-id="982c0-105">getResourcesFolderUrl API 已弃用，将在 2021 年 5 月 31 日停止返回数据。</span><span class="sxs-lookup"><span data-stu-id="982c0-105">The getResourcesFolderUrl API is deprecated and will stop returning data on May 31, 2021.</span></span> <span data-ttu-id="982c0-106">请使用 `resourcesFolderUrl` [educationAssignment](../resources/educationassignment.md) 实体上公开的新属性获取此信息。</span><span class="sxs-lookup"><span data-stu-id="982c0-106">Please use the new property `resourcesFolderUrl` exposed on [educationAssignment](../resources/educationassignment.md) entity to fetch this info.</span></span> 

<span data-ttu-id="982c0-107">此函数返回 OneDrive URL，其中所有基于文件的资源 (Word、Excel 等) 上载。</span><span class="sxs-lookup"><span data-stu-id="982c0-107">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="982c0-108">请注意，文件必须位于此文件夹中才能添加为资源。</span><span class="sxs-lookup"><span data-stu-id="982c0-108">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="982c0-109">只有课堂中的教师可以确定要上载的文件。</span><span class="sxs-lookup"><span data-stu-id="982c0-109">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="982c0-110">权限</span><span class="sxs-lookup"><span data-stu-id="982c0-110">Permissions</span></span>
<span data-ttu-id="982c0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="982c0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="982c0-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="982c0-113">Permission type</span></span>      | <span data-ttu-id="982c0-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="982c0-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="982c0-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="982c0-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="982c0-116">EduAssignments.ReadBasic、EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="982c0-116">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="982c0-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="982c0-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="982c0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="982c0-118">Not supported.</span></span>  |
|<span data-ttu-id="982c0-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="982c0-119">Application</span></span> | <span data-ttu-id="982c0-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="982c0-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="982c0-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="982c0-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="982c0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="982c0-122">Request headers</span></span>
| <span data-ttu-id="982c0-123">标头</span><span class="sxs-lookup"><span data-stu-id="982c0-123">Header</span></span>       | <span data-ttu-id="982c0-124">值</span><span class="sxs-lookup"><span data-stu-id="982c0-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="982c0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="982c0-125">Authorization</span></span>  | <span data-ttu-id="982c0-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="982c0-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="982c0-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="982c0-128">Request body</span></span>
<span data-ttu-id="982c0-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="982c0-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="982c0-130">响应</span><span class="sxs-lookup"><span data-stu-id="982c0-130">Response</span></span>
<span data-ttu-id="982c0-131">如果成功，此方法返回 `200 Ok` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="982c0-131">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="982c0-132">正文将包含OneDrive所有基于文件的资源的文件夹的 URL。</span><span class="sxs-lookup"><span data-stu-id="982c0-132">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="982c0-133">示例</span><span class="sxs-lookup"><span data-stu-id="982c0-133">Example</span></span>
<span data-ttu-id="982c0-134">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="982c0-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="982c0-135">请求</span><span class="sxs-lookup"><span data-stu-id="982c0-135">Request</span></span>
<span data-ttu-id="982c0-136">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="982c0-136">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="982c0-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="982c0-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```
# <a name="c"></a>[<span data-ttu-id="982c0-138">C#</span><span class="sxs-lookup"><span data-stu-id="982c0-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="982c0-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="982c0-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="982c0-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="982c0-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="982c0-141">Java</span><span class="sxs-lookup"><span data-stu-id="982c0-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationassignment-publish-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="982c0-142">响应</span><span class="sxs-lookup"><span data-stu-id="982c0-142">Response</span></span>
<span data-ttu-id="982c0-143">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="982c0-143">The following is an example of a response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Edm.String",
    "value": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


