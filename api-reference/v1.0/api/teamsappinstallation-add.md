---
title: 向团队添加应用
description: 将应用程序安装到指定的团队。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 07e8a5989050a0323fdbcde8027e6c89bef0d454
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908462"
---
# <a name="add-app-to-team"></a><span data-ttu-id="acf79-103">向团队添加应用</span><span class="sxs-lookup"><span data-stu-id="acf79-103">Add app to team</span></span>

<span data-ttu-id="acf79-104">将[应用程序](../resources/teamsapp.md)安装到指定的[团队](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="acf79-104">Install an [app](../resources/teamsapp.md) to the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="acf79-105">权限</span><span class="sxs-lookup"><span data-stu-id="acf79-105">Permissions</span></span>

<span data-ttu-id="acf79-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="acf79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acf79-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="acf79-108">Permission type</span></span>      | <span data-ttu-id="acf79-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="acf79-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="acf79-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="acf79-110">Delegated (work or school account)</span></span> | <span data-ttu-id="acf79-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acf79-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="acf79-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="acf79-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acf79-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="acf79-113">Not supported.</span></span>    |
|<span data-ttu-id="acf79-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="acf79-114">Application</span></span> | <span data-ttu-id="acf79-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acf79-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="acf79-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="acf79-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="acf79-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="acf79-117">Request headers</span></span>

| <span data-ttu-id="acf79-118">标头</span><span class="sxs-lookup"><span data-stu-id="acf79-118">Header</span></span>       | <span data-ttu-id="acf79-119">值</span><span class="sxs-lookup"><span data-stu-id="acf79-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="acf79-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="acf79-120">Authorization</span></span>  | <span data-ttu-id="acf79-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="acf79-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="acf79-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="acf79-123">Request body</span></span>

| <span data-ttu-id="acf79-124">属性</span><span class="sxs-lookup"><span data-stu-id="acf79-124">Property</span></span>   | <span data-ttu-id="acf79-125">类型</span><span class="sxs-lookup"><span data-stu-id="acf79-125">Type</span></span> |<span data-ttu-id="acf79-126">说明</span><span class="sxs-lookup"><span data-stu-id="acf79-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acf79-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="acf79-127">teamsApp</span></span>| [<span data-ttu-id="acf79-128">teamsApp</span><span class="sxs-lookup"><span data-stu-id="acf79-128">teamsApp</span></span>](../resources/teamsapp.md) |<span data-ttu-id="acf79-129">要添加的应用程序。</span><span class="sxs-lookup"><span data-stu-id="acf79-129">The app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="acf79-130">响应</span><span class="sxs-lookup"><span data-stu-id="acf79-130">Response</span></span>

<span data-ttu-id="acf79-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="acf79-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acf79-133">示例</span><span class="sxs-lookup"><span data-stu-id="acf79-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="acf79-134">请求</span><span class="sxs-lookup"><span data-stu-id="acf79-134">Request</span></span>

<span data-ttu-id="acf79-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="acf79-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```

### <a name="response"></a><span data-ttu-id="acf79-136">响应</span><span class="sxs-lookup"><span data-stu-id="acf79-136">Response</span></span>

<span data-ttu-id="acf79-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="acf79-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
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
