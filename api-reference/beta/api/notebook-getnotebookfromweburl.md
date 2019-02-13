---
title: 笔记本： getNotebookFromWebUrl
description: 检索的属性和使用其 URL 路径笔记本对象的关系。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 226cbd70343feaf8fe5404aac6077f9b2438aba8
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/13/2019
ms.locfileid: "29982067"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="20019-103">笔记本： getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="20019-103">notebook: getNotebookFromWebUrl</span></span>

[!包括 beta 免责声明]

<span data-ttu-id="20019-105">通过使用其 URL 路径中检索的属性和[笔记本](../resources/notebook.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="20019-105">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="20019-106">位置可以是用户在 Office 365、 组笔记本或在 Office 365 上的 SharePoint 网站承载团队笔记本的笔记本。</span><span class="sxs-lookup"><span data-stu-id="20019-106">The location can be user notebooks on Office 365, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="20019-107">权限</span><span class="sxs-lookup"><span data-stu-id="20019-107">Permissions</span></span>
<span data-ttu-id="20019-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20019-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20019-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="20019-110">Permission type</span></span>      | <span data-ttu-id="20019-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="20019-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20019-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20019-112">Delegated (work or school account)</span></span> | <span data-ttu-id="20019-113">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20019-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="20019-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="20019-114">Application</span></span> | <span data-ttu-id="20019-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20019-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20019-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20019-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="20019-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="20019-117">Request headers</span></span>
| <span data-ttu-id="20019-118">Name</span><span class="sxs-lookup"><span data-stu-id="20019-118">Name</span></span>       | <span data-ttu-id="20019-119">类型</span><span class="sxs-lookup"><span data-stu-id="20019-119">Type</span></span> | <span data-ttu-id="20019-120">说明</span><span class="sxs-lookup"><span data-stu-id="20019-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="20019-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="20019-121">Authorization</span></span>  | <span data-ttu-id="20019-122">字符串</span><span class="sxs-lookup"><span data-stu-id="20019-122">string</span></span>  | <span data-ttu-id="20019-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="20019-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20019-125">Accept</span><span class="sxs-lookup"><span data-stu-id="20019-125">Accept</span></span> | <span data-ttu-id="20019-126">string</span><span class="sxs-lookup"><span data-stu-id="20019-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="20019-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="20019-127">Request body</span></span>
<span data-ttu-id="20019-128">在请求正文中，提供要检索的笔记本的完整 URL 路径的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20019-128">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="20019-129">属性</span><span class="sxs-lookup"><span data-stu-id="20019-129">Property</span></span>     | <span data-ttu-id="20019-130">类型</span><span class="sxs-lookup"><span data-stu-id="20019-130">Type</span></span>        | <span data-ttu-id="20019-131">说明</span><span class="sxs-lookup"><span data-stu-id="20019-131">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="20019-132">若要检索的笔记本 URL 路径。</span><span class="sxs-lookup"><span data-stu-id="20019-132">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="20019-133">它还可以包含"onenote:"前缀。</span><span class="sxs-lookup"><span data-stu-id="20019-133">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="20019-134">响应</span><span class="sxs-lookup"><span data-stu-id="20019-134">Response</span></span>

<span data-ttu-id="20019-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [notebook](../resources/notebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="20019-135">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="20019-136">示例</span><span class="sxs-lookup"><span data-stu-id="20019-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20019-137">请求</span><span class="sxs-lookup"><span data-stu-id="20019-137">Request</span></span>
<span data-ttu-id="20019-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="20019-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
##### <a name="response"></a><span data-ttu-id="20019-139">响应</span><span class="sxs-lookup"><span data-stu-id="20019-139">Response</span></span>
<span data-ttu-id="20019-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="20019-140">Here is an example of the response.</span></span> 

><span data-ttu-id="20019-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="20019-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json; odata.metadata=minimal
Content-Length: 544

{
    "isDefault": true,
    "userRole": "userRole-value",
    "isShared": true,
    "sectionsUrl": "sectionUrl-value",
    "sectionGroupsUrl": "sectionGroupUrl-value",
    "links": {
        "oneNoteClientUrl": {
            "href": "href-value"
        },
        "oneNoteWebUrl": {
            "href": "href-value"
        }
    },
    "id": "id-value",
    "self": "self-value",
}
```
<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error:{notebook-getnotebookfromweburl.md}:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
