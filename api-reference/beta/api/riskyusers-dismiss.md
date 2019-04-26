---
title: 消除 riskyUsers
description: 消除 riskyUsers 对象的风险。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: 3027320b25c35e60e1b5dccabc7ff34ea642a953
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336338"
---
# <a name="dismiss-riskyusers"></a><span data-ttu-id="03e42-103">消除 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="03e42-103">Dismiss riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="03e42-104">**注意:** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="03e42-104">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="03e42-105">消除**riskyUser**对象的风险。</span><span class="sxs-lookup"><span data-stu-id="03e42-105">Dismiss the risk of a **riskyUser** object.</span></span> <span data-ttu-id="03e42-106">此操作会将目标用户的风险级别设置为 "无"。</span><span class="sxs-lookup"><span data-stu-id="03e42-106">This action will set the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="03e42-107">权限</span><span class="sxs-lookup"><span data-stu-id="03e42-107">Permissions</span></span>
<span data-ttu-id="03e42-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03e42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03e42-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="03e42-110">Permission type</span></span>      | <span data-ttu-id="03e42-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="03e42-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03e42-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03e42-112">Delegated (work or school account)</span></span> | <span data-ttu-id="03e42-113">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="03e42-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="03e42-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03e42-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03e42-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="03e42-115">Not supported.</span></span>    |
|<span data-ttu-id="03e42-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="03e42-116">Application</span></span> | <span data-ttu-id="03e42-117">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="03e42-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03e42-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03e42-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="03e42-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="03e42-119">Request headers</span></span>
| <span data-ttu-id="03e42-120">名称</span><span class="sxs-lookup"><span data-stu-id="03e42-120">Name</span></span>      |<span data-ttu-id="03e42-121">说明</span><span class="sxs-lookup"><span data-stu-id="03e42-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="03e42-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="03e42-122">Authorization</span></span>  | <span data-ttu-id="03e42-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="03e42-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03e42-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="03e42-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="03e42-126">用于确定是否保留更改的工作簿会话 ID。</span><span class="sxs-lookup"><span data-stu-id="03e42-126">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="03e42-127">可选。</span><span class="sxs-lookup"><span data-stu-id="03e42-127">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03e42-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="03e42-128">Request body</span></span>
<span data-ttu-id="03e42-129">在请求正文中指定要消除的 userIds。</span><span class="sxs-lookup"><span data-stu-id="03e42-129">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="03e42-130">响应</span><span class="sxs-lookup"><span data-stu-id="03e42-130">Response</span></span>

<span data-ttu-id="03e42-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="03e42-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="03e42-133">示例</span><span class="sxs-lookup"><span data-stu-id="03e42-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03e42-134">请求</span><span class="sxs-lookup"><span data-stu-id="03e42-134">Request</span></span>
<span data-ttu-id="03e42-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03e42-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "dismiss_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/dismiss
Content-Type: application/json

{
  "userIds": [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
  ]
}
```
##### <a name="response"></a><span data-ttu-id="03e42-136">响应</span><span class="sxs-lookup"><span data-stu-id="03e42-136">Response</span></span>
<span data-ttu-id="03e42-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="03e42-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Dismiss riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
