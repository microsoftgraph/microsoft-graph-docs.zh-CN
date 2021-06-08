---
title: channel： removeEmail
description: 删除频道的预配电子邮件。
author: anandab-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4608538cf136ba4f53a960183bc0b3f4bd7fc269
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813226"
---
# <a name="channel-removeemail"></a><span data-ttu-id="c558c-103">channel： removeEmail</span><span class="sxs-lookup"><span data-stu-id="c558c-103">channel: removeEmail</span></span>

<span data-ttu-id="c558c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c558c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c558c-105">删除频道的已设置 [电子邮件地址](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="c558c-105">Remove the provisioned email address of a [channel](../resources/channel.md).</span></span>

<span data-ttu-id="c558c-106">只有当电子邮件地址是使用[provisionEmail](channel-provisionemail.md)方法或通过 Microsoft Teams 客户端预配时，才能删除。</span><span class="sxs-lookup"><span data-stu-id="c558c-106">You can remove an email address only if it was provisioned using the [provisionEmail](channel-provisionemail.md) method or through the Microsoft Teams client.</span></span>

## <a name="permissions"></a><span data-ttu-id="c558c-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="c558c-107">Permissions</span></span>

<span data-ttu-id="c558c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c558c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c558c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c558c-110">Permission type</span></span>                        | <span data-ttu-id="c558c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c558c-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c558c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c558c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c558c-113">ChannelSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c558c-113">ChannelSettings.ReadWrite.All</span></span>               |
| <span data-ttu-id="c558c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c558c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c558c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c558c-115">Not supported.</span></span>                              |
| <span data-ttu-id="c558c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c558c-116">Application</span></span>                            | <span data-ttu-id="c558c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c558c-117">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="c558c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c558c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/removeEmail
```
## <a name="request-headers"></a><span data-ttu-id="c558c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c558c-119">Request headers</span></span>
| <span data-ttu-id="c558c-120">标头</span><span class="sxs-lookup"><span data-stu-id="c558c-120">Header</span></span>        | <span data-ttu-id="c558c-121">值</span><span class="sxs-lookup"><span data-stu-id="c558c-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="c558c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c558c-122">Authorization</span></span> | <span data-ttu-id="c558c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c558c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c558c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c558c-125">Request body</span></span>

<span data-ttu-id="c558c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c558c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c558c-127">响应</span><span class="sxs-lookup"><span data-stu-id="c558c-127">Response</span></span>

<span data-ttu-id="c558c-128">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c558c-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c558c-129">示例</span><span class="sxs-lookup"><span data-stu-id="c558c-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="c558c-130">请求</span><span class="sxs-lookup"><span data-stu-id="c558c-130">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["893075dd-2487-4122-925f-022c42e20265", "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2"],
  "name": "channel_removeemail"
}
-->
```http
POST https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2/removeEmail
```

### <a name="response"></a><span data-ttu-id="c558c-131">响应</span><span class="sxs-lookup"><span data-stu-id="c558c-131">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove channel email",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


