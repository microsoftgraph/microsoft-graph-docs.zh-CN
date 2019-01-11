---
title: 'page: copyToSection'
description: 将页面复制到特定分区。
localization_priority: Normal
ms.openlocfilehash: 10d0eecd2f84a33e66209f8297b72b8a4630b100
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892503"
---
# <a name="page-copytosection"></a><span data-ttu-id="dac1c-103">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="dac1c-103">page: copyToSection</span></span>

> <span data-ttu-id="dac1c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dac1c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dac1c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dac1c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dac1c-106">将页面复制到特定分区。</span><span class="sxs-lookup"><span data-stu-id="dac1c-106">Copies a page to a specific section.</span></span>

<span data-ttu-id="dac1c-107">对于 Copy 操作，请遵循异步调用模式：首先调用 Copy 操作，然后轮询该操作终结点获取结果。</span><span class="sxs-lookup"><span data-stu-id="dac1c-107">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="dac1c-108">权限</span><span class="sxs-lookup"><span data-stu-id="dac1c-108">Permissions</span></span>
<span data-ttu-id="dac1c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dac1c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dac1c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dac1c-111">Permission type</span></span>      | <span data-ttu-id="dac1c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dac1c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dac1c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dac1c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dac1c-114">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dac1c-114">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="dac1c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dac1c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dac1c-116">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dac1c-116">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="dac1c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="dac1c-117">Application</span></span> | <span data-ttu-id="dac1c-118">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dac1c-118">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dac1c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dac1c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
POST /sites/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="dac1c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dac1c-120">Request headers</span></span>
| <span data-ttu-id="dac1c-121">名称</span><span class="sxs-lookup"><span data-stu-id="dac1c-121">Name</span></span>       | <span data-ttu-id="dac1c-122">类型</span><span class="sxs-lookup"><span data-stu-id="dac1c-122">Type</span></span> | <span data-ttu-id="dac1c-123">说明</span><span class="sxs-lookup"><span data-stu-id="dac1c-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dac1c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dac1c-124">Authorization</span></span>  | <span data-ttu-id="dac1c-125">string</span><span class="sxs-lookup"><span data-stu-id="dac1c-125">string</span></span>  | <span data-ttu-id="dac1c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dac1c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dac1c-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dac1c-128">Content-Type</span></span> | <span data-ttu-id="dac1c-129">string</span><span class="sxs-lookup"><span data-stu-id="dac1c-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="dac1c-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="dac1c-130">Request body</span></span>
<span data-ttu-id="dac1c-131">在请求正文中，提供包含操作所需参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="dac1c-131">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="dac1c-132">参数</span><span class="sxs-lookup"><span data-stu-id="dac1c-132">Parameter</span></span>    | <span data-ttu-id="dac1c-133">类型</span><span class="sxs-lookup"><span data-stu-id="dac1c-133">Type</span></span>   |<span data-ttu-id="dac1c-134">Description</span><span class="sxs-lookup"><span data-stu-id="dac1c-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dac1c-135">siteCollectionId</span><span class="sxs-lookup"><span data-stu-id="dac1c-135">siteCollectionId</span></span>|<span data-ttu-id="dac1c-136">字符串</span><span class="sxs-lookup"><span data-stu-id="dac1c-136">String</span></span>|<span data-ttu-id="dac1c-137">若要将复制到的 SharePoint 网站的 id。</span><span class="sxs-lookup"><span data-stu-id="dac1c-137">The id of the SharePoint site to copy to.</span></span> <span data-ttu-id="dac1c-138">仅当将复制到 Office 365 团队网站使用。</span><span class="sxs-lookup"><span data-stu-id="dac1c-138">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="dac1c-139">siteId</span><span class="sxs-lookup"><span data-stu-id="dac1c-139">siteId</span></span>|<span data-ttu-id="dac1c-140">字符串</span><span class="sxs-lookup"><span data-stu-id="dac1c-140">String</span></span>|<span data-ttu-id="dac1c-141">SharePoint 网站复制到的 id。</span><span class="sxs-lookup"><span data-stu-id="dac1c-141">The id of the SharePoint web to copy to.</span></span> <span data-ttu-id="dac1c-142">仅当将复制到 Office 365 团队网站使用。</span><span class="sxs-lookup"><span data-stu-id="dac1c-142">Use only when copying to an Office 365 team site.</span></span>|
|<span data-ttu-id="dac1c-143">groupId</span><span class="sxs-lookup"><span data-stu-id="dac1c-143">groupId</span></span>|<span data-ttu-id="dac1c-144">字符串</span><span class="sxs-lookup"><span data-stu-id="dac1c-144">String</span></span>|<span data-ttu-id="dac1c-p106">要复制到的组的 ID。仅在复制到 Office 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="dac1c-p106">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="dac1c-147">id</span><span class="sxs-lookup"><span data-stu-id="dac1c-147">id</span></span>|<span data-ttu-id="dac1c-148">String</span><span class="sxs-lookup"><span data-stu-id="dac1c-148">String</span></span>|<span data-ttu-id="dac1c-p107">必需。目标分区的 ID。</span><span class="sxs-lookup"><span data-stu-id="dac1c-p107">Required. The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="dac1c-151">响应</span><span class="sxs-lookup"><span data-stu-id="dac1c-151">Response</span></span>

<span data-ttu-id="dac1c-p108">如果成功，此方法返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。轮询 Operation-Location 终结点以[获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="dac1c-p108">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="dac1c-154">示例</span><span class="sxs-lookup"><span data-stu-id="dac1c-154">Example</span></span>
<span data-ttu-id="dac1c-155">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="dac1c-155">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dac1c-156">请求</span><span class="sxs-lookup"><span data-stu-id="dac1c-156">Request</span></span>
<span data-ttu-id="dac1c-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dac1c-157">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="dac1c-158">响应</span><span class="sxs-lookup"><span data-stu-id="dac1c-158">Response</span></span>
<span data-ttu-id="dac1c-159">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dac1c-159">Here is an example of the response.</span></span>
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
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
