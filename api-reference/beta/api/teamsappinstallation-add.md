---
title: 向团队添加应用
description: 将应用程序安装到指定的团队。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1a77d3b01c70273d0d93ca1e3b1b66d1de53f8f0
ms.sourcegitcommit: d1a9e7c8e1376a99c5a5416257889ec113613a77
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/07/2019
ms.locfileid: "30458671"
---
# <a name="add-app-to-team"></a><span data-ttu-id="0f712-103">向团队添加应用</span><span class="sxs-lookup"><span data-stu-id="0f712-103">Add app to team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f712-104">将[应用程序](../resources/teamsapp.md)安装到指定的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="0f712-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0f712-105">权限</span><span class="sxs-lookup"><span data-stu-id="0f712-105">Permissions</span></span>
<span data-ttu-id="0f712-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0f712-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f712-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f712-108">Permission type</span></span>      | <span data-ttu-id="0f712-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0f712-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f712-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f712-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0f712-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f712-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0f712-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f712-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f712-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f712-113">Not supported.</span></span>    |
|<span data-ttu-id="0f712-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f712-114">Application</span></span> | <span data-ttu-id="0f712-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f712-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f712-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f712-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="0f712-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0f712-117">Request headers</span></span>
| <span data-ttu-id="0f712-118">标头</span><span class="sxs-lookup"><span data-stu-id="0f712-118">Header</span></span>       | <span data-ttu-id="0f712-119">值</span><span class="sxs-lookup"><span data-stu-id="0f712-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0f712-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f712-120">Authorization</span></span>  | <span data-ttu-id="0f712-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0f712-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0f712-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f712-123">Request body</span></span>

| <span data-ttu-id="0f712-124">属性</span><span class="sxs-lookup"><span data-stu-id="0f712-124">Property</span></span>     | <span data-ttu-id="0f712-125">类型</span><span class="sxs-lookup"><span data-stu-id="0f712-125">Type</span></span>   |<span data-ttu-id="0f712-126">说明</span><span class="sxs-lookup"><span data-stu-id="0f712-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f712-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0f712-127">teamsApp</span></span>|<span data-ttu-id="0f712-128">String</span><span class="sxs-lookup"><span data-stu-id="0f712-128">String</span></span>|<span data-ttu-id="0f712-129">要添加的应用程序的 id。</span><span class="sxs-lookup"><span data-stu-id="0f712-129">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="0f712-130">响应</span><span class="sxs-lookup"><span data-stu-id="0f712-130">Response</span></span>

<span data-ttu-id="0f712-131">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0f712-131">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="0f712-132">示例</span><span class="sxs-lookup"><span data-stu-id="0f712-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0f712-133">请求</span><span class="sxs-lookup"><span data-stu-id="0f712-133">Request</span></span>
<span data-ttu-id="0f712-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0f712-134">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="0f712-135">响应</span><span class="sxs-lookup"><span data-stu-id="0f712-135">Response</span></span>
<span data-ttu-id="0f712-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0f712-136">The following is an example of the response.</span></span> <span data-ttu-id="0f712-137">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0f712-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0f712-138">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0f712-138">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="0f712-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0f712-139">See also</span></span>

