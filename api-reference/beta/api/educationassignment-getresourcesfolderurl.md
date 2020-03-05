---
title: educationAssignment： getResourcesFolderUrl
description: '此函数返回您应上载所有基于文件的资源（Word、Excel 等）的 OneDrive URL。  '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d7520db351be8d9b78506354e14988bd479fda92
ms.sourcegitcommit: fc818699566f03493937be95447eb9f656a1f950
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534413"
---
# <a name="educationassignment-getresourcesfolderurl"></a><span data-ttu-id="de3f1-103">educationAssignment： getResourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="de3f1-103">educationAssignment: getResourcesFolderUrl</span></span>

<span data-ttu-id="de3f1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="de3f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de3f1-105">此函数返回您应上载所有基于文件的资源（Word、Excel 等）的 OneDrive URL。</span><span class="sxs-lookup"><span data-stu-id="de3f1-105">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="de3f1-106">请注意，文件必须位于此文件夹中才能作为资源添加。</span><span class="sxs-lookup"><span data-stu-id="de3f1-106">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="de3f1-107">只有课堂中的老师可以确定要上载的文件。</span><span class="sxs-lookup"><span data-stu-id="de3f1-107">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="de3f1-108">权限</span><span class="sxs-lookup"><span data-stu-id="de3f1-108">Permissions</span></span>
<span data-ttu-id="de3f1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de3f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de3f1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="de3f1-111">Permission type</span></span>      | <span data-ttu-id="de3f1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="de3f1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de3f1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de3f1-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="de3f1-114">EduAssignments、User.readbasic.all、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="de3f1-114">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="de3f1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de3f1-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="de3f1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="de3f1-116">Not supported.</span></span>  |
|<span data-ttu-id="de3f1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="de3f1-117">Application</span></span> | <span data-ttu-id="de3f1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="de3f1-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="de3f1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de3f1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="de3f1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="de3f1-120">Request headers</span></span>
| <span data-ttu-id="de3f1-121">标头</span><span class="sxs-lookup"><span data-stu-id="de3f1-121">Header</span></span>       | <span data-ttu-id="de3f1-122">值</span><span class="sxs-lookup"><span data-stu-id="de3f1-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="de3f1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="de3f1-123">Authorization</span></span>  | <span data-ttu-id="de3f1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="de3f1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="de3f1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="de3f1-126">Request body</span></span>
<span data-ttu-id="de3f1-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="de3f1-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="de3f1-128">响应</span><span class="sxs-lookup"><span data-stu-id="de3f1-128">Response</span></span>
<span data-ttu-id="de3f1-129">如果成功，此方法返回 `200 Ok` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="de3f1-129">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="de3f1-130">正文将包含要在其中放置所有基于文件的资源的文件夹的 OneDrive URL。</span><span class="sxs-lookup"><span data-stu-id="de3f1-130">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="de3f1-131">示例</span><span class="sxs-lookup"><span data-stu-id="de3f1-131">Example</span></span>
<span data-ttu-id="de3f1-132">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="de3f1-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="de3f1-133">请求</span><span class="sxs-lookup"><span data-stu-id="de3f1-133">Request</span></span>
<span data-ttu-id="de3f1-134">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="de3f1-134">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="de3f1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="de3f1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```
# <a name="c"></a>[<span data-ttu-id="de3f1-136">C#</span><span class="sxs-lookup"><span data-stu-id="de3f1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de3f1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de3f1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de3f1-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de3f1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="de3f1-139">响应</span><span class="sxs-lookup"><span data-stu-id="de3f1-139">Response</span></span>
<span data-ttu-id="de3f1-140">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="de3f1-140">The following is an example of a response.</span></span> 

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
