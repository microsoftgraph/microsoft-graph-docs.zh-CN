---
title: 升级团队中应用程序
description: 升级团队中的应用程序安装
author: nkramer
ms.openlocfilehash: 1e3ebffa9786d170424dd60618f553c515154140
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341438"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="663ed-103">升级团队中应用程序</span><span class="sxs-lookup"><span data-stu-id="663ed-103">Upgrade an app in a team</span></span>

> <span data-ttu-id="663ed-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="663ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="663ed-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="663ed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="663ed-106">升级[团队](../resources/team.md)中的[应用程序安装](../resources/teamsappinstallation.md)到最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="663ed-106">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="663ed-107">权限</span><span class="sxs-lookup"><span data-stu-id="663ed-107">Permissions</span></span>

<span data-ttu-id="663ed-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="663ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="663ed-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="663ed-110">Permission type</span></span>      | <span data-ttu-id="663ed-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="663ed-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="663ed-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="663ed-112">Delegated (work or school account)</span></span> | <span data-ttu-id="663ed-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="663ed-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="663ed-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="663ed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="663ed-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="663ed-115">Not supported.</span></span>    |
|<span data-ttu-id="663ed-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="663ed-116">Application</span></span> | <span data-ttu-id="663ed-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="663ed-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="663ed-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="663ed-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="663ed-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="663ed-119">Request headers</span></span>
| <span data-ttu-id="663ed-120">标头</span><span class="sxs-lookup"><span data-stu-id="663ed-120">Header</span></span>       | <span data-ttu-id="663ed-121">值</span><span class="sxs-lookup"><span data-stu-id="663ed-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="663ed-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="663ed-122">Authorization</span></span>  | <span data-ttu-id="663ed-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="663ed-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="663ed-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="663ed-125">Request body</span></span>
<span data-ttu-id="663ed-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="663ed-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="663ed-127">响应</span><span class="sxs-lookup"><span data-stu-id="663ed-127">Response</span></span>

<span data-ttu-id="663ed-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="663ed-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="663ed-130">示例</span><span class="sxs-lookup"><span data-stu-id="663ed-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="663ed-131">请求</span><span class="sxs-lookup"><span data-stu-id="663ed-131">Request</span></span>
<span data-ttu-id="663ed-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="663ed-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
#### <a name="response"></a><span data-ttu-id="663ed-133">响应</span><span class="sxs-lookup"><span data-stu-id="663ed-133">Response</span></span>
<span data-ttu-id="663ed-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="663ed-134">The following is an example of the response.</span></span> 

><span data-ttu-id="663ed-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="663ed-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
