---
title: 'educationAssignment: getResourcesFolderUrl'
description: '此函数返回 OneDrive URL 应其中上载所有基于文件的资源 （Word、 Excel 和等等）。  '
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 43bef729d2cf37561d0742ebb3adfb21fe4f486e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512029"
---
# <a name="educationassignment-getresourcesfolderurl"></a><span data-ttu-id="3bf64-103">educationAssignment: getResourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="3bf64-103">educationAssignment: getResourcesFolderUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bf64-104">此函数返回 OneDrive URL 应其中上载所有基于文件的资源 （Word、 Excel 和等等）。</span><span class="sxs-lookup"><span data-stu-id="3bf64-104">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="3bf64-105">请注意，文件必须位于此文件夹中以添加为资源。</span><span class="sxs-lookup"><span data-stu-id="3bf64-105">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="3bf64-106">仅在类中的教师可以确定要上载的文件。</span><span class="sxs-lookup"><span data-stu-id="3bf64-106">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="3bf64-107">权限</span><span class="sxs-lookup"><span data-stu-id="3bf64-107">Permissions</span></span>
<span data-ttu-id="3bf64-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3bf64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bf64-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3bf64-110">Permission type</span></span>      | <span data-ttu-id="3bf64-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3bf64-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3bf64-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3bf64-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="3bf64-113">EduAssignments.ReadBasic EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="3bf64-113">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="3bf64-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3bf64-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3bf64-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3bf64-115">Not supported.</span></span>  |
|<span data-ttu-id="3bf64-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3bf64-116">Application</span></span> | <span data-ttu-id="3bf64-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3bf64-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3bf64-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3bf64-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="3bf64-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3bf64-119">Request headers</span></span>
| <span data-ttu-id="3bf64-120">标头</span><span class="sxs-lookup"><span data-stu-id="3bf64-120">Header</span></span>       | <span data-ttu-id="3bf64-121">值</span><span class="sxs-lookup"><span data-stu-id="3bf64-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3bf64-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bf64-122">Authorization</span></span>  | <span data-ttu-id="3bf64-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3bf64-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3bf64-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3bf64-125">Request body</span></span>
<span data-ttu-id="3bf64-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3bf64-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3bf64-127">响应</span><span class="sxs-lookup"><span data-stu-id="3bf64-127">Response</span></span>
<span data-ttu-id="3bf64-128">如果成功，此方法返回 `200 Ok` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="3bf64-128">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="3bf64-129">正文将包含在其中放入所有基于文件的资源文件夹的 OneDrive URL。</span><span class="sxs-lookup"><span data-stu-id="3bf64-129">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="3bf64-130">示例</span><span class="sxs-lookup"><span data-stu-id="3bf64-130">Example</span></span>
<span data-ttu-id="3bf64-131">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="3bf64-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3bf64-132">请求</span><span class="sxs-lookup"><span data-stu-id="3bf64-132">Request</span></span>
<span data-ttu-id="3bf64-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3bf64-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```

##### <a name="response"></a><span data-ttu-id="3bf64-134">响应</span><span class="sxs-lookup"><span data-stu-id="3bf64-134">Response</span></span>
<span data-ttu-id="3bf64-135">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="3bf64-135">The following is an example of a response.</span></span> 

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
    "Error: /api-reference/beta/api/educationassignment-getresourcesfolderurl.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
