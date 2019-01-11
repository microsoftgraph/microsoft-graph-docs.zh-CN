---
title: automaticRepliesSetting 资源类型
description: '配置设置以自动通知中的邮件传入电子邮件的发件人 '
localization_priority: Normal
ms.openlocfilehash: 0160197a4fafe10b7f78be9124da3b6260bfcee6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820655"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="6c831-103">automaticRepliesSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c831-103">automaticRepliesSetting resource type</span></span>

> <span data-ttu-id="6c831-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6c831-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c831-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6c831-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c831-p102">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。例如，通知已登录用户无法回复电子邮件的自动答复。</span><span class="sxs-lookup"><span data-stu-id="6c831-p102">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="6c831-108">属性</span><span class="sxs-lookup"><span data-stu-id="6c831-108">Properties</span></span>
| <span data-ttu-id="6c831-109">属性</span><span class="sxs-lookup"><span data-stu-id="6c831-109">Property</span></span>     | <span data-ttu-id="6c831-110">类型</span><span class="sxs-lookup"><span data-stu-id="6c831-110">Type</span></span>   |<span data-ttu-id="6c831-111">说明</span><span class="sxs-lookup"><span data-stu-id="6c831-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c831-112">externalAudience</span><span class="sxs-lookup"><span data-stu-id="6c831-112">externalAudience</span></span>|<span data-ttu-id="6c831-113">字符串</span><span class="sxs-lookup"><span data-stu-id="6c831-113">String</span></span>| <span data-ttu-id="6c831-p103">如果 **Status** 是 `AlwaysEnabled` 或 `Scheduled`，则表示将接收 **ExternalReplyMessage** 的已登录用户组织外部的受众组。可能的值是：`none`、`contactsOnly`、`all`。</span><span class="sxs-lookup"><span data-stu-id="6c831-p103">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`. Possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="6c831-116">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="6c831-116">externalReplyMessage</span></span>|<span data-ttu-id="6c831-117">string</span><span class="sxs-lookup"><span data-stu-id="6c831-117">string</span></span>|<span data-ttu-id="6c831-118">如果 **Status** 是 `AlwaysEnabled` 或 `Scheduled`，则表示发送给指定外部受众的自动答复。</span><span class="sxs-lookup"><span data-stu-id="6c831-118">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="6c831-119">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="6c831-119">internalReplyMessage</span></span>|<span data-ttu-id="6c831-120">string</span><span class="sxs-lookup"><span data-stu-id="6c831-120">string</span></span>|<span data-ttu-id="6c831-121">如果 **Status** 为 `AlwaysEnabled` 或 `Scheduled`，则表示发送给已登录用户组织内部受众的自动答复。</span><span class="sxs-lookup"><span data-stu-id="6c831-121">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="6c831-122">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="6c831-122">scheduledEndDateTime</span></span>|[<span data-ttu-id="6c831-123">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6c831-123">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6c831-124">如果 **Status** 设置为 `Scheduled`，则自动答复的日期和时间设置为结束。</span><span class="sxs-lookup"><span data-stu-id="6c831-124">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="6c831-125">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="6c831-125">scheduledStartDateTime</span></span>|[<span data-ttu-id="6c831-126">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6c831-126">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6c831-127">如果 **Status** 设置为 `Scheduled`，则自动答复的日期和时间设置为开始。</span><span class="sxs-lookup"><span data-stu-id="6c831-127">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="6c831-128">status</span><span class="sxs-lookup"><span data-stu-id="6c831-128">status</span></span>|<span data-ttu-id="6c831-129">字符串</span><span class="sxs-lookup"><span data-stu-id="6c831-129">String</span></span>|<span data-ttu-id="6c831-p104">自动答复的配置状态。可能的值是：`disabled`、`alwaysEnabled`、`scheduled`。</span><span class="sxs-lookup"><span data-stu-id="6c831-p104">Configurations status for automatic replies. Possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c831-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c831-132">JSON representation</span></span>

<span data-ttu-id="6c831-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c831-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
}-->

```json
{
  "externalAudience": "String",
  "externalReplyMessage": "string",
  "internalReplyMessage": "string",
  "scheduledEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
