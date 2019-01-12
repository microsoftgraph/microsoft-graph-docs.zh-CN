---
title: 添加成员
description: 使用此 API 可以通过 **members** 导航属性将成员添加到 Office 365 组、安全组或启用邮件的安全组中。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: db0261b71f6499489b48deb099a572599b482d38
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955525"
---
# <a name="add-member"></a><span data-ttu-id="484e2-103">添加成员</span><span class="sxs-lookup"><span data-stu-id="484e2-103">Add member</span></span>

> <span data-ttu-id="484e2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="484e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="484e2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="484e2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="484e2-106">使用此 API 可以通过 **members** 导航属性将成员添加到 Office 365 组、安全组或启用邮件的安全组中。</span><span class="sxs-lookup"><span data-stu-id="484e2-106">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="484e2-107">可以添加用户或其他组。</span><span class="sxs-lookup"><span data-stu-id="484e2-107">You can add users or other groups.</span></span> <span data-ttu-id="484e2-108">重要说明：只能将用户添加到 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="484e2-108">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="484e2-109">权限</span><span class="sxs-lookup"><span data-stu-id="484e2-109">Permissions</span></span>
<span data-ttu-id="484e2-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="484e2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="484e2-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="484e2-112">Permission type</span></span>      | <span data-ttu-id="484e2-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="484e2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="484e2-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="484e2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="484e2-115">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="484e2-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="484e2-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="484e2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="484e2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="484e2-117">Not supported.</span></span>    |
|<span data-ttu-id="484e2-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="484e2-118">Application</span></span> | <span data-ttu-id="484e2-119">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="484e2-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="484e2-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="484e2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="484e2-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="484e2-121">Request headers</span></span>
| <span data-ttu-id="484e2-122">名称</span><span class="sxs-lookup"><span data-stu-id="484e2-122">Name</span></span>       | <span data-ttu-id="484e2-123">类型</span><span class="sxs-lookup"><span data-stu-id="484e2-123">Type</span></span> | <span data-ttu-id="484e2-124">说明</span><span class="sxs-lookup"><span data-stu-id="484e2-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="484e2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="484e2-125">Authorization</span></span>  | <span data-ttu-id="484e2-126">string</span><span class="sxs-lookup"><span data-stu-id="484e2-126">string</span></span>  | <span data-ttu-id="484e2-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="484e2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="484e2-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="484e2-129">Request body</span></span>
<span data-ttu-id="484e2-130">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md) 或 [group](../resources/group.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="484e2-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="484e2-131">响应</span><span class="sxs-lookup"><span data-stu-id="484e2-131">Response</span></span>
<span data-ttu-id="484e2-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="484e2-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="484e2-134">示例</span><span class="sxs-lookup"><span data-stu-id="484e2-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="484e2-135">请求</span><span class="sxs-lookup"><span data-stu-id="484e2-135">Request</span></span>
<span data-ttu-id="484e2-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="484e2-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "add_group_member"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
<span data-ttu-id="484e2-137">在请求正文中，提供的 JSON 表示形式`id`您想要添加的[directoryObject](../resources/directoryobject.md)、[用户](../resources/user.md)或[组](../resources/group.md)对象。</span><span class="sxs-lookup"><span data-stu-id="484e2-137">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="484e2-138">响应</span><span class="sxs-lookup"><span data-stu-id="484e2-138">Response</span></span>
<span data-ttu-id="484e2-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="484e2-139">The following is an example of the response.</span></span>
><span data-ttu-id="484e2-140">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="484e2-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="484e2-141">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="484e2-141">All the properties will be returned from an actual call.</span></span>
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
