---
title: automaticRepliesSetting 资源类型
description: '配置设置，以自动将传入电子邮件的发件人通知发件人的邮件 '
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 46d7738971f2a0f14e44326c51a40245d57e72d7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057071"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="ec2ee-103">automaticRepliesSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="ec2ee-103">automaticRepliesSetting resource type</span></span>

<span data-ttu-id="ec2ee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec2ee-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ec2ee-p101">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。例如，通知已登录用户无法回复电子邮件的自动答复。</span><span class="sxs-lookup"><span data-stu-id="ec2ee-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span>


## <a name="properties"></a><span data-ttu-id="ec2ee-107">属性</span><span class="sxs-lookup"><span data-stu-id="ec2ee-107">Properties</span></span>
| <span data-ttu-id="ec2ee-108">属性</span><span class="sxs-lookup"><span data-stu-id="ec2ee-108">Property</span></span>     | <span data-ttu-id="ec2ee-109">类型</span><span class="sxs-lookup"><span data-stu-id="ec2ee-109">Type</span></span>   |<span data-ttu-id="ec2ee-110">说明</span><span class="sxs-lookup"><span data-stu-id="ec2ee-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec2ee-111">externalAudience</span><span class="sxs-lookup"><span data-stu-id="ec2ee-111">externalAudience</span></span>|<span data-ttu-id="ec2ee-112">externalAudienceScope</span><span class="sxs-lookup"><span data-stu-id="ec2ee-112">externalAudienceScope</span></span>| <span data-ttu-id="ec2ee-113">如果 **Status** 是 \*\*\*\* 或 `AlwaysEnabled`，则表示将接收 `Scheduled` 的已登录用户组织外部的受众组。</span><span class="sxs-lookup"><span data-stu-id="ec2ee-113">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> <span data-ttu-id="ec2ee-114">可能的值包括 `none`、`contactsOnly`、`all`。</span><span class="sxs-lookup"><span data-stu-id="ec2ee-114">The possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="ec2ee-115">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="ec2ee-115">externalReplyMessage</span></span>|<span data-ttu-id="ec2ee-116">string</span><span class="sxs-lookup"><span data-stu-id="ec2ee-116">string</span></span>|<span data-ttu-id="ec2ee-117">如果 **Status** 是 `AlwaysEnabled` 或 `Scheduled`，则表示发送给指定外部受众的自动答复。</span><span class="sxs-lookup"><span data-stu-id="ec2ee-117">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="ec2ee-118">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="ec2ee-118">internalReplyMessage</span></span>|<span data-ttu-id="ec2ee-119">string</span><span class="sxs-lookup"><span data-stu-id="ec2ee-119">string</span></span>|<span data-ttu-id="ec2ee-120">如果 **Status** 为 `AlwaysEnabled` 或 `Scheduled`，则表示发送给已登录用户组织内部受众的自动答复。</span><span class="sxs-lookup"><span data-stu-id="ec2ee-120">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="ec2ee-121">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="ec2ee-121">scheduledEndDateTime</span></span>|[<span data-ttu-id="ec2ee-122">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="ec2ee-122">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="ec2ee-123">如果 **Status** 设置为 `Scheduled`，则自动答复的日期和时间设置为结束。</span><span class="sxs-lookup"><span data-stu-id="ec2ee-123">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="ec2ee-124">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="ec2ee-124">scheduledStartDateTime</span></span>|[<span data-ttu-id="ec2ee-125">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="ec2ee-125">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="ec2ee-126">如果 **Status** 设置为 `Scheduled`，则自动答复的日期和时间设置为开始。</span><span class="sxs-lookup"><span data-stu-id="ec2ee-126">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="ec2ee-127">status</span><span class="sxs-lookup"><span data-stu-id="ec2ee-127">status</span></span>|<span data-ttu-id="ec2ee-128">automaticRepliesStatus</span><span class="sxs-lookup"><span data-stu-id="ec2ee-128">automaticRepliesStatus</span></span>|<span data-ttu-id="ec2ee-129">自动答复的配置状态。</span><span class="sxs-lookup"><span data-stu-id="ec2ee-129">Configurations status for automatic replies.</span></span> <span data-ttu-id="ec2ee-130">可能的值包括 `disabled`、`alwaysEnabled`、`scheduled`。</span><span class="sxs-lookup"><span data-stu-id="ec2ee-130">The possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ec2ee-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ec2ee-131">JSON representation</span></span>

<span data-ttu-id="ec2ee-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec2ee-132">Here is a JSON representation of the resource.</span></span>

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

