---
title: automaticRepliesSetting 资源类型
description: '配置设置，用于自动向发件人发送包含来自 以下发件人的邮件的传入电子邮件： '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 9f191f84697a95c992a8e34896ac5e439c37b973
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958827"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="3b6ea-103">automaticRepliesSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b6ea-103">automaticRepliesSetting resource type</span></span>

<span data-ttu-id="3b6ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b6ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b6ea-p101">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。例如，通知已登录用户无法回复电子邮件的自动答复。</span><span class="sxs-lookup"><span data-stu-id="3b6ea-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span>


## <a name="properties"></a><span data-ttu-id="3b6ea-107">属性</span><span class="sxs-lookup"><span data-stu-id="3b6ea-107">Properties</span></span>
| <span data-ttu-id="3b6ea-108">属性</span><span class="sxs-lookup"><span data-stu-id="3b6ea-108">Property</span></span>     | <span data-ttu-id="3b6ea-109">类型</span><span class="sxs-lookup"><span data-stu-id="3b6ea-109">Type</span></span>   |<span data-ttu-id="3b6ea-110">说明</span><span class="sxs-lookup"><span data-stu-id="3b6ea-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b6ea-111">externalAudience</span><span class="sxs-lookup"><span data-stu-id="3b6ea-111">externalAudience</span></span>|<span data-ttu-id="3b6ea-112">externalAudienceScope</span><span class="sxs-lookup"><span data-stu-id="3b6ea-112">externalAudienceScope</span></span> | <span data-ttu-id="3b6ea-p102">如果 **Status** 是  或 `AlwaysEnabled`，则表示将接收 `Scheduled` 的已登录用户组织外部的受众组。可能的值是：`none`、`contactsOnly`、`all`。</span><span class="sxs-lookup"><span data-stu-id="3b6ea-p102">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`. Possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="3b6ea-115">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="3b6ea-115">externalReplyMessage</span></span>|<span data-ttu-id="3b6ea-116">string</span><span class="sxs-lookup"><span data-stu-id="3b6ea-116">string</span></span>|<span data-ttu-id="3b6ea-117">如果 **Status** 是 `AlwaysEnabled` 或 `Scheduled`，则表示发送给指定外部受众的自动答复。</span><span class="sxs-lookup"><span data-stu-id="3b6ea-117">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="3b6ea-118">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="3b6ea-118">internalReplyMessage</span></span>|<span data-ttu-id="3b6ea-119">string</span><span class="sxs-lookup"><span data-stu-id="3b6ea-119">string</span></span>|<span data-ttu-id="3b6ea-120">如果 **Status** 为 `AlwaysEnabled` 或 `Scheduled`，则表示发送给已登录用户组织内部受众的自动答复。</span><span class="sxs-lookup"><span data-stu-id="3b6ea-120">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="3b6ea-121">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="3b6ea-121">scheduledEndDateTime</span></span>|[<span data-ttu-id="3b6ea-122">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3b6ea-122">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3b6ea-123">如果 **Status** 设置为 `Scheduled`，则自动答复的日期和时间设置为结束。</span><span class="sxs-lookup"><span data-stu-id="3b6ea-123">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="3b6ea-124">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="3b6ea-124">scheduledStartDateTime</span></span>|[<span data-ttu-id="3b6ea-125">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3b6ea-125">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3b6ea-126">如果 **Status** 设置为 `Scheduled`，则自动答复的日期和时间设置为开始。</span><span class="sxs-lookup"><span data-stu-id="3b6ea-126">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="3b6ea-127">status</span><span class="sxs-lookup"><span data-stu-id="3b6ea-127">status</span></span>|<span data-ttu-id="3b6ea-128">automaticRepliesStatus</span><span class="sxs-lookup"><span data-stu-id="3b6ea-128">automaticRepliesStatus</span></span>|<span data-ttu-id="3b6ea-129">自动答复的配置状态。</span><span class="sxs-lookup"><span data-stu-id="3b6ea-129">Configurations status for automatic replies.</span></span> <span data-ttu-id="3b6ea-130">可能的值是：`disabled`、`alwaysEnabled`、`scheduled`。</span><span class="sxs-lookup"><span data-stu-id="3b6ea-130">Possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3b6ea-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b6ea-131">JSON representation</span></span>

<span data-ttu-id="3b6ea-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b6ea-132">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


