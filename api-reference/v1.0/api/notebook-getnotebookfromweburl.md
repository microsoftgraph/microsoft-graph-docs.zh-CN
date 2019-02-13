---
title: 笔记本： getNotebookFromWebUrl
description: 检索的属性和使用其 URL 路径笔记本对象的关系。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 3d14edf5a8992f9f4386e4b50aa74d54986b62f1
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/13/2019
ms.locfileid: "29982060"
---
# <a name="notebook-getnotebookfromweburl"></a><span data-ttu-id="54b4d-103">笔记本： getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="54b4d-103">notebook: getNotebookFromWebUrl</span></span>

<span data-ttu-id="54b4d-104">通过使用其 URL 路径中检索的属性和[笔记本](../resources/notebook.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="54b4d-104">Retrieve the properties and relationships of a [notebook](../resources/notebook.md) object by using its URL path.</span></span>

<span data-ttu-id="54b4d-105">位置可以是用户在 Office 365、 组笔记本或在 Office 365 上的 SharePoint 网站承载团队笔记本的笔记本。</span><span class="sxs-lookup"><span data-stu-id="54b4d-105">The location can be user notebooks on Office 365, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span>
## <a name="permissions"></a><span data-ttu-id="54b4d-106">权限</span><span class="sxs-lookup"><span data-stu-id="54b4d-106">Permissions</span></span>
<span data-ttu-id="54b4d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="54b4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54b4d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="54b4d-109">Permission type</span></span>      | <span data-ttu-id="54b4d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="54b4d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54b4d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54b4d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="54b4d-112">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54b4d-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="54b4d-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="54b4d-113">Application</span></span> | <span data-ttu-id="54b4d-114">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54b4d-114">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="54b4d-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54b4d-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/GetNotebookFromWebUrl
POST /users/{id | userPrincipalName}/onenote/notebooks/GetNotebookFromWebUrl
POST /groups/{id}/onenote/notebooks/GetNotebookFromWebUrl
POST /sites/{id}/onenote/notebooks/GetNotebookFromWebUrl
```
## <a name="request-headers"></a><span data-ttu-id="54b4d-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="54b4d-116">Request headers</span></span>
| <span data-ttu-id="54b4d-117">Name</span><span class="sxs-lookup"><span data-stu-id="54b4d-117">Name</span></span>       | <span data-ttu-id="54b4d-118">类型</span><span class="sxs-lookup"><span data-stu-id="54b4d-118">Type</span></span> | <span data-ttu-id="54b4d-119">说明</span><span class="sxs-lookup"><span data-stu-id="54b4d-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="54b4d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="54b4d-120">Authorization</span></span>  | <span data-ttu-id="54b4d-121">字符串</span><span class="sxs-lookup"><span data-stu-id="54b4d-121">string</span></span>  | <span data-ttu-id="54b4d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="54b4d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="54b4d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="54b4d-124">Accept</span></span> | <span data-ttu-id="54b4d-125">string</span><span class="sxs-lookup"><span data-stu-id="54b4d-125">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="54b4d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="54b4d-126">Request body</span></span>
<span data-ttu-id="54b4d-127">在请求正文中，提供要检索的笔记本的完整 URL 路径的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54b4d-127">In the request body, supply a JSON representation of the full URL path to the notebook you want to retrieve.</span></span>

| <span data-ttu-id="54b4d-128">属性</span><span class="sxs-lookup"><span data-stu-id="54b4d-128">Property</span></span>     | <span data-ttu-id="54b4d-129">类型</span><span class="sxs-lookup"><span data-stu-id="54b4d-129">Type</span></span>        | <span data-ttu-id="54b4d-130">说明</span><span class="sxs-lookup"><span data-stu-id="54b4d-130">Description</span></span> |
|:-------------|:------------|:------------|
| `webUrl`     |`String`     | <span data-ttu-id="54b4d-131">若要检索的笔记本 URL 路径。</span><span class="sxs-lookup"><span data-stu-id="54b4d-131">The URL path of the notebook to retrieve.</span></span> <span data-ttu-id="54b4d-132">它还可以包含"onenote:"前缀。</span><span class="sxs-lookup"><span data-stu-id="54b4d-132">It can also contain a "onenote:" prefix.</span></span>|

## <a name="response"></a><span data-ttu-id="54b4d-133">响应</span><span class="sxs-lookup"><span data-stu-id="54b4d-133">Response</span></span>

<span data-ttu-id="54b4d-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [notebook](../resources/notebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="54b4d-134">If successful, this method returns a `200 OK` response code and a [notebook](../resources/notebook.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="54b4d-135">示例</span><span class="sxs-lookup"><span data-stu-id="54b4d-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54b4d-136">请求</span><span class="sxs-lookup"><span data-stu-id="54b4d-136">Request</span></span>
<span data-ttu-id="54b4d-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="54b4d-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_fromweburl"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/GetNotebookFromWebUrl
Content-type: application/json

{"webUrl":"webUrl value"}
```
##### <a name="response"></a><span data-ttu-id="54b4d-138">响应</span><span class="sxs-lookup"><span data-stu-id="54b4d-138">Response</span></span>
<span data-ttu-id="54b4d-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="54b4d-139">Here is an example of the response.</span></span> 

><span data-ttu-id="54b4d-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="54b4d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
