---
title: 'section: copyToSectionGroup'
description: 将分区复制到特定分区组。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 18afd7d0ac94b9964a049b1ad0c2c120f0d2627b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980256"
---
# <a name="section-copytosectiongroup"></a><span data-ttu-id="5c4d5-103">section: copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="5c4d5-103">section: copyToSectionGroup</span></span>
<span data-ttu-id="5c4d5-104">将分区复制到特定分区组。</span><span class="sxs-lookup"><span data-stu-id="5c4d5-104">Copies a section to a specific section group.</span></span>

<span data-ttu-id="5c4d5-105">对于 Copy 操作，请遵循异步调用模式：首先调用 Copy 操作，然后轮询该操作终结点获取结果。</span><span class="sxs-lookup"><span data-stu-id="5c4d5-105">For Copy operations, you follow an asynchronous calling pattern:  First call the Copy action, and then poll the operation endpoint for the result.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c4d5-106">权限</span><span class="sxs-lookup"><span data-stu-id="5c4d5-106">Permissions</span></span>
<span data-ttu-id="5c4d5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c4d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c4d5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c4d5-109">Permission type</span></span>      | <span data-ttu-id="5c4d5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5c4d5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c4d5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c4d5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5c4d5-112">Notes.Create、Notes.ReadWrite、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c4d5-112">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="5c4d5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c4d5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c4d5-114">Notes.Create、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c4d5-114">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="5c4d5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c4d5-115">Application</span></span> | <span data-ttu-id="5c4d5-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c4d5-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c4d5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c4d5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/copyToSectionGroup
POST /users/{id | userPrincipalName}/onenote/sections/{id}/copyToSectionGroup
POST /groups/{id}/onenote/sections/{id}/copyToSectionGroup
```
## <a name="request-headers"></a><span data-ttu-id="5c4d5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c4d5-118">Request headers</span></span>
| <span data-ttu-id="5c4d5-119">名称</span><span class="sxs-lookup"><span data-stu-id="5c4d5-119">Name</span></span>       | <span data-ttu-id="5c4d5-120">类型</span><span class="sxs-lookup"><span data-stu-id="5c4d5-120">Type</span></span> | <span data-ttu-id="5c4d5-121">说明</span><span class="sxs-lookup"><span data-stu-id="5c4d5-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5c4d5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c4d5-122">Authorization</span></span>  | <span data-ttu-id="5c4d5-123">string</span><span class="sxs-lookup"><span data-stu-id="5c4d5-123">string</span></span>  | <span data-ttu-id="5c4d5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5c4d5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5c4d5-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5c4d5-126">Content-Type</span></span> | <span data-ttu-id="5c4d5-127">string</span><span class="sxs-lookup"><span data-stu-id="5c4d5-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="5c4d5-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c4d5-128">Request body</span></span>
<span data-ttu-id="5c4d5-129">在请求正文中，提供包含操作所需参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5c4d5-129">In the request body, provide a JSON object that contains the parameters that your operation needs.</span></span>

| <span data-ttu-id="5c4d5-130">参数</span><span class="sxs-lookup"><span data-stu-id="5c4d5-130">Parameter</span></span>    | <span data-ttu-id="5c4d5-131">类型</span><span class="sxs-lookup"><span data-stu-id="5c4d5-131">Type</span></span>   |<span data-ttu-id="5c4d5-132">说明</span><span class="sxs-lookup"><span data-stu-id="5c4d5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c4d5-133">groupId</span><span class="sxs-lookup"><span data-stu-id="5c4d5-133">groupId</span></span>|<span data-ttu-id="5c4d5-134">字符串</span><span class="sxs-lookup"><span data-stu-id="5c4d5-134">String</span></span>|<span data-ttu-id="5c4d5-p103">要复制到的组的 ID。仅在复制到 Office 365 组时使用。</span><span class="sxs-lookup"><span data-stu-id="5c4d5-p103">The id of the group to copy to. Use only when copying to an Office 365 group.</span></span>|
|<span data-ttu-id="5c4d5-137">id</span><span class="sxs-lookup"><span data-stu-id="5c4d5-137">id</span></span>|<span data-ttu-id="5c4d5-138">字符串</span><span class="sxs-lookup"><span data-stu-id="5c4d5-138">String</span></span>|<span data-ttu-id="5c4d5-p104">必需。目标分区组的 ID。</span><span class="sxs-lookup"><span data-stu-id="5c4d5-p104">Required. The id of the destination section group.</span></span> |
|<span data-ttu-id="5c4d5-141">renameAs</span><span class="sxs-lookup"><span data-stu-id="5c4d5-141">renameAs</span></span>|<span data-ttu-id="5c4d5-142">字符串</span><span class="sxs-lookup"><span data-stu-id="5c4d5-142">String</span></span>|<span data-ttu-id="5c4d5-p105">副本的名称。默认为现有项的名称。</span><span class="sxs-lookup"><span data-stu-id="5c4d5-p105">The name of the copy. Defaults to the name of the existing item.</span></span> |

<!--groupId missing-->
<!--|siteCollectionId|String||
|siteId|String||-->

## <a name="response"></a><span data-ttu-id="5c4d5-145">响应</span><span class="sxs-lookup"><span data-stu-id="5c4d5-145">Response</span></span>

<span data-ttu-id="5c4d5-p106">如果成功，此方法返回 `202 Accepted` 响应代码和 `Operation-Location` 标头。轮询 Operation-Location 终结点以[获取复制操作的状态](onenoteoperation-get.md)。</span><span class="sxs-lookup"><span data-stu-id="5c4d5-p106">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation-get.md).</span></span>

## <a name="example"></a><span data-ttu-id="5c4d5-148">示例</span><span class="sxs-lookup"><span data-stu-id="5c4d5-148">Example</span></span>
<span data-ttu-id="5c4d5-149">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="5c4d5-149">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5c4d5-150">请求</span><span class="sxs-lookup"><span data-stu-id="5c4d5-150">Request</span></span>
<span data-ttu-id="5c4d5-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5c4d5-151">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytosectiongroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToSectionGroup
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <a name="response"></a><span data-ttu-id="5c4d5-152">响应</span><span class="sxs-lookup"><span data-stu-id="5c4d5-152">Response</span></span>
<span data-ttu-id="5c4d5-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5c4d5-153">Here is an example of the response.</span></span>
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
  "description": "section: copyToSectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
