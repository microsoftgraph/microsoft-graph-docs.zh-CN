---
title: 消除 riskyUsers
description: 消除 riskyUsers 对象的风险。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: 8e7a64e5762808691c4997c83b112a17c9667d47
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/30/2019
ms.locfileid: "31013129"
---
# <a name="dismiss-riskyusers"></a><span data-ttu-id="4c76b-103">消除 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="4c76b-103">Dismiss riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="4c76b-104">**注意:** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="4c76b-104">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="4c76b-105">消除**riskyUsers**对象的风险。</span><span class="sxs-lookup"><span data-stu-id="4c76b-105">Dismiss the risk of a **riskyUsers** object.</span></span> <span data-ttu-id="4c76b-106">此操作会将目标用户的风险级别设置为 "无"。</span><span class="sxs-lookup"><span data-stu-id="4c76b-106">This action will set the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="4c76b-107">权限</span><span class="sxs-lookup"><span data-stu-id="4c76b-107">Permissions</span></span>
<span data-ttu-id="4c76b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4c76b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c76b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c76b-110">Permission type</span></span>      | <span data-ttu-id="4c76b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4c76b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c76b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c76b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4c76b-113">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="4c76b-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="4c76b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c76b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c76b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c76b-115">Not supported.</span></span>    |
|<span data-ttu-id="4c76b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4c76b-116">Application</span></span> | <span data-ttu-id="4c76b-117">IdentityRiskyUser</span><span class="sxs-lookup"><span data-stu-id="4c76b-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c76b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c76b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="4c76b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4c76b-119">Request headers</span></span>
| <span data-ttu-id="4c76b-120">名称</span><span class="sxs-lookup"><span data-stu-id="4c76b-120">Name</span></span>      |<span data-ttu-id="4c76b-121">说明</span><span class="sxs-lookup"><span data-stu-id="4c76b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4c76b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c76b-122">Authorization</span></span>  | <span data-ttu-id="4c76b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4c76b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4c76b-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4c76b-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="4c76b-126">用于确定是否保留更改的工作簿会话 ID。</span><span class="sxs-lookup"><span data-stu-id="4c76b-126">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="4c76b-127">可选。</span><span class="sxs-lookup"><span data-stu-id="4c76b-127">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c76b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4c76b-128">Request body</span></span>
<span data-ttu-id="4c76b-129">在请求正文中指定要消除的 userIds。</span><span class="sxs-lookup"><span data-stu-id="4c76b-129">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="4c76b-130">响应</span><span class="sxs-lookup"><span data-stu-id="4c76b-130">Response</span></span>

<span data-ttu-id="4c76b-131">如果成功，此方法返回 `204 NoContent` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4c76b-131">If successful, this method returns a `204 NoContent` response code.</span></span>
## <a name="example"></a><span data-ttu-id="4c76b-132">示例</span><span class="sxs-lookup"><span data-stu-id="4c76b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c76b-133">请求</span><span class="sxs-lookup"><span data-stu-id="4c76b-133">Request</span></span>
<span data-ttu-id="4c76b-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4c76b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "dismiss_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/dismiss

Request Body
{
  "userIds": [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
  ]
}
```
##### <a name="response"></a><span data-ttu-id="4c76b-135">响应</span><span class="sxs-lookup"><span data-stu-id="4c76b-135">Response</span></span>
<span data-ttu-id="4c76b-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4c76b-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUsers"
} -->
```http
HTTP/1.1 204 NoContent
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
