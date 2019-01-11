---
title: 删除所有者
description: 使用此 API 可以通过 owners 导航属性从 Office 365 组、安全组或启用邮件的安全组中删除所有者。
localization_priority: Normal
ms.openlocfilehash: 7fe13b00d2e14bf69c1e3903f09d641d81f2dc0f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821649"
---
# <a name="remove-owner"></a><span data-ttu-id="5ffd5-103">删除所有者</span><span class="sxs-lookup"><span data-stu-id="5ffd5-103">Remove owner</span></span>
<span data-ttu-id="5ffd5-104">使用此 API 可以通过 owners 导航属性从 Office 365 组、安全组或启用邮件的安全组中删除所有者。</span><span class="sxs-lookup"><span data-stu-id="5ffd5-104">Use this API to remove an owner from an Office 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ffd5-105">权限</span><span class="sxs-lookup"><span data-stu-id="5ffd5-105">Permissions</span></span>
<span data-ttu-id="5ffd5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5ffd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ffd5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ffd5-108">Permission type</span></span>      | <span data-ttu-id="5ffd5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5ffd5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ffd5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ffd5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5ffd5-111">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5ffd5-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5ffd5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ffd5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ffd5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ffd5-113">Not supported.</span></span>    |
|<span data-ttu-id="5ffd5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ffd5-114">Application</span></span> | <span data-ttu-id="5ffd5-115">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ffd5-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ffd5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ffd5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="5ffd5-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ffd5-117">Request headers</span></span>
| <span data-ttu-id="5ffd5-118">名称</span><span class="sxs-lookup"><span data-stu-id="5ffd5-118">Name</span></span>       | <span data-ttu-id="5ffd5-119">类型</span><span class="sxs-lookup"><span data-stu-id="5ffd5-119">Type</span></span> | <span data-ttu-id="5ffd5-120">说明</span><span class="sxs-lookup"><span data-stu-id="5ffd5-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5ffd5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ffd5-121">Authorization</span></span>  | <span data-ttu-id="5ffd5-122">string</span><span class="sxs-lookup"><span data-stu-id="5ffd5-122">string</span></span>  | <span data-ttu-id="5ffd5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5ffd5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ffd5-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ffd5-125">Request body</span></span>
<span data-ttu-id="5ffd5-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5ffd5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ffd5-127">响应</span><span class="sxs-lookup"><span data-stu-id="5ffd5-127">Response</span></span>
<span data-ttu-id="5ffd5-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5ffd5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ffd5-130">示例</span><span class="sxs-lookup"><span data-stu-id="5ffd5-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5ffd5-131">请求</span><span class="sxs-lookup"><span data-stu-id="5ffd5-131">Request</span></span>
<span data-ttu-id="5ffd5-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5ffd5-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_owner_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/owners/{id}/$ref
```
<span data-ttu-id="5ffd5-133">在请求中，指定要在 $ref 段后删除的 directory 对象 `id`。</span><span class="sxs-lookup"><span data-stu-id="5ffd5-133">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="5ffd5-134">响应</span><span class="sxs-lookup"><span data-stu-id="5ffd5-134">Response</span></span>
<span data-ttu-id="5ffd5-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5ffd5-135">The following is an example of the response.</span></span>
><span data-ttu-id="5ffd5-136">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5ffd5-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5ffd5-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5ffd5-137">All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
