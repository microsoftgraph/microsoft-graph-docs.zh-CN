---
title: 升级团队中的应用程序
description: 升级团队中的应用程序安装
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9ef5c41c8b09512b0ee6ebb888be1df1166cf9c5
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2019
ms.locfileid: "30056978"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="5edac-103">升级团队中的应用程序</span><span class="sxs-lookup"><span data-stu-id="5edac-103">Upgrade an app in a team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5edac-104">将[团队](../resources/team.md)中的[应用程序安装](../resources/teamsappinstallation.md)升级到最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="5edac-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

><span data-ttu-id="5edac-105">**注意:** 如果使用的是应用程序权限, 则会出现已知问题。</span><span class="sxs-lookup"><span data-stu-id="5edac-105">**Note:** If you're using application permissions, a known issue will occur.</span></span> <span data-ttu-id="5edac-106">有关详细信息，请参阅[已知问题](graph/concepts/known-issues.md)。</span><span class="sxs-lookup"><span data-stu-id="5edac-106">For details, see [known issues](graph/concepts/known-issues.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5edac-107">权限</span><span class="sxs-lookup"><span data-stu-id="5edac-107">Permissions</span></span>

<span data-ttu-id="5edac-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5edac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5edac-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5edac-110">Permission type</span></span>      | <span data-ttu-id="5edac-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5edac-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5edac-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5edac-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5edac-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5edac-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5edac-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5edac-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5edac-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5edac-115">Not supported.</span></span>    |
|<span data-ttu-id="5edac-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5edac-116">Application</span></span> | <span data-ttu-id="5edac-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5edac-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5edac-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5edac-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="5edac-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5edac-119">Request headers</span></span>
| <span data-ttu-id="5edac-120">标头</span><span class="sxs-lookup"><span data-stu-id="5edac-120">Header</span></span>       | <span data-ttu-id="5edac-121">值</span><span class="sxs-lookup"><span data-stu-id="5edac-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5edac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5edac-122">Authorization</span></span>  | <span data-ttu-id="5edac-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5edac-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5edac-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5edac-125">Request body</span></span>
<span data-ttu-id="5edac-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5edac-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5edac-127">响应</span><span class="sxs-lookup"><span data-stu-id="5edac-127">Response</span></span>

<span data-ttu-id="5edac-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5edac-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5edac-130">示例</span><span class="sxs-lookup"><span data-stu-id="5edac-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5edac-131">请求</span><span class="sxs-lookup"><span data-stu-id="5edac-131">Request</span></span>
<span data-ttu-id="5edac-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5edac-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
#### <a name="response"></a><span data-ttu-id="5edac-133">响应</span><span class="sxs-lookup"><span data-stu-id="5edac-133">Response</span></span>
<span data-ttu-id="5edac-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5edac-134">The following is an example of the response.</span></span> 

><span data-ttu-id="5edac-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5edac-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/teamsappinstallation-upgrade.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
