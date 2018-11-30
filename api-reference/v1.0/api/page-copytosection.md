---
title: 'page: copyToSection'
description: 将页面复制到特定分区。
ms.openlocfilehash: eaa6aae4939856be14a47de1800d3691b53274ec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009547"
---
# <a name="page-copytosection"></a><span data-ttu-id="7b937-103">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="7b937-103">page: copyToSection</span></span>
<span data-ttu-id="7b937-104">将页面复制到特定分区。</span><span class="sxs-lookup"><span data-stu-id="7b937-104">Copies a page to a specific section.</span></span>

<span data-ttu-id="7b937-105">对于 Copy 操作，请遵循异步调用模式：首先调用 Copy 操作，然后轮询该操作终结点获取结果。</span><span class="sxs-lookup"><span data-stu-id="7b937-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b937-106">权限</span><span class="sxs-lookup"><span data-stu-id="7b937-106">Permissions</span></span>
<span data-ttu-id="7b937-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b937-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b937-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b937-109">Permission type</span></span>      | <span data-ttu-id="7b937-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7b937-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b937-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b937-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7b937-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b937-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="7b937-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b937-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b937-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7b937-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="7b937-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b937-115">Application</span></span> | <span data-ttu-id="7b937-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b937-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b937-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b937-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="7b937-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b937-118">Request headers</span></span>
| <span data-ttu-id="7b937-119">名称</span><span class="sxs-lookup"><span data-stu-id="7b937-119">Name</span></span>       | <span data-ttu-id="7b937-120">类型</span><span class="sxs-lookup"><span data-stu-id="7b937-120">Type</span></span> | <span data-ttu-id="7b937-121">说明</span><span class="sxs-lookup"><span data-stu-id="7b937-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7b937-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b937-122">Authorization</span></span>  | <span data-ttu-id="7b937-123">string</span><span class="sxs-lookup"><span data-stu-id="7b937-123">string</span></span>  | <span data-ttu-id="7b937-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7b937-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7b937-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7b937-126">Content-Type</span></span> | <span data-ttu-id="7b937-127">string</span><span class="sxs-lookup"><span data-stu-id="7b937-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="7b937-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b937-128">Request body</span></span>
<span data-ttu-id="7b937-129">在请求正文中，提供包含操作所需参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7b937-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="7b937-130">参数</span><span class="sxs-lookup"><span data-stu-id="7b937-130">Parameter</span></span>    | <span data-ttu-id="7b937-131">类型</span><span class="sxs-lookup"><span data-stu-id="7b937-131">Type</span></span>   |<span data-ttu-id="7b937-132">说明</span><span class="sxs-lookup"><span data-stu-id="7b937-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b937-133">groupId</span><span class="sxs-lookup"><span data-stu-id="7b937-133">groupId</span></span>|<span data-ttu-id="7b937-134">字符串</span><span class="sxs-lookup"><span data-stu-id="7b937-134">String</span></span>|<span data-ttu-id="7b937-p103">要复制到的组的 ID。仅在复制到 Office 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="7b937-p103">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="7b937-137">id</span><span class="sxs-lookup"><span data-stu-id="7b937-137">id</span></span>|<span data-ttu-id="7b937-138">String</span><span class="sxs-lookup"><span data-stu-id="7b937-138">String</span></span>|<span data-ttu-id="7b937-p104">必需。目标分区的 ID。</span><span class="sxs-lookup"><span data-stu-id="7b937-p104">Required. The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="7b937-141">响应</span><span class="sxs-lookup"><span data-stu-id="7b937-141">Response</span></span>

<span data-ttu-id="7b937-p105">如果成功，此方法返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。轮询 Operation-Location 终结点以[获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="7b937-p105">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="7b937-144">示例</span><span class="sxs-lookup"><span data-stu-id="7b937-144">Example</span></span>
<span data-ttu-id="7b937-145">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="7b937-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7b937-146">请求</span><span class="sxs-lookup"><span data-stu-id="7b937-146">Request</span></span>
<span data-ttu-id="7b937-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7b937-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```

##### <a name="response"></a><span data-ttu-id="7b937-148">响应</span><span class="sxs-lookup"><span data-stu-id="7b937-148">Response</span></span>
<span data-ttu-id="7b937-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7b937-149">Here is an example of the response.</span></span>
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