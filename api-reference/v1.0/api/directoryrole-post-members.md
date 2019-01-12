---
title: 添加目录角色成员
description: 使用此 API 创建新的目录角色成员。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f138be1632c72f8c31eb08fcdaefc50e7affb3e5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991529"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="529ad-103">添加目录角色成员</span><span class="sxs-lookup"><span data-stu-id="529ad-103">Add directory role member</span></span>

<span data-ttu-id="529ad-104">使用此 API 创建新的目录角色成员。</span><span class="sxs-lookup"><span data-stu-id="529ad-104">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="529ad-105">权限</span><span class="sxs-lookup"><span data-stu-id="529ad-105">Permissions</span></span>
<span data-ttu-id="529ad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="529ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="529ad-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="529ad-108">Permission type</span></span>      | <span data-ttu-id="529ad-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="529ad-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="529ad-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="529ad-110">Delegated (work or school account)</span></span> | <span data-ttu-id="529ad-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="529ad-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="529ad-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="529ad-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="529ad-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="529ad-113">Not supported.</span></span>    |
|<span data-ttu-id="529ad-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="529ad-114">Application</span></span> | <span data-ttu-id="529ad-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="529ad-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="529ad-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="529ad-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="529ad-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="529ad-117">Request headers</span></span>
| <span data-ttu-id="529ad-118">名称</span><span class="sxs-lookup"><span data-stu-id="529ad-118">Name</span></span>       | <span data-ttu-id="529ad-119">类型</span><span class="sxs-lookup"><span data-stu-id="529ad-119">Type</span></span> | <span data-ttu-id="529ad-120">说明</span><span class="sxs-lookup"><span data-stu-id="529ad-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="529ad-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="529ad-121">Authorization</span></span>  | <span data-ttu-id="529ad-122">string</span><span class="sxs-lookup"><span data-stu-id="529ad-122">string</span></span>  | <span data-ttu-id="529ad-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="529ad-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="529ad-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="529ad-125">Content-Type</span></span>  | <span data-ttu-id="529ad-126">string</span><span class="sxs-lookup"><span data-stu-id="529ad-126">string</span></span>  | <span data-ttu-id="529ad-127">application/json</span><span class="sxs-lookup"><span data-stu-id="529ad-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="529ad-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="529ad-128">Request body</span></span>
<span data-ttu-id="529ad-129">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md) 或 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="529ad-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="529ad-130">响应</span><span class="sxs-lookup"><span data-stu-id="529ad-130">Response</span></span>

<span data-ttu-id="529ad-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="529ad-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="529ad-132">示例</span><span class="sxs-lookup"><span data-stu-id="529ad-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="529ad-133">请求</span><span class="sxs-lookup"><span data-stu-id="529ad-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

##### <a name="response"></a><span data-ttu-id="529ad-134">响应</span><span class="sxs-lookup"><span data-stu-id="529ad-134">Response</span></span>
<span data-ttu-id="529ad-135">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="529ad-135">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
