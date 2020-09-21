---
title: 删除参与者
description: 删除呼叫中的特定参与者。
manager: zhengni
author: jackry6350
ms.author: yoren
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 8c08821f723152adb82cde0255d21ea3d8718a8e
ms.sourcegitcommit: d12bd5435c198bcd096e1f7f6a2716f4a04631cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/19/2020
ms.locfileid: "48137154"
---
# <a name="delete-participant"></a><span data-ttu-id="7df36-103">删除参与者</span><span class="sxs-lookup"><span data-stu-id="7df36-103">Delete participant</span></span>

<span data-ttu-id="7df36-104">删除呼叫中的特定参与者。</span><span class="sxs-lookup"><span data-stu-id="7df36-104">Delete a specific participant in a call.</span></span> <span data-ttu-id="7df36-105">在某些情况下，应用程序需要从活动呼叫中删除参与者。</span><span class="sxs-lookup"><span data-stu-id="7df36-105">In some situations, it is appropriate for an application to remove a participant from an active call.</span></span> <span data-ttu-id="7df36-106">此操作可以在参与者应答呼叫之前或之后完成。</span><span class="sxs-lookup"><span data-stu-id="7df36-106">This action can be done either before or after the participant answers the call.</span></span> <span data-ttu-id="7df36-107">删除活动的呼叫者后，它们将立即从呼叫中删除，无签出或删除后通知。</span><span class="sxs-lookup"><span data-stu-id="7df36-107">When an active caller is removed, they are immediately dropped from the call with no pre- or post-removal notification.</span></span>

## <a name="permissions"></a><span data-ttu-id="7df36-108">权限</span><span class="sxs-lookup"><span data-stu-id="7df36-108">Permissions</span></span>
<span data-ttu-id="7df36-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7df36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7df36-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7df36-111">Permission type</span></span>                        | <span data-ttu-id="7df36-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7df36-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7df36-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7df36-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7df36-114">不支持</span><span class="sxs-lookup"><span data-stu-id="7df36-114">Not Supported</span></span>                               |
| <span data-ttu-id="7df36-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7df36-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7df36-116">不支持</span><span class="sxs-lookup"><span data-stu-id="7df36-116">Not Supported</span></span>                               |
| <span data-ttu-id="7df36-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7df36-117">Application</span></span>                            | <span data-ttu-id="7df36-118">无</span><span class="sxs-lookup"><span data-stu-id="7df36-118">None</span></span>                                        |

<span data-ttu-id="7df36-119">租户级应用程序会议配置是允许应用程序调用此 API 所必需的。</span><span class="sxs-lookup"><span data-stu-id="7df36-119">Tenant-level application meeting configuration is required to allow an application to call this API.</span></span> <span data-ttu-id="7df36-120">租户管理员应在租户远程 PowerShell 中调用以下 cmdlet，以向应用程序授予调用此 API 的权限。</span><span class="sxs-lookup"><span data-stu-id="7df36-120">The tenant admin should call the following cmdlet on the tenant remote PowerShell to grant the permission to the application to call this API.</span></span> <span data-ttu-id="7df36-121">有关详细信息，请参阅 [CsApplicationMeetingConfiguration](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/skype/skype-ps/skype/Set-CsApplicationMeetingConfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="7df36-121">For more information, see [Set-CsApplicationMeetingConfiguration](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/skype/skype-ps/skype/Set-CsApplicationMeetingConfiguration.md).</span></span>
```
PS C:\> Set-CsApplicationMeetingConfiguration -AllowRemoveParticipantAppIds @{Add="app_id"}
```

## <a name="http-request"></a><span data-ttu-id="7df36-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7df36-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /communications/calls/{id}/participants/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7df36-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="7df36-123">Request headers</span></span>
| <span data-ttu-id="7df36-124">名称</span><span class="sxs-lookup"><span data-stu-id="7df36-124">Name</span></span>          | <span data-ttu-id="7df36-125">说明</span><span class="sxs-lookup"><span data-stu-id="7df36-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7df36-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7df36-126">Authorization</span></span> | <span data-ttu-id="7df36-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7df36-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7df36-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7df36-129">Request body</span></span>
<span data-ttu-id="7df36-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7df36-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7df36-131">响应</span><span class="sxs-lookup"><span data-stu-id="7df36-131">Response</span></span>
<span data-ttu-id="7df36-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7df36-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7df36-134">示例</span><span class="sxs-lookup"><span data-stu-id="7df36-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7df36-135">请求</span><span class="sxs-lookup"><span data-stu-id="7df36-135">Request</span></span>
<span data-ttu-id="7df36-136">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="7df36-136">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete-participant"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/communications/calls/{id}/participants/{id}
```

##### <a name="response"></a><span data-ttu-id="7df36-137">响应</span><span class="sxs-lookup"><span data-stu-id="7df36-137">Response</span></span>

> <span data-ttu-id="7df36-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7df36-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
