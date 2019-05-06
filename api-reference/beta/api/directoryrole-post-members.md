---
title: 添加目录角色成员
description: 使用此 API 创建新的目录角色成员。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8037ee8945b7f8bc25e2daf39dd23a2142b81045
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33590292"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="fa23f-103">添加目录角色成员</span><span class="sxs-lookup"><span data-stu-id="fa23f-103">Add directory role member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa23f-104">使用此 API 创建新的目录角色成员。</span><span class="sxs-lookup"><span data-stu-id="fa23f-104">Use this API to create a new directory role member.</span></span>
## <a name="permissions"></a><span data-ttu-id="fa23f-105">权限</span><span class="sxs-lookup"><span data-stu-id="fa23f-105">Permissions</span></span>
<span data-ttu-id="fa23f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa23f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa23f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa23f-108">Permission type</span></span>      | <span data-ttu-id="fa23f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa23f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa23f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa23f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fa23f-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fa23f-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fa23f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa23f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa23f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa23f-113">Not supported.</span></span>    |
|<span data-ttu-id="fa23f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa23f-114">Application</span></span> | <span data-ttu-id="fa23f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa23f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa23f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa23f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="fa23f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa23f-117">Request headers</span></span>
| <span data-ttu-id="fa23f-118">名称</span><span class="sxs-lookup"><span data-stu-id="fa23f-118">Name</span></span>       | <span data-ttu-id="fa23f-119">类型</span><span class="sxs-lookup"><span data-stu-id="fa23f-119">Type</span></span> | <span data-ttu-id="fa23f-120">说明</span><span class="sxs-lookup"><span data-stu-id="fa23f-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fa23f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa23f-121">Authorization</span></span>  | <span data-ttu-id="fa23f-122">string</span><span class="sxs-lookup"><span data-stu-id="fa23f-122">string</span></span>  | <span data-ttu-id="fa23f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fa23f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa23f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa23f-125">Request body</span></span>
<span data-ttu-id="fa23f-126">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa23f-126">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fa23f-127">响应</span><span class="sxs-lookup"><span data-stu-id="fa23f-127">Response</span></span>

<span data-ttu-id="fa23f-128">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fa23f-128">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa23f-129">示例</span><span class="sxs-lookup"><span data-stu-id="fa23f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa23f-130">请求</span><span class="sxs-lookup"><span data-stu-id="fa23f-130">Request</span></span>
<span data-ttu-id="fa23f-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fa23f-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="fa23f-132">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa23f-132">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fa23f-133">响应</span><span class="sxs-lookup"><span data-stu-id="fa23f-133">Response</span></span>
<span data-ttu-id="fa23f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fa23f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="fa23f-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="fa23f-137">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa23f-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="fa23f-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_directoryrole-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryrole-post-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
