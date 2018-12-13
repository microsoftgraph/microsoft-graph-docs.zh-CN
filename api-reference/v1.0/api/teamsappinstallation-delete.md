---
title: 从工作组中删除应用程序
description: 从指定的团队中卸载应用程序。
ms.openlocfilehash: f9e04ad9d6672c3b9cfaaee9109b1bba0f7ab4c6
ms.sourcegitcommit: ba6b1d1a12dcb54916b4d3e529c856f6514e01e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/12/2018
ms.locfileid: "27241053"
---
# <a name="delete-app-from-team"></a><span data-ttu-id="b376b-103">从工作组中删除应用程序</span><span class="sxs-lookup"><span data-stu-id="b376b-103">Delete app from team</span></span>



<span data-ttu-id="b376b-104">从指定的[团队](../resources/team.md)中卸载[应用程序](../resources/teamsappinstallation.md)。</span><span class="sxs-lookup"><span data-stu-id="b376b-104">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b376b-105">权限</span><span class="sxs-lookup"><span data-stu-id="b376b-105">Permissions</span></span>
<span data-ttu-id="b376b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b376b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b376b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b376b-108">Permission type</span></span>      | <span data-ttu-id="b376b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b376b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b376b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b376b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b376b-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b376b-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b376b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b376b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b376b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b376b-113">Not supported.</span></span>    |
|<span data-ttu-id="b376b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b376b-114">Application</span></span> | <span data-ttu-id="b376b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b376b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b376b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b376b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b376b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b376b-117">Request headers</span></span>
| <span data-ttu-id="b376b-118">标头</span><span class="sxs-lookup"><span data-stu-id="b376b-118">Header</span></span>       | <span data-ttu-id="b376b-119">值</span><span class="sxs-lookup"><span data-stu-id="b376b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b376b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b376b-120">Authorization</span></span>  | <span data-ttu-id="b376b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b376b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b376b-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b376b-123">Request body</span></span>
<span data-ttu-id="b376b-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b376b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b376b-125">响应</span><span class="sxs-lookup"><span data-stu-id="b376b-125">Response</span></span>

<span data-ttu-id="b376b-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b376b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b376b-128">示例</span><span class="sxs-lookup"><span data-stu-id="b376b-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b376b-129">请求</span><span class="sxs-lookup"><span data-stu-id="b376b-129">Request</span></span>
<span data-ttu-id="b376b-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b376b-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE /teams/{id}/installedApps/{id}
```
#### <a name="response"></a><span data-ttu-id="b376b-131">响应</span><span class="sxs-lookup"><span data-stu-id="b376b-131">Response</span></span>
<span data-ttu-id="b376b-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b376b-132">The following is an example of the response.</span></span> <span data-ttu-id="b376b-133">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b376b-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b376b-134">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b376b-134">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
