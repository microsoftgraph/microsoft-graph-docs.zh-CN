---
title: channel： provisionEmail
description: 预配频道的电子邮件。
author: anandab-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 35865ff1b44fad5bc66951df571dbd5252a363df
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813230"
---
# <a name="channel-provisionemail"></a><span data-ttu-id="5c6ce-103">channel： provisionEmail</span><span class="sxs-lookup"><span data-stu-id="5c6ce-103">channel: provisionEmail</span></span>

<span data-ttu-id="5c6ce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c6ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c6ce-105">为频道设置 [电子邮件地址](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="5c6ce-105">Provision an email address for a [channel](../resources/channel.md).</span></span>

<span data-ttu-id="5c6ce-106">Microsoft Teams默认情况下，系统不会自动为频道设置电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="5c6ce-106">Microsoft Teams does not automatically provision an email address for a channel by default.</span></span> <span data-ttu-id="5c6ce-107">若要Teams电子邮件地址，可以调用 **provisionEmail，** 或者通过 Teams 用户界面，选择"获取电子邮件地址"，这将触发 Teams以生成电子邮件地址（如果尚未设置电子邮件地址）。</span><span class="sxs-lookup"><span data-stu-id="5c6ce-107">To have Teams provision an email address, you can call **provisionEmail**, or through the Teams user interface, select **Get email address**, which triggers Teams to generate an email address if it has not already provisioned one.</span></span>

<span data-ttu-id="5c6ce-108">若要删除频道的预配电子邮件地址，请使用 [removeEmail](channel-removeemail.md) 方法。</span><span class="sxs-lookup"><span data-stu-id="5c6ce-108">To remove a channel's provisioned email address, use the [removeEmail](channel-removeemail.md) method.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c6ce-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="5c6ce-109">Permissions</span></span>

<span data-ttu-id="5c6ce-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c6ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5c6ce-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c6ce-112">Permission type</span></span>                        | <span data-ttu-id="5c6ce-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5c6ce-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5c6ce-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c6ce-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="5c6ce-115">ChannelSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c6ce-115">ChannelSettings.ReadWrite.All</span></span>               |
| <span data-ttu-id="5c6ce-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c6ce-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c6ce-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c6ce-117">Not supported.</span></span>                              |
| <span data-ttu-id="5c6ce-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c6ce-118">Application</span></span>                            | <span data-ttu-id="5c6ce-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c6ce-119">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="5c6ce-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c6ce-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/provisionEmail
```
## <a name="request-headers"></a><span data-ttu-id="5c6ce-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c6ce-121">Request headers</span></span>
| <span data-ttu-id="5c6ce-122">标头</span><span class="sxs-lookup"><span data-stu-id="5c6ce-122">Header</span></span>        | <span data-ttu-id="5c6ce-123">值</span><span class="sxs-lookup"><span data-stu-id="5c6ce-123">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="5c6ce-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c6ce-124">Authorization</span></span> | <span data-ttu-id="5c6ce-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5c6ce-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c6ce-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c6ce-127">Request body</span></span>

<span data-ttu-id="5c6ce-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5c6ce-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c6ce-129">响应</span><span class="sxs-lookup"><span data-stu-id="5c6ce-129">Response</span></span>

<span data-ttu-id="5c6ce-130">如果频道的电子邮件设置成功，此方法在响应正文中返回 响应代码和 `200 OK` [provisionChannelEmailResult](../resources/provisionChannelEmailResult.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5c6ce-130">If the channel's email is provisioned successfully, this method returns a `200 OK` response code and a [provisionChannelEmailResult](../resources/provisionChannelEmailResult.md) object in the response body.</span></span> <span data-ttu-id="5c6ce-131">设置的电子邮件地址位于 **email** 属性中。</span><span class="sxs-lookup"><span data-stu-id="5c6ce-131">The provisioned email address is in the **email** property.</span></span>

## <a name="example"></a><span data-ttu-id="5c6ce-132">示例</span><span class="sxs-lookup"><span data-stu-id="5c6ce-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="5c6ce-133">请求</span><span class="sxs-lookup"><span data-stu-id="5c6ce-133">Request</span></span>
<span data-ttu-id="5c6ce-134">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="5c6ce-134">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["893075dd-2487-4122-925f-022c42e20265", "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2"],
  "name": "channel_provisionemail"
}
-->
```http
POST https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2/provisionEmail
```

### <a name="response"></a><span data-ttu-id="5c6ce-135">响应</span><span class="sxs-lookup"><span data-stu-id="5c6ce-135">Response</span></span>
<span data-ttu-id="5c6ce-136">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="5c6ce-136">The following is an example of a response.</span></span>
<span data-ttu-id="5c6ce-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5c6ce-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.provisionChannelEmailResult"
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.provisionChannelEmailResult",
    "email": "1df8f174.teamsgraph.onmicrosoft.com@amer.teams.ms"
}
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Provision channel email",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


