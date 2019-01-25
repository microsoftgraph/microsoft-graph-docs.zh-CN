---
title: 删除成员
description: 使用此 API 可以通过 **members** 导航属性从 Office 365 组、安全组或启用邮件的安全组中删除成员。可以删除用户或其他组。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: bda39ba1435d1368241db42a67b448fe178cef26
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524084"
---
# <a name="remove-member"></a><span data-ttu-id="6664d-104">删除成员</span><span class="sxs-lookup"><span data-stu-id="6664d-104">Remove member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6664d-p102">使用此 API 可以通过 **members** 导航属性从 Office 365 组、安全组或启用邮件的安全组中删除成员。可以删除用户或其他组。</span><span class="sxs-lookup"><span data-stu-id="6664d-p102">Use this API to remove a member from an Office 365 group, a security group, or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="6664d-107">权限</span><span class="sxs-lookup"><span data-stu-id="6664d-107">Permissions</span></span>
<span data-ttu-id="6664d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6664d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6664d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6664d-110">Permission type</span></span>      | <span data-ttu-id="6664d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6664d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6664d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6664d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6664d-113">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6664d-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6664d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6664d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6664d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6664d-115">Not supported.</span></span>    |
|<span data-ttu-id="6664d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6664d-116">Application</span></span> | <span data-ttu-id="6664d-117">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6664d-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6664d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6664d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="6664d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6664d-119">Request headers</span></span>
| <span data-ttu-id="6664d-120">名称</span><span class="sxs-lookup"><span data-stu-id="6664d-120">Name</span></span>       | <span data-ttu-id="6664d-121">类型</span><span class="sxs-lookup"><span data-stu-id="6664d-121">Type</span></span> | <span data-ttu-id="6664d-122">说明</span><span class="sxs-lookup"><span data-stu-id="6664d-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6664d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6664d-123">Authorization</span></span>  | <span data-ttu-id="6664d-124">string</span><span class="sxs-lookup"><span data-stu-id="6664d-124">string</span></span>  | <span data-ttu-id="6664d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6664d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6664d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6664d-127">Request body</span></span>
<span data-ttu-id="6664d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6664d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6664d-129">响应</span><span class="sxs-lookup"><span data-stu-id="6664d-129">Response</span></span>
<span data-ttu-id="6664d-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6664d-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6664d-132">示例</span><span class="sxs-lookup"><span data-stu-id="6664d-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6664d-133">请求</span><span class="sxs-lookup"><span data-stu-id="6664d-133">Request</span></span>
<span data-ttu-id="6664d-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6664d-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="6664d-135">在请求中，指定要在 $ref 段后删除的 directory 对象 `id`。</span><span class="sxs-lookup"><span data-stu-id="6664d-135">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="6664d-136">响应</span><span class="sxs-lookup"><span data-stu-id="6664d-136">Response</span></span>
<span data-ttu-id="6664d-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6664d-137">The following is an example of the response.</span></span>
><span data-ttu-id="6664d-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6664d-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6664d-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6664d-139">All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/group-delete-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
