---
title: '页面: copyToSection'
description: 将页面复制到特定分区。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: dd7abb016345195bd5a32e20a5623d6fca9fd6ff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539378"
---
# <a name="page-copytosection"></a><span data-ttu-id="56017-103">页面: copyToSection</span><span class="sxs-lookup"><span data-stu-id="56017-103">page: copyToSection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56017-104">将页面复制到特定分区。</span><span class="sxs-lookup"><span data-stu-id="56017-104">Copies a page to a specific section.</span></span>

<span data-ttu-id="56017-105">对于复制操作, 请遵循异步调用模式: 首先调用复制操作, 然后轮询操作终结点以获取结果。</span><span class="sxs-lookup"><span data-stu-id="56017-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="56017-106">权限</span><span class="sxs-lookup"><span data-stu-id="56017-106">Permissions</span></span>
<span data-ttu-id="56017-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56017-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56017-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="56017-109">Permission type</span></span>      | <span data-ttu-id="56017-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56017-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56017-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56017-111">Delegated (work or school account)</span></span> | <span data-ttu-id="56017-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56017-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="56017-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56017-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56017-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56017-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="56017-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="56017-115">Application</span></span> | <span data-ttu-id="56017-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56017-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56017-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56017-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="56017-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="56017-118">Request headers</span></span>
| <span data-ttu-id="56017-119">名称</span><span class="sxs-lookup"><span data-stu-id="56017-119">Name</span></span>       | <span data-ttu-id="56017-120">类型</span><span class="sxs-lookup"><span data-stu-id="56017-120">Type</span></span> | <span data-ttu-id="56017-121">说明</span><span class="sxs-lookup"><span data-stu-id="56017-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="56017-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="56017-122">Authorization</span></span>  | <span data-ttu-id="56017-123">string</span><span class="sxs-lookup"><span data-stu-id="56017-123">string</span></span>  | <span data-ttu-id="56017-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="56017-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="56017-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="56017-126">Content-Type</span></span> | <span data-ttu-id="56017-127">string</span><span class="sxs-lookup"><span data-stu-id="56017-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="56017-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="56017-128">Request body</span></span>
<span data-ttu-id="56017-129">在请求正文中, 提供一个 JSON 对象, 其中包含您的操作所需的参数。</span><span class="sxs-lookup"><span data-stu-id="56017-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="56017-130">参数</span><span class="sxs-lookup"><span data-stu-id="56017-130">Parameter</span></span>    | <span data-ttu-id="56017-131">类型</span><span class="sxs-lookup"><span data-stu-id="56017-131">Type</span></span>   |<span data-ttu-id="56017-132">说明</span><span class="sxs-lookup"><span data-stu-id="56017-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56017-133">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="56017-133">siteCollectionId</span></span>|<span data-ttu-id="56017-134">String</span><span class="sxs-lookup"><span data-stu-id="56017-134">String</span></span>|<span data-ttu-id="56017-135">要复制到的 SharePoint 网站的 id。</span><span class="sxs-lookup"><span data-stu-id="56017-135">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="56017-136">仅在复制到 Office 365 团队网站时使用。</span><span class="sxs-lookup"><span data-stu-id="56017-136">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="56017-137">siteId</span><span class="sxs-lookup"><span data-stu-id="56017-137">siteId</span></span>|<span data-ttu-id="56017-138">String</span><span class="sxs-lookup"><span data-stu-id="56017-138">String</span></span>|<span data-ttu-id="56017-139">要复制到的 SharePoint 网站的 id。</span><span class="sxs-lookup"><span data-stu-id="56017-139">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="56017-140">仅在复制到 Office 365 团队网站时使用。</span><span class="sxs-lookup"><span data-stu-id="56017-140">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="56017-141">groupId</span><span class="sxs-lookup"><span data-stu-id="56017-141">groupId</span></span>|<span data-ttu-id="56017-142">String</span><span class="sxs-lookup"><span data-stu-id="56017-142">String</span></span>|<span data-ttu-id="56017-143">要复制到的组的 id。</span><span class="sxs-lookup"><span data-stu-id="56017-143">The id of the group to copy to.</span></span> <span data-ttu-id="56017-144">仅在复制到 Office 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="56017-144">Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="56017-145">id</span><span class="sxs-lookup"><span data-stu-id="56017-145">id</span></span>|<span data-ttu-id="56017-146">String</span><span class="sxs-lookup"><span data-stu-id="56017-146">String</span></span>|<span data-ttu-id="56017-147">必需。</span><span class="sxs-lookup"><span data-stu-id="56017-147">Required.</span></span> <span data-ttu-id="56017-148">目标部分的 id。</span><span class="sxs-lookup"><span data-stu-id="56017-148">The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="56017-149">响应</span><span class="sxs-lookup"><span data-stu-id="56017-149">Response</span></span>

<span data-ttu-id="56017-150">如果成功, 此方法将`202 Accepted`返回响应代码和`Operation-Location`标头。</span><span class="sxs-lookup"><span data-stu-id="56017-150">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header.</span></span> <span data-ttu-id="56017-151">轮询操作-位置终结点以[获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="56017-151">Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="56017-152">示例</span><span class="sxs-lookup"><span data-stu-id="56017-152">Example</span></span>
<span data-ttu-id="56017-153">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="56017-153">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="56017-154">请求</span><span class="sxs-lookup"><span data-stu-id="56017-154">Request</span></span>
<span data-ttu-id="56017-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="56017-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/beta/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```

##### <a name="response"></a><span data-ttu-id="56017-156">响应</span><span class="sxs-lookup"><span data-stu-id="56017-156">Response</span></span>
<span data-ttu-id="56017-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="56017-157">Here is an example of the response.</span></span>
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
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/page-copytosection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
