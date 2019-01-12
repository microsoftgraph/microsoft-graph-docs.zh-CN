---
title: 'notebook: copyNotebook'
description: 将笔记本复制到目标文档库中的 Notebooks 文件夹。如果该文件夹不存在，则将创建该文件夹。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: aa684dcaa01f2a8c16be1c75a7b973ee8adb8eea
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972927"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="91a31-104">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="91a31-104">notebook: copyNotebook</span></span>
<span data-ttu-id="91a31-p102">将笔记本复制到目标文档库中的 Notebooks 文件夹。如果该文件夹不存在，则将创建该文件夹。</span><span class="sxs-lookup"><span data-stu-id="91a31-p102">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="91a31-107">对于 Copy 操作，请遵循异步调用模式：首先调用 Copy 操作，然后轮询该操作终结点获取结果。</span><span class="sxs-lookup"><span data-stu-id="91a31-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="91a31-108">权限</span><span class="sxs-lookup"><span data-stu-id="91a31-108">Permissions</span></span>
<span data-ttu-id="91a31-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="91a31-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91a31-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="91a31-111">Permission type</span></span>      | <span data-ttu-id="91a31-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="91a31-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91a31-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91a31-113">Delegated (work or school account)</span></span> | <span data-ttu-id="91a31-114">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91a31-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="91a31-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91a31-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91a31-116">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91a31-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="91a31-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="91a31-117">Application</span></span> | <span data-ttu-id="91a31-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91a31-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91a31-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91a31-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="91a31-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="91a31-120">Request headers</span></span>
| <span data-ttu-id="91a31-121">名称</span><span class="sxs-lookup"><span data-stu-id="91a31-121">Name</span></span>       | <span data-ttu-id="91a31-122">类型</span><span class="sxs-lookup"><span data-stu-id="91a31-122">Type</span></span> | <span data-ttu-id="91a31-123">说明</span><span class="sxs-lookup"><span data-stu-id="91a31-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="91a31-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="91a31-124">Authorization</span></span>  | <span data-ttu-id="91a31-125">string</span><span class="sxs-lookup"><span data-stu-id="91a31-125">string</span></span>  | <span data-ttu-id="91a31-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="91a31-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="91a31-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91a31-128">Content-Type</span></span> | <span data-ttu-id="91a31-129">string</span><span class="sxs-lookup"><span data-stu-id="91a31-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="91a31-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="91a31-130">Request body</span></span>
<span data-ttu-id="91a31-p105">在请求正文中，提供包含操作所需参数的 JSON 对象。如果无需任何参数，则可以发送空的正文。</span><span class="sxs-lookup"><span data-stu-id="91a31-p105">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="91a31-133">参数</span><span class="sxs-lookup"><span data-stu-id="91a31-133">Parameter</span></span>    | <span data-ttu-id="91a31-134">类型</span><span class="sxs-lookup"><span data-stu-id="91a31-134">Type</span></span>   |<span data-ttu-id="91a31-135">说明</span><span class="sxs-lookup"><span data-stu-id="91a31-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91a31-136">groupId</span><span class="sxs-lookup"><span data-stu-id="91a31-136">groupId</span></span>|<span data-ttu-id="91a31-137">字符串</span><span class="sxs-lookup"><span data-stu-id="91a31-137">String</span></span>|<span data-ttu-id="91a31-p106">要复制到的组的 ID。仅在复制到 Office 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="91a31-p106">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="91a31-140">renameAs</span><span class="sxs-lookup"><span data-stu-id="91a31-140">renameAs</span></span>|<span data-ttu-id="91a31-141">字符串</span><span class="sxs-lookup"><span data-stu-id="91a31-141">String</span></span>|<span data-ttu-id="91a31-p107">副本的名称。默认为现有项的名称。</span><span class="sxs-lookup"><span data-stu-id="91a31-p107">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="91a31-144">响应</span><span class="sxs-lookup"><span data-stu-id="91a31-144">Response</span></span>

<span data-ttu-id="91a31-p108">如果成功，此方法返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。轮询 Operation-Location 终结点以[获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="91a31-p108">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="91a31-147">示例</span><span class="sxs-lookup"><span data-stu-id="91a31-147">Example</span></span>
<span data-ttu-id="91a31-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="91a31-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="91a31-149">请求</span><span class="sxs-lookup"><span data-stu-id="91a31-149">Request</span></span>
<span data-ttu-id="91a31-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="91a31-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="91a31-151">响应</span><span class="sxs-lookup"><span data-stu-id="91a31-151">Response</span></span>
<span data-ttu-id="91a31-152">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="91a31-152">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
