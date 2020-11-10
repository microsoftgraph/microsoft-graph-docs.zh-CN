---
title: 删除参与者
description: 删除呼叫中的特定参与者。
manager: zhengni
author: jackry6350
ms.author: yoren
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: ece6c6d19ab6513d25d0b176a4563071dafc1cd0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964382"
---
# <a name="delete-participant"></a><span data-ttu-id="4425b-103">删除参与者</span><span class="sxs-lookup"><span data-stu-id="4425b-103">Delete participant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4425b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4425b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4425b-105">删除呼叫中的特定参与者。</span><span class="sxs-lookup"><span data-stu-id="4425b-105">Delete a specific participant in a call.</span></span> <span data-ttu-id="4425b-106">在某些情况下，应用程序需要从活动呼叫中删除参与者。</span><span class="sxs-lookup"><span data-stu-id="4425b-106">In some situations, it is appropriate for an application to remove a participant from an active call.</span></span> <span data-ttu-id="4425b-107">在参与者应答呼叫后，可以完成此操作。</span><span class="sxs-lookup"><span data-stu-id="4425b-107">This action can be done after the participant answers the call.</span></span> <span data-ttu-id="4425b-108">删除活动的呼叫者后，它们将立即从呼叫中删除，无签出或删除后通知。</span><span class="sxs-lookup"><span data-stu-id="4425b-108">When an active caller is removed, they are immediately dropped from the call with no pre- or post-removal notification.</span></span>

## <a name="permissions"></a><span data-ttu-id="4425b-109">权限</span><span class="sxs-lookup"><span data-stu-id="4425b-109">Permissions</span></span>
<span data-ttu-id="4425b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4425b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4425b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="4425b-112">Permission type</span></span>                        | <span data-ttu-id="4425b-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4425b-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4425b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4425b-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="4425b-115">不支持</span><span class="sxs-lookup"><span data-stu-id="4425b-115">Not Supported</span></span>                               |
| <span data-ttu-id="4425b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4425b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4425b-117">不支持</span><span class="sxs-lookup"><span data-stu-id="4425b-117">Not Supported</span></span>                               |
| <span data-ttu-id="4425b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="4425b-118">Application</span></span>                            | <span data-ttu-id="4425b-119">无</span><span class="sxs-lookup"><span data-stu-id="4425b-119">None</span></span>                                        |

<span data-ttu-id="4425b-120">租户级应用程序会议配置是允许应用程序调用此 API 所必需的。</span><span class="sxs-lookup"><span data-stu-id="4425b-120">Tenant-level application meeting configuration is required to allow an application to call this API.</span></span> <span data-ttu-id="4425b-121">租户管理员应在租户远程 PowerShell 中调用以下 cmdlet，以向应用程序授予调用此 API 的权限。</span><span class="sxs-lookup"><span data-stu-id="4425b-121">The tenant admin should call the following cmdlet on the tenant remote PowerShell to grant the permission to the application to call this API.</span></span> <span data-ttu-id="4425b-122">有关详细信息，请参阅 [CsApplicationMeetingConfiguration](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/skype/skype-ps/skype/Set-CsApplicationMeetingConfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="4425b-122">For more information, see [Set-CsApplicationMeetingConfiguration](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/skype/skype-ps/skype/Set-CsApplicationMeetingConfiguration.md).</span></span>
```
PS C:\> Set-CsApplicationMeetingConfiguration -AllowRemoveParticipantAppIds @{Add="app_id"}
```

## <a name="http-request"></a><span data-ttu-id="4425b-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4425b-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}/participants/{id}
DELETE /communications/calls/{id}/participants/{id}
```
> <span data-ttu-id="4425b-124">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="4425b-124">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="4425b-125">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="4425b-125">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4425b-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="4425b-126">Request headers</span></span>
| <span data-ttu-id="4425b-127">名称</span><span class="sxs-lookup"><span data-stu-id="4425b-127">Name</span></span>          | <span data-ttu-id="4425b-128">说明</span><span class="sxs-lookup"><span data-stu-id="4425b-128">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4425b-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="4425b-129">Authorization</span></span> | <span data-ttu-id="4425b-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4425b-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4425b-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="4425b-132">Request body</span></span>
<span data-ttu-id="4425b-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4425b-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4425b-134">响应</span><span class="sxs-lookup"><span data-stu-id="4425b-134">Response</span></span>
<span data-ttu-id="4425b-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4425b-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4425b-137">示例</span><span class="sxs-lookup"><span data-stu-id="4425b-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="4425b-138">请求</span><span class="sxs-lookup"><span data-stu-id="4425b-138">Request</span></span>
<span data-ttu-id="4425b-139">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="4425b-139">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4425b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="4425b-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-participant"
}-->
```http
DELETE https://graph.microsoft.com/beta/communications/calls/{id}/participants/{id}
```
# <a name="c"></a>[<span data-ttu-id="4425b-141">C#</span><span class="sxs-lookup"><span data-stu-id="4425b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-participant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4425b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4425b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-participant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4425b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4425b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-participant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4425b-144">Java</span><span class="sxs-lookup"><span data-stu-id="4425b-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-participant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4425b-145">响应</span><span class="sxs-lookup"><span data-stu-id="4425b-145">Response</span></span>

> <span data-ttu-id="4425b-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4425b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Delete participant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
