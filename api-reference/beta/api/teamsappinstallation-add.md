---
title: 将应用添加到团队
description: 将应用程序安装到指定的团队。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 353298dc43479057e689f43e3a7274523468caee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516824"
---
# <a name="add-app-to-team"></a><span data-ttu-id="03b01-103">将应用添加到团队</span><span class="sxs-lookup"><span data-stu-id="03b01-103">Add app to team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03b01-104">将[应用程序](../resources/teamsapp.md)安装到指定的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="03b01-104">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="03b01-105">权限</span><span class="sxs-lookup"><span data-stu-id="03b01-105">Permissions</span></span>
<span data-ttu-id="03b01-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03b01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03b01-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="03b01-108">Permission type</span></span>      | <span data-ttu-id="03b01-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="03b01-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03b01-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03b01-110">Delegated (work or school account)</span></span> | <span data-ttu-id="03b01-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03b01-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="03b01-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03b01-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03b01-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="03b01-113">Not supported.</span></span>    |
|<span data-ttu-id="03b01-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="03b01-114">Application</span></span> | <span data-ttu-id="03b01-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="03b01-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="03b01-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03b01-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="03b01-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="03b01-117">Request headers</span></span>
| <span data-ttu-id="03b01-118">标头</span><span class="sxs-lookup"><span data-stu-id="03b01-118">Header</span></span>       | <span data-ttu-id="03b01-119">值</span><span class="sxs-lookup"><span data-stu-id="03b01-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="03b01-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="03b01-120">Authorization</span></span>  | <span data-ttu-id="03b01-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="03b01-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="03b01-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="03b01-123">Request body</span></span>

| <span data-ttu-id="03b01-124">属性</span><span class="sxs-lookup"><span data-stu-id="03b01-124">Property</span></span>     | <span data-ttu-id="03b01-125">类型</span><span class="sxs-lookup"><span data-stu-id="03b01-125">Type</span></span>   |<span data-ttu-id="03b01-126">说明</span><span class="sxs-lookup"><span data-stu-id="03b01-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03b01-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="03b01-127">teamsApp</span></span>|<span data-ttu-id="03b01-128">String</span><span class="sxs-lookup"><span data-stu-id="03b01-128">String</span></span>|<span data-ttu-id="03b01-129">添加应用程序的 id。</span><span class="sxs-lookup"><span data-stu-id="03b01-129">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="03b01-130">响应</span><span class="sxs-lookup"><span data-stu-id="03b01-130">Response</span></span>

<span data-ttu-id="03b01-131">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="03b01-131">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="03b01-132">示例</span><span class="sxs-lookup"><span data-stu-id="03b01-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="03b01-133">请求</span><span class="sxs-lookup"><span data-stu-id="03b01-133">Request</span></span>
<span data-ttu-id="03b01-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="03b01-134">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="03b01-135">响应</span><span class="sxs-lookup"><span data-stu-id="03b01-135">Response</span></span>
<span data-ttu-id="03b01-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="03b01-136">The following is an example of the response.</span></span> <span data-ttu-id="03b01-137">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="03b01-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="03b01-138">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="03b01-138">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="03b01-139">另请参阅</span><span class="sxs-lookup"><span data-stu-id="03b01-139">See also</span></span>

