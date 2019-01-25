---
title: 'section: copyToNotebook'
description: 将分区复制到特定笔记本。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 4ec5292aa7b11b268b73514af8aee42260e3d6a9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523321"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="a0a00-103">section: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="a0a00-103">section: copyToNotebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0a00-104">将分区复制到特定笔记本。</span><span class="sxs-lookup"><span data-stu-id="a0a00-104">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="a0a00-105">对于 Copy 操作，请遵循异步调用模式：首先调用 Copy 操作，然后轮询该操作终结点获取结果。</span><span class="sxs-lookup"><span data-stu-id="a0a00-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="a0a00-106">权限</span><span class="sxs-lookup"><span data-stu-id="a0a00-106">Permissions</span></span>
<span data-ttu-id="a0a00-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0a00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0a00-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0a00-109">Permission type</span></span>      | <span data-ttu-id="a0a00-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0a00-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0a00-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0a00-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a0a00-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0a00-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a0a00-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0a00-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0a00-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0a00-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="a0a00-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0a00-115">Application</span></span> | <span data-ttu-id="a0a00-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0a00-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0a00-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0a00-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
POST /sites/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="a0a00-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0a00-118">Request headers</span></span>
| <span data-ttu-id="a0a00-119">名称</span><span class="sxs-lookup"><span data-stu-id="a0a00-119">Name</span></span>       | <span data-ttu-id="a0a00-120">类型</span><span class="sxs-lookup"><span data-stu-id="a0a00-120">Type</span></span> | <span data-ttu-id="a0a00-121">说明</span><span class="sxs-lookup"><span data-stu-id="a0a00-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a0a00-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0a00-122">Authorization</span></span>  | <span data-ttu-id="a0a00-123">string</span><span class="sxs-lookup"><span data-stu-id="a0a00-123">string</span></span>  | <span data-ttu-id="a0a00-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a0a00-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a0a00-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a0a00-126">Content-Type</span></span> | <span data-ttu-id="a0a00-127">string</span><span class="sxs-lookup"><span data-stu-id="a0a00-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="a0a00-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0a00-128">Request body</span></span>
<span data-ttu-id="a0a00-129">在请求正文中，提供包含操作所需参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a0a00-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="a0a00-130">参数</span><span class="sxs-lookup"><span data-stu-id="a0a00-130">Parameter</span></span>    | <span data-ttu-id="a0a00-131">类型</span><span class="sxs-lookup"><span data-stu-id="a0a00-131">Type</span></span>   |<span data-ttu-id="a0a00-132">说明</span><span class="sxs-lookup"><span data-stu-id="a0a00-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0a00-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="a0a00-133">siteCollectionId</span></span>|<span data-ttu-id="a0a00-134">String</span><span class="sxs-lookup"><span data-stu-id="a0a00-134">String</span></span>|<span data-ttu-id="a0a00-135">若要将复制到的 SharePoint 网站的 id。</span><span class="sxs-lookup"><span data-stu-id="a0a00-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="a0a00-136">仅当将复制到 Office 365 团队网站使用。</span><span class="sxs-lookup"><span data-stu-id="a0a00-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="a0a00-137">siteId</span><span class="sxs-lookup"><span data-stu-id="a0a00-137">siteId</span></span>|<span data-ttu-id="a0a00-138">String</span><span class="sxs-lookup"><span data-stu-id="a0a00-138">String</span></span>|<span data-ttu-id="a0a00-139">SharePoint 网站复制到的 id。</span><span class="sxs-lookup"><span data-stu-id="a0a00-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="a0a00-140">仅当将复制到 Office 365 团队网站使用。</span><span class="sxs-lookup"><span data-stu-id="a0a00-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="a0a00-141">groupId</span><span class="sxs-lookup"><span data-stu-id="a0a00-141">groupId</span></span>|<span data-ttu-id="a0a00-142">String</span><span class="sxs-lookup"><span data-stu-id="a0a00-142">String</span></span>|<span data-ttu-id="a0a00-p105">要复制到的组的 ID。仅在复制到 Office 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="a0a00-p105">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="a0a00-145">id</span><span class="sxs-lookup"><span data-stu-id="a0a00-145">id</span></span>|<span data-ttu-id="a0a00-146">String</span><span class="sxs-lookup"><span data-stu-id="a0a00-146">String</span></span>|<span data-ttu-id="a0a00-p106">必需。目标笔记本的 ID。</span><span class="sxs-lookup"><span data-stu-id="a0a00-p106">Required. The id of the destination notebook.</span></span> |
|<span data-ttu-id="a0a00-149">renameAs</span><span class="sxs-lookup"><span data-stu-id="a0a00-149">renameAs</span></span>|<span data-ttu-id="a0a00-150">String</span><span class="sxs-lookup"><span data-stu-id="a0a00-150">String</span></span>|<span data-ttu-id="a0a00-p107">副本的名称。默认为现有项的名称。</span><span class="sxs-lookup"><span data-stu-id="a0a00-p107">The name of the copy. Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="a0a00-153">响应</span><span class="sxs-lookup"><span data-stu-id="a0a00-153">Response</span></span>

<span data-ttu-id="a0a00-p108">如果成功，此方法返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。轮询 Operation-Location 终结点以[获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="a0a00-p108">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="a0a00-156">示例</span><span class="sxs-lookup"><span data-stu-id="a0a00-156">Example</span></span>
<span data-ttu-id="a0a00-157">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a0a00-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a0a00-158">请求</span><span class="sxs-lookup"><span data-stu-id="a0a00-158">Request</span></span>
<span data-ttu-id="a0a00-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a0a00-159">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="a0a00-160">响应</span><span class="sxs-lookup"><span data-stu-id="a0a00-160">Response</span></span>
<span data-ttu-id="a0a00-161">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a0a00-161">Here is an example of the response.</span></span>
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
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/section-copytonotebook.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
