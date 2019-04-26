---
title: automaticRepliesSetting 资源类型
description: '配置设置, 以自动将传入电子邮件的发件人通知发件人的邮件 '
localization_priority: Normal
ms.openlocfilehash: 6d7be13a47359e74b4d7a1dc44a4cca38924396e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328217"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="a54ea-103">automaticRepliesSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="a54ea-103">automaticRepliesSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a54ea-p101">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。例如，通知已登录用户无法回复电子邮件的自动答复。</span><span class="sxs-lookup"><span data-stu-id="a54ea-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="a54ea-106">属性</span><span class="sxs-lookup"><span data-stu-id="a54ea-106">Properties</span></span>
| <span data-ttu-id="a54ea-107">属性</span><span class="sxs-lookup"><span data-stu-id="a54ea-107">Property</span></span>     | <span data-ttu-id="a54ea-108">类型</span><span class="sxs-lookup"><span data-stu-id="a54ea-108">Type</span></span>   |<span data-ttu-id="a54ea-109">说明</span><span class="sxs-lookup"><span data-stu-id="a54ea-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a54ea-110">externalAudience</span><span class="sxs-lookup"><span data-stu-id="a54ea-110">externalAudience</span></span>|<span data-ttu-id="a54ea-111">String</span><span class="sxs-lookup"><span data-stu-id="a54ea-111">String</span></span>| <span data-ttu-id="a54ea-p102">如果 **Status** 是 \*\*\*\* 或 `AlwaysEnabled`，则表示将接收 `Scheduled` 的已登录用户组织外部的受众组。可能的值是：`none`、`contactsOnly`、`all`。</span><span class="sxs-lookup"><span data-stu-id="a54ea-p102">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`. Possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="a54ea-114">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="a54ea-114">externalReplyMessage</span></span>|<span data-ttu-id="a54ea-115">string</span><span class="sxs-lookup"><span data-stu-id="a54ea-115">string</span></span>|<span data-ttu-id="a54ea-116">如果 **Status** 是 `AlwaysEnabled` 或 `Scheduled`，则表示发送给指定外部受众的自动答复。</span><span class="sxs-lookup"><span data-stu-id="a54ea-116">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="a54ea-117">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="a54ea-117">internalReplyMessage</span></span>|<span data-ttu-id="a54ea-118">string</span><span class="sxs-lookup"><span data-stu-id="a54ea-118">string</span></span>|<span data-ttu-id="a54ea-119">如果 **Status** 为 `AlwaysEnabled` 或 `Scheduled`，则表示发送给已登录用户组织内部受众的自动答复。</span><span class="sxs-lookup"><span data-stu-id="a54ea-119">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="a54ea-120">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="a54ea-120">scheduledEndDateTime</span></span>|[<span data-ttu-id="a54ea-121">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a54ea-121">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="a54ea-122">如果 **Status** 设置为 `Scheduled`，则自动答复的日期和时间设置为结束。</span><span class="sxs-lookup"><span data-stu-id="a54ea-122">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="a54ea-123">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="a54ea-123">scheduledStartDateTime</span></span>|[<span data-ttu-id="a54ea-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a54ea-124">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="a54ea-125">如果 **Status** 设置为 `Scheduled`，则自动答复的日期和时间设置为开始。</span><span class="sxs-lookup"><span data-stu-id="a54ea-125">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="a54ea-126">status</span><span class="sxs-lookup"><span data-stu-id="a54ea-126">status</span></span>|<span data-ttu-id="a54ea-127">String</span><span class="sxs-lookup"><span data-stu-id="a54ea-127">String</span></span>|<span data-ttu-id="a54ea-p103">自动答复的配置状态。可能的值是：`disabled`、`alwaysEnabled`、`scheduled`。</span><span class="sxs-lookup"><span data-stu-id="a54ea-p103">Configurations status for automatic replies. Possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a54ea-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a54ea-130">JSON representation</span></span>

<span data-ttu-id="a54ea-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a54ea-131">Here is a JSON representation of the resource.</span></span>

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
