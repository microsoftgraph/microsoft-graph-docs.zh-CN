---
title: automaticRepliesSetting 资源类型
description: '配置设置以自动通知中的邮件传入电子邮件的发件人 '
localization_priority: Normal
ms.openlocfilehash: 5ff16aa93042e0d66063cb62de7a8dcdf870c892
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529850"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="6f214-103">automaticRepliesSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="6f214-103">automaticRepliesSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f214-p101">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。例如，通知已登录用户无法回复电子邮件的自动答复。</span><span class="sxs-lookup"><span data-stu-id="6f214-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="6f214-106">属性</span><span class="sxs-lookup"><span data-stu-id="6f214-106">Properties</span></span>
| <span data-ttu-id="6f214-107">属性</span><span class="sxs-lookup"><span data-stu-id="6f214-107">Property</span></span>     | <span data-ttu-id="6f214-108">类型</span><span class="sxs-lookup"><span data-stu-id="6f214-108">Type</span></span>   |<span data-ttu-id="6f214-109">说明</span><span class="sxs-lookup"><span data-stu-id="6f214-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f214-110">externalAudience</span><span class="sxs-lookup"><span data-stu-id="6f214-110">externalAudience</span></span>|<span data-ttu-id="6f214-111">String</span><span class="sxs-lookup"><span data-stu-id="6f214-111">String</span></span>| <span data-ttu-id="6f214-p102">如果 **Status** 是 `AlwaysEnabled` 或 `Scheduled`，则表示将接收 **ExternalReplyMessage** 的已登录用户组织外部的受众组。可能的值是：`none`、`contactsOnly`、`all`。</span><span class="sxs-lookup"><span data-stu-id="6f214-p102">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`. Possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="6f214-114">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="6f214-114">externalReplyMessage</span></span>|<span data-ttu-id="6f214-115">string</span><span class="sxs-lookup"><span data-stu-id="6f214-115">string</span></span>|<span data-ttu-id="6f214-116">如果 **Status** 是 `AlwaysEnabled` 或 `Scheduled`，则表示发送给指定外部受众的自动答复。</span><span class="sxs-lookup"><span data-stu-id="6f214-116">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="6f214-117">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="6f214-117">internalReplyMessage</span></span>|<span data-ttu-id="6f214-118">string</span><span class="sxs-lookup"><span data-stu-id="6f214-118">string</span></span>|<span data-ttu-id="6f214-119">如果 **Status** 为 `AlwaysEnabled` 或 `Scheduled`，则表示发送给已登录用户组织内部受众的自动答复。</span><span class="sxs-lookup"><span data-stu-id="6f214-119">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="6f214-120">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="6f214-120">scheduledEndDateTime</span></span>|[<span data-ttu-id="6f214-121">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6f214-121">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6f214-122">如果 Status 设置为 ，则自动答复的日期和时间设置为结束。</span><span class="sxs-lookup"><span data-stu-id="6f214-122">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="6f214-123">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="6f214-123">scheduledStartDateTime</span></span>|[<span data-ttu-id="6f214-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6f214-124">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="6f214-125">如果 Status 设置为 ，则自动答复的日期和时间设置为开始。</span><span class="sxs-lookup"><span data-stu-id="6f214-125">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="6f214-126">status</span><span class="sxs-lookup"><span data-stu-id="6f214-126">status</span></span>|<span data-ttu-id="6f214-127">String</span><span class="sxs-lookup"><span data-stu-id="6f214-127">String</span></span>|<span data-ttu-id="6f214-p103">自动答复的配置状态。可能的值是：`disabled`、`alwaysEnabled`、`scheduled`。</span><span class="sxs-lookup"><span data-stu-id="6f214-p103">Configurations status for automatic replies. Possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f214-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6f214-130">JSON representation</span></span>

<span data-ttu-id="6f214-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f214-131">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/automaticrepliessetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
