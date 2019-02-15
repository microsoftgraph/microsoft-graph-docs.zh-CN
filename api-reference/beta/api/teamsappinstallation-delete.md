---
title: 从团队中删除应用程序
description: 从指定的团队中卸载应用程序。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: aa75f72375432609afb748959cb82ff63fa1b721
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057020"
---
# <a name="delete-app-from-team"></a><span data-ttu-id="cdf99-103">从团队中删除应用程序</span><span class="sxs-lookup"><span data-stu-id="cdf99-103">Delete app from team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdf99-104">从指定的[团队](../resources/team.md)中卸载[应用程序](../resources/teamsappinstallation.md)。</span><span class="sxs-lookup"><span data-stu-id="cdf99-104">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

><span data-ttu-id="cdf99-105">**注意:** 如果使用的是应用程序权限, 则会出现已知问题。</span><span class="sxs-lookup"><span data-stu-id="cdf99-105">**Note:** If you're using application permissions, a known issue will occur.</span></span> <span data-ttu-id="cdf99-106">有关详细信息，请参阅[已知问题](graph/concepts/known-issues.md)。</span><span class="sxs-lookup"><span data-stu-id="cdf99-106">For details, see [known issues](graph/concepts/known-issues.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cdf99-107">权限</span><span class="sxs-lookup"><span data-stu-id="cdf99-107">Permissions</span></span>
<span data-ttu-id="cdf99-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cdf99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdf99-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cdf99-110">Permission type</span></span>      | <span data-ttu-id="cdf99-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cdf99-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdf99-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cdf99-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cdf99-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdf99-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cdf99-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cdf99-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdf99-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cdf99-115">Not supported.</span></span>    |
|<span data-ttu-id="cdf99-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cdf99-116">Application</span></span> | <span data-ttu-id="cdf99-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdf99-117">Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="cdf99-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cdf99-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cdf99-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cdf99-119">Request headers</span></span>
| <span data-ttu-id="cdf99-120">标头</span><span class="sxs-lookup"><span data-stu-id="cdf99-120">Header</span></span>       | <span data-ttu-id="cdf99-121">值</span><span class="sxs-lookup"><span data-stu-id="cdf99-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cdf99-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdf99-122">Authorization</span></span>  | <span data-ttu-id="cdf99-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cdf99-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cdf99-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="cdf99-125">Request body</span></span>
<span data-ttu-id="cdf99-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cdf99-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdf99-127">响应</span><span class="sxs-lookup"><span data-stu-id="cdf99-127">Response</span></span>

<span data-ttu-id="cdf99-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cdf99-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdf99-130">示例</span><span class="sxs-lookup"><span data-stu-id="cdf99-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cdf99-131">请求</span><span class="sxs-lookup"><span data-stu-id="cdf99-131">Request</span></span>
<span data-ttu-id="cdf99-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cdf99-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
#### <a name="response"></a><span data-ttu-id="cdf99-133">响应</span><span class="sxs-lookup"><span data-stu-id="cdf99-133">Response</span></span>
<span data-ttu-id="cdf99-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cdf99-134">The following is an example of the response.</span></span> <span data-ttu-id="cdf99-135">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cdf99-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cdf99-136">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cdf99-136">All of the properties will be returned from an actual call.</span></span>
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
