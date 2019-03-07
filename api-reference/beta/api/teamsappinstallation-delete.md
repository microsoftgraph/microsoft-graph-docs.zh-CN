---
title: 从团队中删除应用程序
description: 从指定的团队中卸载应用程序。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 592f488ad73337cc89b92d5a57bd874664fba9cf
ms.sourcegitcommit: d1a9e7c8e1376a99c5a5416257889ec113613a77
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/07/2019
ms.locfileid: "30458664"
---
# <a name="delete-app-from-team"></a><span data-ttu-id="76247-103">从团队中删除应用程序</span><span class="sxs-lookup"><span data-stu-id="76247-103">Delete app from team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76247-104">从指定的[团队](../resources/team.md)中卸载[应用程序](../resources/teamsappinstallation.md)。</span><span class="sxs-lookup"><span data-stu-id="76247-104">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="76247-105">权限</span><span class="sxs-lookup"><span data-stu-id="76247-105">Permissions</span></span>
<span data-ttu-id="76247-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76247-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76247-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="76247-108">Permission type</span></span>      | <span data-ttu-id="76247-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="76247-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76247-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76247-110">Delegated (work or school account)</span></span> | <span data-ttu-id="76247-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76247-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="76247-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76247-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76247-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="76247-113">Not supported.</span></span>    |
|<span data-ttu-id="76247-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="76247-114">Application</span></span> | <span data-ttu-id="76247-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76247-115">Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="76247-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76247-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="76247-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="76247-117">Request headers</span></span>
| <span data-ttu-id="76247-118">标头</span><span class="sxs-lookup"><span data-stu-id="76247-118">Header</span></span>       | <span data-ttu-id="76247-119">值</span><span class="sxs-lookup"><span data-stu-id="76247-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="76247-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="76247-120">Authorization</span></span>  | <span data-ttu-id="76247-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="76247-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="76247-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="76247-123">Request body</span></span>
<span data-ttu-id="76247-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="76247-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76247-125">响应</span><span class="sxs-lookup"><span data-stu-id="76247-125">Response</span></span>

<span data-ttu-id="76247-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="76247-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76247-128">示例</span><span class="sxs-lookup"><span data-stu-id="76247-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="76247-129">请求</span><span class="sxs-lookup"><span data-stu-id="76247-129">Request</span></span>
<span data-ttu-id="76247-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="76247-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
#### <a name="response"></a><span data-ttu-id="76247-131">响应</span><span class="sxs-lookup"><span data-stu-id="76247-131">Response</span></span>
<span data-ttu-id="76247-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="76247-132">The following is an example of the response.</span></span> <span data-ttu-id="76247-133">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="76247-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="76247-134">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="76247-134">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsappinstallation-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
