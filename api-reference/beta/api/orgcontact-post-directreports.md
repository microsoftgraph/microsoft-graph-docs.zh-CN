---
title: 创建 directReport
description: 使用此 API 创建新的 directReport。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c992c515f3eb63f3041b6afb246b59c2392625f9
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657124"
---
# <a name="create-directreport"></a><span data-ttu-id="59345-103">创建 directReport</span><span class="sxs-lookup"><span data-stu-id="59345-103">Create directReport</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59345-104">使用此 API 创建新的 directReport。</span><span class="sxs-lookup"><span data-stu-id="59345-104">Use this API to create a new directReport.</span></span>
## <a name="permissions"></a><span data-ttu-id="59345-105">权限</span><span class="sxs-lookup"><span data-stu-id="59345-105">Permissions</span></span>
<span data-ttu-id="59345-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59345-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59345-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="59345-108">Permission type</span></span>      | <span data-ttu-id="59345-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59345-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59345-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59345-110">Delegated (work or school account)</span></span> | <span data-ttu-id="59345-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="59345-111">Not supported.</span></span>    |
|<span data-ttu-id="59345-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59345-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59345-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="59345-113">Not supported.</span></span>    |
|<span data-ttu-id="59345-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="59345-114">Application</span></span> | <span data-ttu-id="59345-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="59345-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59345-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59345-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/directReports

```
## <a name="request-headers"></a><span data-ttu-id="59345-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="59345-117">Request headers</span></span>
| <span data-ttu-id="59345-118">名称</span><span class="sxs-lookup"><span data-stu-id="59345-118">Name</span></span>       | <span data-ttu-id="59345-119">类型</span><span class="sxs-lookup"><span data-stu-id="59345-119">Type</span></span> | <span data-ttu-id="59345-120">说明</span><span class="sxs-lookup"><span data-stu-id="59345-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="59345-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="59345-121">Authorization</span></span>  | <span data-ttu-id="59345-122">string</span><span class="sxs-lookup"><span data-stu-id="59345-122">string</span></span>  | <span data-ttu-id="59345-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="59345-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59345-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="59345-125">Request body</span></span>
<span data-ttu-id="59345-126">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59345-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="59345-127">响应</span><span class="sxs-lookup"><span data-stu-id="59345-127">Response</span></span>

<span data-ttu-id="59345-128">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="59345-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59345-129">示例</span><span class="sxs-lookup"><span data-stu-id="59345-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59345-130">请求</span><span class="sxs-lookup"><span data-stu-id="59345-130">Request</span></span>
<span data-ttu-id="59345-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="59345-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_orgcontact"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/directReports
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="59345-132">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59345-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="59345-133">响应</span><span class="sxs-lookup"><span data-stu-id="59345-133">Response</span></span>
<span data-ttu-id="59345-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="59345-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="59345-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="59345-137">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59345-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="59345-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_orgcontact-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create directReport",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-post-directreports.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
