---
title: mailboxSettings 资源类型
description: 已登录用户的主邮箱的设置。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f6dbb44810c9469eb6ddb4dc8fd3299bb2b71e71
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522867"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="a0d80-103">mailboxSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="a0d80-103">mailboxSettings resource type</span></span>

<span data-ttu-id="a0d80-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a0d80-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0d80-105">[用户](user.md)的主邮箱的设置。</span><span class="sxs-lookup"><span data-stu-id="a0d80-105">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="a0d80-106">您可以通过查询用户的**mailboxSettings**属性来[获取](../api/user-get-mailboxsettings.md)或[更新](../api/user-update-mailboxsettings.md)用户的邮箱设置。</span><span class="sxs-lookup"><span data-stu-id="a0d80-106">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="a0d80-107">属性</span><span class="sxs-lookup"><span data-stu-id="a0d80-107">Properties</span></span>
| <span data-ttu-id="a0d80-108">属性</span><span class="sxs-lookup"><span data-stu-id="a0d80-108">Property</span></span>     | <span data-ttu-id="a0d80-109">类型</span><span class="sxs-lookup"><span data-stu-id="a0d80-109">Type</span></span>   |<span data-ttu-id="a0d80-110">说明</span><span class="sxs-lookup"><span data-stu-id="a0d80-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0d80-111">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="a0d80-111">archiveFolder</span></span>|<span data-ttu-id="a0d80-112">string</span><span class="sxs-lookup"><span data-stu-id="a0d80-112">string</span></span>|<span data-ttu-id="a0d80-113">用户存档文件夹的文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="a0d80-113">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="a0d80-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="a0d80-114">automaticRepliesSetting</span></span>|[<span data-ttu-id="a0d80-115">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="a0d80-115">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="a0d80-116">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。</span><span class="sxs-lookup"><span data-stu-id="a0d80-116">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="a0d80-117">dateFormat</span><span class="sxs-lookup"><span data-stu-id="a0d80-117">dateFormat</span></span>|<span data-ttu-id="a0d80-118">string</span><span class="sxs-lookup"><span data-stu-id="a0d80-118">string</span></span>|<span data-ttu-id="a0d80-119">用户邮箱的日期格式。</span><span class="sxs-lookup"><span data-stu-id="a0d80-119">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="a0d80-120">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="a0d80-120">delegateMeetingMessageDeliveryOptions</span></span>|<span data-ttu-id="a0d80-121">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="a0d80-121">delegateMeetingMessageDeliveryOptions</span></span>| <span data-ttu-id="a0d80-122">如果用户具有日历代理，则指定代理、邮箱所有者，还是同时接收会议邮件和会议响应。</span><span class="sxs-lookup"><span data-stu-id="a0d80-122">If the user has a calendar delegate, this specifies whether the delegate, mailbox owner, or both receive meeting messages and meeting responses.</span></span> <span data-ttu-id="a0d80-123">可取值为：`sendToDelegateAndInformationToPrincipal`、`sendToDelegateAndPrincipal`、`sendToDelegateOnly`。</span><span class="sxs-lookup"><span data-stu-id="a0d80-123">Possible values are: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span></span> <span data-ttu-id="a0d80-124">默认值为`sendToDelegateOnly`。</span><span class="sxs-lookup"><span data-stu-id="a0d80-124">The default is `sendToDelegateOnly`.</span></span>|
|<span data-ttu-id="a0d80-125">语言</span><span class="sxs-lookup"><span data-stu-id="a0d80-125">language</span></span>|[<span data-ttu-id="a0d80-126">localeInfo</span><span class="sxs-lookup"><span data-stu-id="a0d80-126">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="a0d80-127">用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="a0d80-127">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="a0d80-128">timeFormat</span><span class="sxs-lookup"><span data-stu-id="a0d80-128">timeFormat</span></span>|<span data-ttu-id="a0d80-129">string</span><span class="sxs-lookup"><span data-stu-id="a0d80-129">string</span></span>|<span data-ttu-id="a0d80-130">用户邮箱的时间格式。</span><span class="sxs-lookup"><span data-stu-id="a0d80-130">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="a0d80-131">timeZone</span><span class="sxs-lookup"><span data-stu-id="a0d80-131">timeZone</span></span>|<span data-ttu-id="a0d80-132">string</span><span class="sxs-lookup"><span data-stu-id="a0d80-132">string</span></span>|<span data-ttu-id="a0d80-133">用户邮箱的默认时区。</span><span class="sxs-lookup"><span data-stu-id="a0d80-133">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="a0d80-134">workingHours</span><span class="sxs-lookup"><span data-stu-id="a0d80-134">workingHours</span></span>|[<span data-ttu-id="a0d80-135">workingHours</span><span class="sxs-lookup"><span data-stu-id="a0d80-135">workingHours</span></span>](workinghours.md)|<span data-ttu-id="a0d80-136">特定时区用户一周的工作天数和小时数。</span><span class="sxs-lookup"><span data-stu-id="a0d80-136">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a0d80-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0d80-137">JSON representation</span></span>

<span data-ttu-id="a0d80-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0d80-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "archiveFolder"
  ],
  "@odata.type": "microsoft.graph.mailboxSettings"
}-->

```json
{
  "archiveFolder": "string",
  "automaticRepliesSetting": {"@odata.type": "microsoft.graph.automaticRepliesSetting"},
  "dateFormat": "string",
  "delegateMeetingMessageDeliveryOptions": "String",
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
  "timeFormat": "string",
  "timeZone": "string",
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
