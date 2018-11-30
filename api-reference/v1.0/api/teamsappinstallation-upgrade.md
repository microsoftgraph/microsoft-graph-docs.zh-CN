---
title: 升级团队中应用程序
description: 升级团队中的应用程序安装
ms.openlocfilehash: 37f42a307b2f86e7a447e3df05030e94495eaa6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008271"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="9db37-103">升级团队中应用程序</span><span class="sxs-lookup"><span data-stu-id="9db37-103">Upgrade an app in a team</span></span>



<span data-ttu-id="9db37-104">升级[团队](../resources/team.md)中的[应用程序安装](../resources/teamsappinstallation.md)到最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="9db37-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="9db37-105">权限</span><span class="sxs-lookup"><span data-stu-id="9db37-105">Permissions</span></span>

<span data-ttu-id="9db37-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9db37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9db37-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9db37-108">Permission type</span></span>      | <span data-ttu-id="9db37-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9db37-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9db37-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9db37-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9db37-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9db37-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9db37-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9db37-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9db37-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9db37-113">Not supported.</span></span>    |
|<span data-ttu-id="9db37-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9db37-114">Application</span></span> | <span data-ttu-id="9db37-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9db37-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9db37-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9db37-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="9db37-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9db37-117">Request headers</span></span>
| <span data-ttu-id="9db37-118">标头</span><span class="sxs-lookup"><span data-stu-id="9db37-118">Header</span></span>       | <span data-ttu-id="9db37-119">值</span><span class="sxs-lookup"><span data-stu-id="9db37-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9db37-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9db37-120">Authorization</span></span>  | <span data-ttu-id="9db37-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9db37-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9db37-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="9db37-123">Request body</span></span>
<span data-ttu-id="9db37-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9db37-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9db37-125">响应</span><span class="sxs-lookup"><span data-stu-id="9db37-125">Response</span></span>

<span data-ttu-id="9db37-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9db37-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9db37-128">示例</span><span class="sxs-lookup"><span data-stu-id="9db37-128">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9db37-129">请求</span><span class="sxs-lookup"><span data-stu-id="9db37-129">Request</span></span>
<span data-ttu-id="9db37-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9db37-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
#### <a name="response"></a><span data-ttu-id="9db37-131">响应</span><span class="sxs-lookup"><span data-stu-id="9db37-131">Response</span></span>
<span data-ttu-id="9db37-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9db37-132">The following is an example of the response.</span></span> 

><span data-ttu-id="9db37-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9db37-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
