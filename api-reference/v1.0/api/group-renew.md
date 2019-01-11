---
title: 'group: renew'
description: 续订组以更新到期时间。 续订后，组的有效期就会延长策略中定义的天数。
localization_priority: Normal
ms.openlocfilehash: 401a1ff278be792b5e19af415e11a865e3a86bb4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849348"
---
# <a name="group-renew"></a><span data-ttu-id="fa13f-104">group: renew</span><span class="sxs-lookup"><span data-stu-id="fa13f-104">group: renew</span></span>

<span data-ttu-id="fa13f-105">续订组以更新到期时间。</span><span class="sxs-lookup"><span data-stu-id="fa13f-105">Renews a group's expiration.</span></span> <span data-ttu-id="fa13f-106">续订后，组的有效期就会延长策略中定义的天数。</span><span class="sxs-lookup"><span data-stu-id="fa13f-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa13f-107">权限</span><span class="sxs-lookup"><span data-stu-id="fa13f-107">Permissions</span></span>

<span data-ttu-id="fa13f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa13f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="fa13f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa13f-110">Permission type</span></span>      | <span data-ttu-id="fa13f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa13f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa13f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa13f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fa13f-113">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa13f-113">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="fa13f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa13f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa13f-115">不支持</span><span class="sxs-lookup"><span data-stu-id="fa13f-115">Not supported</span></span> |
|<span data-ttu-id="fa13f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa13f-116">Application</span></span> | <span data-ttu-id="fa13f-117">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa13f-117">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa13f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa13f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/renew
```

## <a name="request-headers"></a><span data-ttu-id="fa13f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa13f-119">Request headers</span></span>
| <span data-ttu-id="fa13f-120">名称</span><span class="sxs-lookup"><span data-stu-id="fa13f-120">Name</span></span>       | <span data-ttu-id="fa13f-121">说明</span><span class="sxs-lookup"><span data-stu-id="fa13f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fa13f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa13f-122">Authorization</span></span>  | <span data-ttu-id="fa13f-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="fa13f-123">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="fa13f-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa13f-124">Request body</span></span>

<span data-ttu-id="fa13f-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fa13f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa13f-126">响应</span><span class="sxs-lookup"><span data-stu-id="fa13f-126">Response</span></span>

<span data-ttu-id="fa13f-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fa13f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa13f-129">示例</span><span class="sxs-lookup"><span data-stu-id="fa13f-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fa13f-130">请求</span><span class="sxs-lookup"><span data-stu-id="fa13f-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/renew
```

##### <a name="response"></a><span data-ttu-id="fa13f-131">响应</span><span class="sxs-lookup"><span data-stu-id="fa13f-131">Response</span></span>
<span data-ttu-id="fa13f-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fa13f-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Boolean"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: renew",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
