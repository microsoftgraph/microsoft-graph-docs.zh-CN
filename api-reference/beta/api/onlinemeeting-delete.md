---
title: 删除 onlineMeeting
description: 删除联机会议。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d0b851651a4cf7d0aa1071f46cfccd2a275af55e
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292747"
---
# <a name="delete-onlinemeeting"></a><span data-ttu-id="c5bc5-103">删除 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="c5bc5-103">Delete onlineMeeting</span></span>

<span data-ttu-id="c5bc5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5bc5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5bc5-105">删除 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c5bc5-105">Delete an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5bc5-106">权限</span><span class="sxs-lookup"><span data-stu-id="c5bc5-106">Permissions</span></span>

| <span data-ttu-id="c5bc5-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5bc5-107">Permission type</span></span>                        | <span data-ttu-id="c5bc5-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5bc5-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c5bc5-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5bc5-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="c5bc5-110">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5bc5-110">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="c5bc5-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5bc5-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5bc5-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5bc5-112">Not Supported.</span></span>                              |
| <span data-ttu-id="c5bc5-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5bc5-113">Application</span></span>                            | <span data-ttu-id="c5bc5-114">OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="c5bc5-114">OnlineMeetings.ReadWrite.All\*</span></span>                |

> [!IMPORTANT]
> <span data-ttu-id="c5bc5-115">\*管理员必须创建应用程序访问[](/graph/cloud-communication-online-meeting-application-access-policy)策略，并授予用户，授权策略中配置的应用代表该用户 (用户 ID（在已创建的重新指定路径) 中指定）删除联机会议。</span><span class="sxs-lookup"><span data-stu-id="c5bc5-115">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to delete an online meeting on behalf of that user (user ID specified in the reuqest path) has created.</span></span>

## <a name="http-request"></a><span data-ttu-id="c5bc5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5bc5-116">HTTP request</span></span>

<span data-ttu-id="c5bc5-117">使用委派令牌时的请求</span><span class="sxs-lookup"><span data-stu-id="c5bc5-117">Request when using a delegated token</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/{meetingId}
```

<span data-ttu-id="c5bc5-118">使用应用程序令牌时的请求：</span><span class="sxs-lookup"><span data-stu-id="c5bc5-118">Request when using an application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/users/{userId}/onlineMeetings/{meetingId}
```

> <span data-ttu-id="c5bc5-119">**注意：**</span><span class="sxs-lookup"><span data-stu-id="c5bc5-119">**Note:**</span></span>
>
> - <span data-ttu-id="c5bc5-120">`userId`是 Azure 用户管理门户中[用户的对象 ID。](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span><span class="sxs-lookup"><span data-stu-id="c5bc5-120">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="c5bc5-121">有关详细信息，请参阅 [应用程序访问策略](/graph/cloud-communication-online-meeting-application-access-policy)。</span><span class="sxs-lookup"><span data-stu-id="c5bc5-121">For more details, see [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>
> - <span data-ttu-id="c5bc5-122">`meetingId`是[onlineMeeting 对象的](../resources/onlinemeeting.md)ID。</span><span class="sxs-lookup"><span data-stu-id="c5bc5-122">`meetingId` is the **id** of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5bc5-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5bc5-123">Request headers</span></span>
| <span data-ttu-id="c5bc5-124">名称</span><span class="sxs-lookup"><span data-stu-id="c5bc5-124">Name</span></span>          | <span data-ttu-id="c5bc5-125">说明</span><span class="sxs-lookup"><span data-stu-id="c5bc5-125">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c5bc5-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5bc5-126">Authorization</span></span> | <span data-ttu-id="c5bc5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c5bc5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5bc5-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5bc5-129">Request body</span></span>
<span data-ttu-id="c5bc5-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c5bc5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5bc5-131">响应</span><span class="sxs-lookup"><span data-stu-id="c5bc5-131">Response</span></span>
<span data-ttu-id="c5bc5-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c5bc5-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c5bc5-134">示例</span><span class="sxs-lookup"><span data-stu-id="c5bc5-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c5bc5-135">请求</span><span class="sxs-lookup"><span data-stu-id="c5bc5-135">Request</span></span>
<span data-ttu-id="c5bc5-136">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="c5bc5-136">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c5bc5-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5bc5-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onlineMeetings/550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype
```
# <a name="c"></a>[<span data-ttu-id="c5bc5-138">C#</span><span class="sxs-lookup"><span data-stu-id="c5bc5-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5bc5-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5bc5-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5bc5-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5bc5-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5bc5-141">Java</span><span class="sxs-lookup"><span data-stu-id="c5bc5-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-call-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c5bc5-142">响应</span><span class="sxs-lookup"><span data-stu-id="c5bc5-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


