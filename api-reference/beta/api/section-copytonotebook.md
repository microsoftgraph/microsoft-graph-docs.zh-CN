---
title: '部分: copyToNotebook'
description: 将分区复制到特定笔记本。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 4ec5292aa7b11b268b73514af8aee42260e3d6a9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545527"
---
# <a name="section-copytonotebook"></a><span data-ttu-id="2048e-103">部分: copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="2048e-103">section: copyToNotebook</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2048e-104">将分区复制到特定笔记本。</span><span class="sxs-lookup"><span data-stu-id="2048e-104">Copies a section to a specific notebook.</span></span>

<span data-ttu-id="2048e-105">对于复制操作, 请遵循异步调用模式: 首先调用复制操作, 然后轮询操作终结点以获取结果。</span><span class="sxs-lookup"><span data-stu-id="2048e-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>
## <a name="permissions"></a><span data-ttu-id="2048e-106">权限</span><span class="sxs-lookup"><span data-stu-id="2048e-106">Permissions</span></span>
<span data-ttu-id="2048e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2048e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2048e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2048e-109">Permission type</span></span>      | <span data-ttu-id="2048e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2048e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2048e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2048e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2048e-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2048e-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="2048e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2048e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2048e-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2048e-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="2048e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2048e-115">Application</span></span> | <span data-ttu-id="2048e-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2048e-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2048e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2048e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToNotebook
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToNotebook
POST /groups/{id}/onenote/sections/{id}/copyToNotebook
POST /sites/{id}/onenote/sections/{id}/copyToNotebook
```
## <a name="request-headers"></a><span data-ttu-id="2048e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2048e-118">Request headers</span></span>
| <span data-ttu-id="2048e-119">名称</span><span class="sxs-lookup"><span data-stu-id="2048e-119">Name</span></span>       | <span data-ttu-id="2048e-120">类型</span><span class="sxs-lookup"><span data-stu-id="2048e-120">Type</span></span> | <span data-ttu-id="2048e-121">说明</span><span class="sxs-lookup"><span data-stu-id="2048e-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2048e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2048e-122">Authorization</span></span>  | <span data-ttu-id="2048e-123">string</span><span class="sxs-lookup"><span data-stu-id="2048e-123">string</span></span>  | <span data-ttu-id="2048e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2048e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2048e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2048e-126">Content-Type</span></span> | <span data-ttu-id="2048e-127">string</span><span class="sxs-lookup"><span data-stu-id="2048e-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="2048e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="2048e-128">Request body</span></span>
<span data-ttu-id="2048e-129">在请求正文中, 提供一个 JSON 对象, 其中包含您的操作所需的参数。</span><span class="sxs-lookup"><span data-stu-id="2048e-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="2048e-130">参数</span><span class="sxs-lookup"><span data-stu-id="2048e-130">Parameter</span></span>    | <span data-ttu-id="2048e-131">类型</span><span class="sxs-lookup"><span data-stu-id="2048e-131">Type</span></span>   |<span data-ttu-id="2048e-132">说明</span><span class="sxs-lookup"><span data-stu-id="2048e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2048e-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="2048e-133">siteCollectionId</span></span>|<span data-ttu-id="2048e-134">String</span><span class="sxs-lookup"><span data-stu-id="2048e-134">String</span></span>|<span data-ttu-id="2048e-135">要复制到的 SharePoint 网站的 id。</span><span class="sxs-lookup"><span data-stu-id="2048e-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="2048e-136">仅在复制到 Office 365 团队网站时使用。</span><span class="sxs-lookup"><span data-stu-id="2048e-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="2048e-137">siteId</span><span class="sxs-lookup"><span data-stu-id="2048e-137">siteId</span></span>|<span data-ttu-id="2048e-138">String</span><span class="sxs-lookup"><span data-stu-id="2048e-138">String</span></span>|<span data-ttu-id="2048e-139">要复制到的 SharePoint 网站的 id。</span><span class="sxs-lookup"><span data-stu-id="2048e-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="2048e-140">仅在复制到 Office 365 团队网站时使用。</span><span class="sxs-lookup"><span data-stu-id="2048e-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="2048e-141">groupId</span><span class="sxs-lookup"><span data-stu-id="2048e-141">groupId</span></span>|<span data-ttu-id="2048e-142">String</span><span class="sxs-lookup"><span data-stu-id="2048e-142">String</span></span>|<span data-ttu-id="2048e-143">要复制到的组的 id。</span><span class="sxs-lookup"><span data-stu-id="2048e-143">The id of the group to copy to.</span></span> <span data-ttu-id="2048e-144">仅在复制到 Office 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="2048e-144">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="2048e-145">id</span><span class="sxs-lookup"><span data-stu-id="2048e-145">id</span></span>|<span data-ttu-id="2048e-146">String</span><span class="sxs-lookup"><span data-stu-id="2048e-146">String</span></span>|<span data-ttu-id="2048e-147">必需。</span><span class="sxs-lookup"><span data-stu-id="2048e-147">Required.</span></span> <span data-ttu-id="2048e-148">目标笔记本的 id。</span><span class="sxs-lookup"><span data-stu-id="2048e-148">The id of the destination notebook.</span></span> |
|<span data-ttu-id="2048e-149">renameAs</span><span class="sxs-lookup"><span data-stu-id="2048e-149">renameAs</span></span>|<span data-ttu-id="2048e-150">String</span><span class="sxs-lookup"><span data-stu-id="2048e-150">String</span></span>|<span data-ttu-id="2048e-151">副本的名称。</span><span class="sxs-lookup"><span data-stu-id="2048e-151">The name of the copy.</span></span> <span data-ttu-id="2048e-152">默认值为现有项目的名称。</span><span class="sxs-lookup"><span data-stu-id="2048e-152">Defaults to the name of the existing item.</span></span> |

## <a name="response"></a><span data-ttu-id="2048e-153">响应</span><span class="sxs-lookup"><span data-stu-id="2048e-153">Response</span></span>

<span data-ttu-id="2048e-154">如果成功, 此方法将`202 Accepted`返回响应代码和`Operation-Location`标头。</span><span class="sxs-lookup"><span data-stu-id="2048e-154">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="2048e-155">轮询操作-位置终结点以[获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="2048e-155">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="2048e-156">示例</span><span class="sxs-lookup"><span data-stu-id="2048e-156">Example</span></span>
<span data-ttu-id="2048e-157">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="2048e-157">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2048e-158">请求</span><span class="sxs-lookup"><span data-stu-id="2048e-158">Request</span></span>
<span data-ttu-id="2048e-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2048e-159">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="2048e-160">响应</span><span class="sxs-lookup"><span data-stu-id="2048e-160">Response</span></span>
<span data-ttu-id="2048e-161">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2048e-161">Here is an example of the response.</span></span>
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
