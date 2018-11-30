---
title: 指定经理
description: 使用此 API 指定用户的经理。
ms.openlocfilehash: b0e8c9f7c7aa30784497a333d9a92e52749ade73
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046819"
---
# <a name="assign-a-manager"></a><span data-ttu-id="fb875-103">指定经理</span><span class="sxs-lookup"><span data-stu-id="fb875-103">Assign a manager</span></span>

> <span data-ttu-id="fb875-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fb875-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb875-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fb875-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fb875-106">使用此 API 指定用户的经理。</span><span class="sxs-lookup"><span data-stu-id="fb875-106">Use this API to assign a user's manager.</span></span>
> <span data-ttu-id="fb875-107">注意：不能指定直接下属，请改用此 API。</span><span class="sxs-lookup"><span data-stu-id="fb875-107">Note: You cannot assign direct reports - instead use this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb875-108">权限</span><span class="sxs-lookup"><span data-stu-id="fb875-108">Permissions</span></span>
<span data-ttu-id="fb875-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb875-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb875-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb875-111">Permission type</span></span>      | <span data-ttu-id="fb875-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb875-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb875-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb875-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fb875-114">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fb875-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fb875-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb875-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb875-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb875-116">Not supported.</span></span>    |
|<span data-ttu-id="fb875-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb875-117">Application</span></span> | <span data-ttu-id="fb875-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb875-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb875-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb875-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /users/{id}/manager/$ref
```
## <a name="request-headers"></a><span data-ttu-id="fb875-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb875-120">Request headers</span></span>
| <span data-ttu-id="fb875-121">名称</span><span class="sxs-lookup"><span data-stu-id="fb875-121">Name</span></span>       | <span data-ttu-id="fb875-122">类型</span><span class="sxs-lookup"><span data-stu-id="fb875-122">Type</span></span> | <span data-ttu-id="fb875-123">说明</span><span class="sxs-lookup"><span data-stu-id="fb875-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fb875-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb875-124">Authorization</span></span>  | <span data-ttu-id="fb875-125">string</span><span class="sxs-lookup"><span data-stu-id="fb875-125">string</span></span>  | <span data-ttu-id="fb875-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fb875-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb875-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb875-128">Request body</span></span>
<span data-ttu-id="fb875-129">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md) 或 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb875-129">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="fb875-130">响应</span><span class="sxs-lookup"><span data-stu-id="fb875-130">Response</span></span>

<span data-ttu-id="fb875-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fb875-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb875-133">示例</span><span class="sxs-lookup"><span data-stu-id="fb875-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb875-134">请求</span><span class="sxs-lookup"><span data-stu-id="fb875-134">Request</span></span>
<span data-ttu-id="fb875-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb875-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
PUT https://graph.microsoft.com/v1.0/users/{id}/manager/$ref
Content-type: application/json
Content-length: xxx

{
  "@odata.id": "https://graph.microsoft.com/v1.0/users/{id}"
}
```
<span data-ttu-id="fb875-136">在请求正文中，提供要添加的 [user](../resources/user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb875-136">In the request body, supply a JSON representation of [user](../resources/user.md) object to be added.</span></span>
##### <a name="response"></a><span data-ttu-id="fb875-137">响应</span><span class="sxs-lookup"><span data-stu-id="fb875-137">Response</span></span>
<span data-ttu-id="fb875-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fb875-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
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
