---
title: automaticRepliesSetting 资源类型
description: '配置设置以自动通知中的邮件传入电子邮件的发件人 '
localization_priority: Normal
ms.openlocfilehash: 81fb16a9124c60f43887150917f132579aa4f163
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821404"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="a8dcb-103">automaticRepliesSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="a8dcb-103">automaticRepliesSetting resource type</span></span>

<span data-ttu-id="a8dcb-p101">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。例如，通知已登录用户无法回复电子邮件的自动答复。</span><span class="sxs-lookup"><span data-stu-id="a8dcb-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="a8dcb-106">属性</span><span class="sxs-lookup"><span data-stu-id="a8dcb-106">Properties</span></span>
| <span data-ttu-id="a8dcb-107">属性</span><span class="sxs-lookup"><span data-stu-id="a8dcb-107">Property</span></span>     | <span data-ttu-id="a8dcb-108">类型</span><span class="sxs-lookup"><span data-stu-id="a8dcb-108">Type</span></span>   |<span data-ttu-id="a8dcb-109">说明</span><span class="sxs-lookup"><span data-stu-id="a8dcb-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8dcb-110">externalAudience</span><span class="sxs-lookup"><span data-stu-id="a8dcb-110">externalAudience</span></span>|<span data-ttu-id="a8dcb-111">externalAudienceScope</span><span class="sxs-lookup"><span data-stu-id="a8dcb-111">externalAudienceScope</span></span>| <span data-ttu-id="a8dcb-112">一组的访问群体已登录的用户组织的外部用户将收到**ExternalReplyMessage**，如果**状态**为`AlwaysEnabled`或`Scheduled`。</span><span class="sxs-lookup"><span data-stu-id="a8dcb-112">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> <span data-ttu-id="a8dcb-113">可能的值为： `none`， `contactsOnly`， `all`。</span><span class="sxs-lookup"><span data-stu-id="a8dcb-113">The possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="a8dcb-114">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="a8dcb-114">externalReplyMessage</span></span>|<span data-ttu-id="a8dcb-115">string</span><span class="sxs-lookup"><span data-stu-id="a8dcb-115">string</span></span>|<span data-ttu-id="a8dcb-116">如果 **Status** 是 `AlwaysEnabled` 或 `Scheduled`，则表示发送给指定外部受众的自动答复。</span><span class="sxs-lookup"><span data-stu-id="a8dcb-116">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="a8dcb-117">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="a8dcb-117">internalReplyMessage</span></span>|<span data-ttu-id="a8dcb-118">string</span><span class="sxs-lookup"><span data-stu-id="a8dcb-118">string</span></span>|<span data-ttu-id="a8dcb-119">如果 **Status** 为 `AlwaysEnabled` 或 `Scheduled`，则表示发送给已登录用户组织内部受众的自动答复。</span><span class="sxs-lookup"><span data-stu-id="a8dcb-119">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="a8dcb-120">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="a8dcb-120">scheduledEndDateTime</span></span>|[<span data-ttu-id="a8dcb-121">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a8dcb-121">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="a8dcb-122">如果 **Status** 设置为 `Scheduled`，则自动答复的日期和时间设置为结束。</span><span class="sxs-lookup"><span data-stu-id="a8dcb-122">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="a8dcb-123">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="a8dcb-123">scheduledStartDateTime</span></span>|[<span data-ttu-id="a8dcb-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a8dcb-124">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="a8dcb-125">如果 **Status** 设置为 `Scheduled`，则自动答复的日期和时间设置为开始。</span><span class="sxs-lookup"><span data-stu-id="a8dcb-125">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="a8dcb-126">status</span><span class="sxs-lookup"><span data-stu-id="a8dcb-126">status</span></span>|<span data-ttu-id="a8dcb-127">automaticRepliesStatus</span><span class="sxs-lookup"><span data-stu-id="a8dcb-127">automaticRepliesStatus</span></span>|<span data-ttu-id="a8dcb-128">配置自动答复状态。</span><span class="sxs-lookup"><span data-stu-id="a8dcb-128">Configurations status for automatic replies.</span></span> <span data-ttu-id="a8dcb-129">可能的值为： `disabled`， `alwaysEnabled`， `scheduled`。</span><span class="sxs-lookup"><span data-stu-id="a8dcb-129">The possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a8dcb-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a8dcb-130">JSON representation</span></span>

<span data-ttu-id="a8dcb-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8dcb-131">Here is a JSON representation of the resource.</span></span>

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
