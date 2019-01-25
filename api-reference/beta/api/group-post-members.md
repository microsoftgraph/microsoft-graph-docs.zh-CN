---
title: 添加成员
description: 使用此 API 可以通过 **members** 导航属性将成员添加到 Office 365 组、安全组或启用邮件的安全组中。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: ac21262858137074ed92978f0ab6530052fcc2de
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515676"
---
# <a name="add-member"></a><span data-ttu-id="290a9-103">添加成员</span><span class="sxs-lookup"><span data-stu-id="290a9-103">Add member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="290a9-104">使用此 API 可以通过 **members** 导航属性将成员添加到 Office 365 组、安全组或启用邮件的安全组中。</span><span class="sxs-lookup"><span data-stu-id="290a9-104">Use this API to add a member to an Office 365 Group, a security group, or a mail-enabled security group through the **members** navigation property.</span></span>

<span data-ttu-id="290a9-105">可以添加用户或其他组。</span><span class="sxs-lookup"><span data-stu-id="290a9-105">You can add users or other groups.</span></span> <span data-ttu-id="290a9-106">重要说明：只能将用户添加到 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="290a9-106">Important: You can add only users to Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="290a9-107">权限</span><span class="sxs-lookup"><span data-stu-id="290a9-107">Permissions</span></span>
<span data-ttu-id="290a9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="290a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="290a9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="290a9-110">Permission type</span></span>      | <span data-ttu-id="290a9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="290a9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="290a9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="290a9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="290a9-113">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="290a9-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="290a9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="290a9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="290a9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="290a9-115">Not supported.</span></span>    |
|<span data-ttu-id="290a9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="290a9-116">Application</span></span> | <span data-ttu-id="290a9-117">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="290a9-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="290a9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="290a9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="290a9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="290a9-119">Request headers</span></span>
| <span data-ttu-id="290a9-120">名称</span><span class="sxs-lookup"><span data-stu-id="290a9-120">Name</span></span>       | <span data-ttu-id="290a9-121">类型</span><span class="sxs-lookup"><span data-stu-id="290a9-121">Type</span></span> | <span data-ttu-id="290a9-122">说明</span><span class="sxs-lookup"><span data-stu-id="290a9-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="290a9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="290a9-123">Authorization</span></span>  | <span data-ttu-id="290a9-124">string</span><span class="sxs-lookup"><span data-stu-id="290a9-124">string</span></span>  | <span data-ttu-id="290a9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="290a9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="290a9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="290a9-127">Request body</span></span>
<span data-ttu-id="290a9-128">在请求正文中，提供要添加的 [directoryObject](../resources/directoryobject.md)、[user](../resources/user.md) 或 [group](../resources/group.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="290a9-128">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="290a9-129">响应</span><span class="sxs-lookup"><span data-stu-id="290a9-129">Response</span></span>
<span data-ttu-id="290a9-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="290a9-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="290a9-132">示例</span><span class="sxs-lookup"><span data-stu-id="290a9-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="290a9-133">请求</span><span class="sxs-lookup"><span data-stu-id="290a9-133">Request</span></span>
<span data-ttu-id="290a9-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="290a9-134">The following is an example of the request.</span></span>
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
<span data-ttu-id="290a9-135">在请求正文中，提供的 JSON 表示形式`id`您想要添加的[directoryObject](../resources/directoryobject.md)、[用户](../resources/user.md)或[组](../resources/group.md)对象。</span><span class="sxs-lookup"><span data-stu-id="290a9-135">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

#### <a name="response"></a><span data-ttu-id="290a9-136">响应</span><span class="sxs-lookup"><span data-stu-id="290a9-136">Response</span></span>
<span data-ttu-id="290a9-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="290a9-137">The following is an example of the response.</span></span>
><span data-ttu-id="290a9-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="290a9-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="290a9-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="290a9-139">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
