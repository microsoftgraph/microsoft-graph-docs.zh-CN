---
title: 'page: copyToSection'
description: 将页面复制到特定分区。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: b09c47ab7dbaec7b7dd63d134cdefae1260d9e8d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934819"
---
# <a name="page-copytosection"></a><span data-ttu-id="36f4e-103">page: copyToSection</span><span class="sxs-lookup"><span data-stu-id="36f4e-103">page: copyToSection</span></span>
<span data-ttu-id="36f4e-104">将页面复制到特定分区。</span><span class="sxs-lookup"><span data-stu-id="36f4e-104">Copies a page to a specific section.</span></span>

<span data-ttu-id="36f4e-105">对于 Copy 操作，请遵循异步调用模式：首先调用 Copy 操作，然后轮询该操作终结点获取结果。</span><span class="sxs-lookup"><span data-stu-id="36f4e-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="36f4e-106">权限</span><span class="sxs-lookup"><span data-stu-id="36f4e-106">Permissions</span></span>
<span data-ttu-id="36f4e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36f4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36f4e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="36f4e-109">Permission type</span></span>      | <span data-ttu-id="36f4e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="36f4e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36f4e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36f4e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="36f4e-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36f4e-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="36f4e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36f4e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36f4e-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36f4e-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="36f4e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="36f4e-115">Application</span></span> | <span data-ttu-id="36f4e-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36f4e-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="36f4e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36f4e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/pages/{id}/copyToSection
POST /users/{id | userPrincipalName}/onenote/pages/{id}/copyToSection
POST /groups/{id}/onenote/pages/{id}/copyToSection
```
## <a name="request-headers"></a><span data-ttu-id="36f4e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="36f4e-118">Request headers</span></span>
| <span data-ttu-id="36f4e-119">名称</span><span class="sxs-lookup"><span data-stu-id="36f4e-119">Name</span></span>       | <span data-ttu-id="36f4e-120">类型</span><span class="sxs-lookup"><span data-stu-id="36f4e-120">Type</span></span> | <span data-ttu-id="36f4e-121">说明</span><span class="sxs-lookup"><span data-stu-id="36f4e-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="36f4e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="36f4e-122">Authorization</span></span>  | <span data-ttu-id="36f4e-123">string</span><span class="sxs-lookup"><span data-stu-id="36f4e-123">string</span></span>  | <span data-ttu-id="36f4e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="36f4e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="36f4e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="36f4e-126">Content-Type</span></span> | <span data-ttu-id="36f4e-127">string</span><span class="sxs-lookup"><span data-stu-id="36f4e-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="36f4e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="36f4e-128">Request body</span></span>
<span data-ttu-id="36f4e-129">在请求正文中，提供包含操作所需参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="36f4e-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="36f4e-130">参数</span><span class="sxs-lookup"><span data-stu-id="36f4e-130">Parameter</span></span>    | <span data-ttu-id="36f4e-131">类型</span><span class="sxs-lookup"><span data-stu-id="36f4e-131">Type</span></span>   |<span data-ttu-id="36f4e-132">说明</span><span class="sxs-lookup"><span data-stu-id="36f4e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36f4e-133">groupId</span><span class="sxs-lookup"><span data-stu-id="36f4e-133">groupId</span></span>|<span data-ttu-id="36f4e-134">字符串</span><span class="sxs-lookup"><span data-stu-id="36f4e-134">String</span></span>|<span data-ttu-id="36f4e-p103">要复制到的组的 ID。仅在复制到 Office 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="36f4e-p103">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="36f4e-137">id</span><span class="sxs-lookup"><span data-stu-id="36f4e-137">id</span></span>|<span data-ttu-id="36f4e-138">String</span><span class="sxs-lookup"><span data-stu-id="36f4e-138">String</span></span>|<span data-ttu-id="36f4e-p104">必需。目标分区的 ID。</span><span class="sxs-lookup"><span data-stu-id="36f4e-p104">Required. The id of the destination section.</span></span>|

## <a name="response"></a><span data-ttu-id="36f4e-141">响应</span><span class="sxs-lookup"><span data-stu-id="36f4e-141">Response</span></span>

<span data-ttu-id="36f4e-p105">如果成功，此方法返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。轮询 Operation-Location 终结点以[获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="36f4e-p105">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="36f4e-144">示例</span><span class="sxs-lookup"><span data-stu-id="36f4e-144">Example</span></span>
<span data-ttu-id="36f4e-145">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="36f4e-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="36f4e-146">请求</span><span class="sxs-lookup"><span data-stu-id="36f4e-146">Request</span></span>
<span data-ttu-id="36f4e-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="36f4e-147">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="36f4e-148">响应</span><span class="sxs-lookup"><span data-stu-id="36f4e-148">Response</span></span>
<span data-ttu-id="36f4e-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="36f4e-149">Here is an example of the response.</span></span>
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
