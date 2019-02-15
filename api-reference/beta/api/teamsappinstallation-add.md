---
title: 向团队添加应用
description: 将应用程序安装到指定的团队。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 35d2521d9bff37ea45f7496a825429762daaf8f7
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2019
ms.locfileid: "30056992"
---
# <a name="add-app-to-team"></a><span data-ttu-id="94d89-103">向团队添加应用</span><span class="sxs-lookup"><span data-stu-id="94d89-103">Add app to team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94d89-104">将[应用程序](../resources/teamsapp.md)安装到指定的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="94d89-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

><span data-ttu-id="94d89-105">**注意:** 如果使用的是应用程序权限, 则会出现已知问题。</span><span class="sxs-lookup"><span data-stu-id="94d89-105">**Note:** If you're using application permissions, a known issue will occur.</span></span> <span data-ttu-id="94d89-106">有关详细信息，请参阅[已知问题](graph/concepts/known-issues.md)。</span><span class="sxs-lookup"><span data-stu-id="94d89-106">For details, see [known issues](graph/concepts/known-issues.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="94d89-107">权限</span><span class="sxs-lookup"><span data-stu-id="94d89-107">Permissions</span></span>
<span data-ttu-id="94d89-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94d89-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94d89-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="94d89-110">Permission type</span></span>      | <span data-ttu-id="94d89-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94d89-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94d89-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94d89-112">Delegated (work or school account)</span></span> | <span data-ttu-id="94d89-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94d89-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="94d89-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94d89-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94d89-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="94d89-115">Not supported.</span></span>    |
|<span data-ttu-id="94d89-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="94d89-116">Application</span></span> | <span data-ttu-id="94d89-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94d89-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94d89-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94d89-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="94d89-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="94d89-119">Request headers</span></span>
| <span data-ttu-id="94d89-120">标头</span><span class="sxs-lookup"><span data-stu-id="94d89-120">Header</span></span>       | <span data-ttu-id="94d89-121">值</span><span class="sxs-lookup"><span data-stu-id="94d89-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="94d89-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="94d89-122">Authorization</span></span>  | <span data-ttu-id="94d89-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94d89-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="94d89-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="94d89-125">Request body</span></span>

| <span data-ttu-id="94d89-126">属性</span><span class="sxs-lookup"><span data-stu-id="94d89-126">Property</span></span>     | <span data-ttu-id="94d89-127">类型</span><span class="sxs-lookup"><span data-stu-id="94d89-127">Type</span></span>   |<span data-ttu-id="94d89-128">说明</span><span class="sxs-lookup"><span data-stu-id="94d89-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94d89-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="94d89-129">teamsApp</span></span>|<span data-ttu-id="94d89-130">字符串</span><span class="sxs-lookup"><span data-stu-id="94d89-130">String</span></span>|<span data-ttu-id="94d89-131">要添加的应用程序的 id。</span><span class="sxs-lookup"><span data-stu-id="94d89-131">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="94d89-132">响应</span><span class="sxs-lookup"><span data-stu-id="94d89-132">Response</span></span>

<span data-ttu-id="94d89-133">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="94d89-133">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="94d89-134">示例</span><span class="sxs-lookup"><span data-stu-id="94d89-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="94d89-135">请求</span><span class="sxs-lookup"><span data-stu-id="94d89-135">Request</span></span>
<span data-ttu-id="94d89-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="94d89-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/installedApps
{
   "teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
#### <a name="response"></a><span data-ttu-id="94d89-137">响应</span><span class="sxs-lookup"><span data-stu-id="94d89-137">Response</span></span>
<span data-ttu-id="94d89-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="94d89-138">The following is an example of the response.</span></span> <span data-ttu-id="94d89-139">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="94d89-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="94d89-140">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="94d89-140">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
}
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
    "Error: /api-reference/beta/api/teamsappinstallation-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

## <a name="see-also"></a><span data-ttu-id="94d89-141">另请参阅</span><span class="sxs-lookup"><span data-stu-id="94d89-141">See also</span></span>

