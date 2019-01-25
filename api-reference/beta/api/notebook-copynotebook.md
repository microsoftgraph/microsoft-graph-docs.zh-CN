---
title: 'notebook: copyNotebook'
description: 将笔记本复制到目标文档库中的 Notebooks 文件夹。如果该文件夹不存在，则将创建该文件夹。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7100d768fb411aeab8ccbd0622de26aeae8a7133
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515599"
---
# <a name="notebook-copynotebook"></a><span data-ttu-id="b4ad8-104">notebook: copyNotebook</span><span class="sxs-lookup"><span data-stu-id="b4ad8-104">notebook: copyNotebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4ad8-p102">将笔记本复制到目标文档库中的 Notebooks 文件夹。如果该文件夹不存在，则将创建该文件夹。</span><span class="sxs-lookup"><span data-stu-id="b4ad8-p102">Copies a notebook to the Notebooks folder in the destination Documents library. The folder is created if it doesn't exist.</span></span>

<span data-ttu-id="b4ad8-107">对于 Copy 操作，请遵循异步调用模式：首先调用 Copy 操作，然后轮询该操作终结点获取结果。</span><span class="sxs-lookup"><span data-stu-id="b4ad8-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4ad8-108">权限</span><span class="sxs-lookup"><span data-stu-id="b4ad8-108">Permissions</span></span>
<span data-ttu-id="b4ad8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4ad8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4ad8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4ad8-111">Permission type</span></span>      | <span data-ttu-id="b4ad8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4ad8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4ad8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4ad8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b4ad8-114">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4ad8-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b4ad8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4ad8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4ad8-116">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4ad8-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b4ad8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4ad8-117">Application</span></span> | <span data-ttu-id="b4ad8-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4ad8-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4ad8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4ad8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/notebooks/{id}/copyNotebook
POST /users/{id | userPrincipalName}/onenote/notebooks/{id}/copyNotebook
POST /groups/{id}/onenote/notebooks/{id}/copyNotebook
POST /sites/{id}/onenote/notebooks/{id}/copyNotebook
```
## <a name="request-headers"></a><span data-ttu-id="b4ad8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4ad8-120">Request headers</span></span>
| <span data-ttu-id="b4ad8-121">名称</span><span class="sxs-lookup"><span data-stu-id="b4ad8-121">Name</span></span>       | <span data-ttu-id="b4ad8-122">类型</span><span class="sxs-lookup"><span data-stu-id="b4ad8-122">Type</span></span> | <span data-ttu-id="b4ad8-123">说明</span><span class="sxs-lookup"><span data-stu-id="b4ad8-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b4ad8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4ad8-124">Authorization</span></span>  | <span data-ttu-id="b4ad8-125">string</span><span class="sxs-lookup"><span data-stu-id="b4ad8-125">string</span></span>  | <span data-ttu-id="b4ad8-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4ad8-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b4ad8-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b4ad8-128">Content-Type</span></span> | <span data-ttu-id="b4ad8-129">string</span><span class="sxs-lookup"><span data-stu-id="b4ad8-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b4ad8-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4ad8-130">Request body</span></span>
<span data-ttu-id="b4ad8-p105">在请求正文中，提供包含操作所需参数的 JSON 对象。如果无需任何参数，则可以发送空的正文。</span><span class="sxs-lookup"><span data-stu-id="b4ad8-p105">In the request body, provide a JSON object that contains the parameters that your operation needs. It's okay to send an empty body if none are needed.</span></span>

| <span data-ttu-id="b4ad8-133">参数</span><span class="sxs-lookup"><span data-stu-id="b4ad8-133">Parameter</span></span>    | <span data-ttu-id="b4ad8-134">类型</span><span class="sxs-lookup"><span data-stu-id="b4ad8-134">Type</span></span>   |<span data-ttu-id="b4ad8-135">说明</span><span class="sxs-lookup"><span data-stu-id="b4ad8-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4ad8-136">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="b4ad8-136">siteCollectionId</span></span>|<span data-ttu-id="b4ad8-137">String</span><span class="sxs-lookup"><span data-stu-id="b4ad8-137">String</span></span>|<span data-ttu-id="b4ad8-138">若要将复制到的 SharePoint 网站的 id。</span><span class="sxs-lookup"><span data-stu-id="b4ad8-138">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="b4ad8-139">仅当将复制到 Office 365 团队网站使用。</span><span class="sxs-lookup"><span data-stu-id="b4ad8-139">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="b4ad8-140">siteId</span><span class="sxs-lookup"><span data-stu-id="b4ad8-140">siteId</span></span>|<span data-ttu-id="b4ad8-141">String</span><span class="sxs-lookup"><span data-stu-id="b4ad8-141">String</span></span>|<span data-ttu-id="b4ad8-142">SharePoint 网站复制到的 id。</span><span class="sxs-lookup"><span data-stu-id="b4ad8-142">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="b4ad8-143">仅当将复制到 Office 365 团队网站使用。</span><span class="sxs-lookup"><span data-stu-id="b4ad8-143">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="b4ad8-144">groupId</span><span class="sxs-lookup"><span data-stu-id="b4ad8-144">groupId</span></span>|<span data-ttu-id="b4ad8-145">String</span><span class="sxs-lookup"><span data-stu-id="b4ad8-145">String</span></span>|<span data-ttu-id="b4ad8-p108">要复制到的组的 ID。仅在复制到 Office 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="b4ad8-p108">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="b4ad8-148">renameAs</span><span class="sxs-lookup"><span data-stu-id="b4ad8-148">renameAs</span></span>|<span data-ttu-id="b4ad8-149">String</span><span class="sxs-lookup"><span data-stu-id="b4ad8-149">String</span></span>|<span data-ttu-id="b4ad8-p109">副本的名称。默认为现有项的名称。</span><span class="sxs-lookup"><span data-stu-id="b4ad8-p109">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="b4ad8-152">响应</span><span class="sxs-lookup"><span data-stu-id="b4ad8-152">Response</span></span>

<span data-ttu-id="b4ad8-p110">如果成功，此方法返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。轮询 Operation-Location 终结点以[获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="b4ad8-p110">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="b4ad8-155">示例</span><span class="sxs-lookup"><span data-stu-id="b4ad8-155">Example</span></span>
<span data-ttu-id="b4ad8-156">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="b4ad8-156">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b4ad8-157">请求</span><span class="sxs-lookup"><span data-stu-id="b4ad8-157">Request</span></span>
<span data-ttu-id="b4ad8-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b4ad8-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="b4ad8-159">响应</span><span class="sxs-lookup"><span data-stu-id="b4ad8-159">Response</span></span>
<span data-ttu-id="b4ad8-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b4ad8-160">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/notebook-copynotebook.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
