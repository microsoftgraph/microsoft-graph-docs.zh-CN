---
title: 'educationAssignment: getResourcesFolderUrl'
description: '此函数返回您应上载所有基于文件的资源 (Word、Excel 等) 的 OneDrive URL。  '
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: a0165b61af2d5ad07bb9eea6309bd6c899e6f34c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325121"
---
# <a name="educationassignment-getresourcesfolderurl"></a><span data-ttu-id="3157b-103">educationAssignment: getResourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="3157b-103">educationAssignment: getResourcesFolderUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3157b-104">此函数返回您应上载所有基于文件的资源 (Word、Excel 等) 的 OneDrive URL。</span><span class="sxs-lookup"><span data-stu-id="3157b-104">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="3157b-105">请注意, 文件必须位于此文件夹中才能作为资源添加。</span><span class="sxs-lookup"><span data-stu-id="3157b-105">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="3157b-106">只有课堂中的老师可以确定要上载的文件。</span><span class="sxs-lookup"><span data-stu-id="3157b-106">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="3157b-107">权限</span><span class="sxs-lookup"><span data-stu-id="3157b-107">Permissions</span></span>
<span data-ttu-id="3157b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3157b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3157b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3157b-110">Permission type</span></span>      | <span data-ttu-id="3157b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3157b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3157b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3157b-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="3157b-113">EduAssignments、user.readbasic.all、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="3157b-113">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="3157b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3157b-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3157b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3157b-115">Not supported.</span></span>  |
|<span data-ttu-id="3157b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3157b-116">Application</span></span> | <span data-ttu-id="3157b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3157b-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3157b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3157b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="3157b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3157b-119">Request headers</span></span>
| <span data-ttu-id="3157b-120">标头</span><span class="sxs-lookup"><span data-stu-id="3157b-120">Header</span></span>       | <span data-ttu-id="3157b-121">值</span><span class="sxs-lookup"><span data-stu-id="3157b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3157b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3157b-122">Authorization</span></span>  | <span data-ttu-id="3157b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3157b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3157b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3157b-125">Request body</span></span>
<span data-ttu-id="3157b-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3157b-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3157b-127">响应</span><span class="sxs-lookup"><span data-stu-id="3157b-127">Response</span></span>
<span data-ttu-id="3157b-128">如果成功，此方法返回 `200 Ok` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="3157b-128">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="3157b-129">正文将包含要在其中放置所有基于文件的资源的文件夹的 OneDrive URL。</span><span class="sxs-lookup"><span data-stu-id="3157b-129">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="3157b-130">示例</span><span class="sxs-lookup"><span data-stu-id="3157b-130">Example</span></span>
<span data-ttu-id="3157b-131">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="3157b-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3157b-132">请求</span><span class="sxs-lookup"><span data-stu-id="3157b-132">Request</span></span>
<span data-ttu-id="3157b-133">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="3157b-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```

##### <a name="response"></a><span data-ttu-id="3157b-134">响应</span><span class="sxs-lookup"><span data-stu-id="3157b-134">Response</span></span>
<span data-ttu-id="3157b-135">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="3157b-135">The following is an example of a response.</span></span> 

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
  "suppressions": []
}
-->
