---
title: 从通道删除选项卡
description: '删除 （取消锁定） 从指定的通道团队中的一个选项卡。 '
ms.openlocfilehash: b3f35d2cc8280d440b8c834ad9443bd5bbfd6bcc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009820"
---
# <a name="delete-tab-from-channel"></a><span data-ttu-id="2abca-103">从通道删除选项卡</span><span class="sxs-lookup"><span data-stu-id="2abca-103">Delete tab from channel</span></span>



<span data-ttu-id="2abca-104">删除 （取消锁定） 从指定的[频道](../resources/channel.md)[团队](../resources/team.md)中的一个选项卡。</span><span class="sxs-lookup"><span data-stu-id="2abca-104">Removes (unpins) a tab from the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="2abca-105">权限</span><span class="sxs-lookup"><span data-stu-id="2abca-105">Permissions</span></span>
<span data-ttu-id="2abca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2abca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2abca-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2abca-108">Permission type</span></span>      | <span data-ttu-id="2abca-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2abca-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2abca-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2abca-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2abca-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2abca-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2abca-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2abca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2abca-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2abca-113">Not supported.</span></span>    |
|<span data-ttu-id="2abca-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2abca-114">Application</span></span> | <span data-ttu-id="2abca-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2abca-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2abca-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2abca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2abca-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2abca-117">Request headers</span></span>
| <span data-ttu-id="2abca-118">标头</span><span class="sxs-lookup"><span data-stu-id="2abca-118">Header</span></span>       | <span data-ttu-id="2abca-119">值</span><span class="sxs-lookup"><span data-stu-id="2abca-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2abca-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2abca-120">Authorization</span></span>  | <span data-ttu-id="2abca-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2abca-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2abca-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="2abca-123">Request body</span></span>
<span data-ttu-id="2abca-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2abca-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2abca-125">响应</span><span class="sxs-lookup"><span data-stu-id="2abca-125">Response</span></span>

<span data-ttu-id="2abca-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2abca-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2abca-128">示例</span><span class="sxs-lookup"><span data-stu-id="2abca-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2abca-129">请求</span><span class="sxs-lookup"><span data-stu-id="2abca-129">Request</span></span>
<span data-ttu-id="2abca-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2abca-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
```
#### <a name="response"></a><span data-ttu-id="2abca-131">响应</span><span class="sxs-lookup"><span data-stu-id="2abca-131">Response</span></span>
<span data-ttu-id="2abca-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2abca-132">The following is an example of the response.</span></span> <span data-ttu-id="2abca-133">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2abca-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2abca-134">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2abca-134">All of the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete tab from channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
