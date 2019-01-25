---
title: 删除组
description: 删除组。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 349900cffa4b0df1763e1ed8b8213ce81ec27351
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529962"
---
# <a name="delete-group"></a><span data-ttu-id="16563-103">删除组</span><span class="sxs-lookup"><span data-stu-id="16563-103">Delete group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16563-104">删除组。</span><span class="sxs-lookup"><span data-stu-id="16563-104">Deletes a group.</span></span>

<span data-ttu-id="16563-105">删除组后，项目添加到[已删除项目](../resources/directory.md)。</span><span class="sxs-lookup"><span data-stu-id="16563-105">When a group is deleted, the item is added to [deleted items](../resources/directory.md).</span></span> <span data-ttu-id="16563-106">组将已删除的项目中保持最多 30 天。</span><span class="sxs-lookup"><span data-stu-id="16563-106">The group will remain in deleted items for up to 30 days.</span></span> <span data-ttu-id="16563-107">组可以完全从还原已删除项目在 30 天。</span><span class="sxs-lookup"><span data-stu-id="16563-107">A group can be fully restored from deleted items during the 30 days.</span></span> <span data-ttu-id="16563-108">30 天后删除的项目被永久删除。</span><span class="sxs-lookup"><span data-stu-id="16563-108">After 30 days, deleted items are permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="16563-109">权限</span><span class="sxs-lookup"><span data-stu-id="16563-109">Permissions</span></span>
<span data-ttu-id="16563-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16563-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16563-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="16563-112">Permission type</span></span>      | <span data-ttu-id="16563-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16563-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16563-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16563-114">Delegated (work or school account)</span></span> | <span data-ttu-id="16563-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16563-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="16563-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16563-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16563-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="16563-117">Not supported.</span></span>    |
|<span data-ttu-id="16563-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="16563-118">Application</span></span> | <span data-ttu-id="16563-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16563-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16563-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16563-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="16563-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="16563-121">Request headers</span></span>
| <span data-ttu-id="16563-122">名称</span><span class="sxs-lookup"><span data-stu-id="16563-122">Name</span></span>       | <span data-ttu-id="16563-123">类型</span><span class="sxs-lookup"><span data-stu-id="16563-123">Type</span></span> | <span data-ttu-id="16563-124">说明</span><span class="sxs-lookup"><span data-stu-id="16563-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="16563-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="16563-125">Authorization</span></span>  | <span data-ttu-id="16563-126">string</span><span class="sxs-lookup"><span data-stu-id="16563-126">string</span></span>  | <span data-ttu-id="16563-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="16563-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16563-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="16563-129">Request body</span></span>
<span data-ttu-id="16563-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="16563-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16563-131">响应</span><span class="sxs-lookup"><span data-stu-id="16563-131">Response</span></span>
<span data-ttu-id="16563-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="16563-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16563-134">示例</span><span class="sxs-lookup"><span data-stu-id="16563-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="16563-135">请求</span><span class="sxs-lookup"><span data-stu-id="16563-135">Request</span></span>
<span data-ttu-id="16563-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="16563-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="16563-137">响应</span><span class="sxs-lookup"><span data-stu-id="16563-137">Response</span></span>
<span data-ttu-id="16563-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="16563-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
