---
title: 将应用程序添加到团队
description: 将应用程序安装到指定的团队。
ms.openlocfilehash: f3cf62163747bd1a288b59a39e5ff1fc9d82783b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046636"
---
# <a name="add-app-to-team"></a><span data-ttu-id="a0802-103">将应用程序添加到团队</span><span class="sxs-lookup"><span data-stu-id="a0802-103">Add app to team</span></span>

> <span data-ttu-id="a0802-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a0802-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0802-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a0802-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a0802-106">将[应用程序](../resources/teamsapp.md)安装到指定的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="a0802-106">Installs an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a0802-107">权限</span><span class="sxs-lookup"><span data-stu-id="a0802-107">Permissions</span></span>
<span data-ttu-id="a0802-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0802-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0802-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0802-110">Permission type</span></span>      | <span data-ttu-id="a0802-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0802-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0802-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0802-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a0802-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0802-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a0802-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0802-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0802-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0802-115">Not supported.</span></span>    |
|<span data-ttu-id="a0802-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0802-116">Application</span></span> | <span data-ttu-id="a0802-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0802-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0802-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0802-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="a0802-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0802-119">Request headers</span></span>
| <span data-ttu-id="a0802-120">标头</span><span class="sxs-lookup"><span data-stu-id="a0802-120">Header</span></span>       | <span data-ttu-id="a0802-121">值</span><span class="sxs-lookup"><span data-stu-id="a0802-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a0802-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0802-122">Authorization</span></span>  | <span data-ttu-id="a0802-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a0802-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a0802-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0802-125">Request body</span></span>

| <span data-ttu-id="a0802-126">属性</span><span class="sxs-lookup"><span data-stu-id="a0802-126">Property</span></span>     | <span data-ttu-id="a0802-127">类型</span><span class="sxs-lookup"><span data-stu-id="a0802-127">Type</span></span>   |<span data-ttu-id="a0802-128">说明</span><span class="sxs-lookup"><span data-stu-id="a0802-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0802-129">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a0802-129">teamsApp</span></span>|<span data-ttu-id="a0802-130">字符串</span><span class="sxs-lookup"><span data-stu-id="a0802-130">String</span></span>|<span data-ttu-id="a0802-131">添加应用程序的 id。</span><span class="sxs-lookup"><span data-stu-id="a0802-131">The id of the app to add.</span></span>|


## <a name="response"></a><span data-ttu-id="a0802-132">响应</span><span class="sxs-lookup"><span data-stu-id="a0802-132">Response</span></span>

<span data-ttu-id="a0802-133">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a0802-133">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="a0802-134">示例</span><span class="sxs-lookup"><span data-stu-id="a0802-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a0802-135">请求</span><span class="sxs-lookup"><span data-stu-id="a0802-135">Request</span></span>
<span data-ttu-id="a0802-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a0802-136">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="a0802-137">响应</span><span class="sxs-lookup"><span data-stu-id="a0802-137">Response</span></span>
<span data-ttu-id="a0802-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a0802-138">The following is an example of the response.</span></span> <span data-ttu-id="a0802-139">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a0802-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a0802-140">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a0802-140">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="a0802-141">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a0802-141">See also</span></span>

