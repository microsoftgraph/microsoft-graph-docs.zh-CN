---
title: mailboxSettings 资源类型
description: 已登录用户的主邮箱的设置。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6d966ecb599d98c92bf1e70eca1f61fb665e359d
ms.sourcegitcommit: 7c017000888a910a0ad85404946f4fc50742c8d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2020
ms.locfileid: "41652042"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="ff380-103">mailboxSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff380-103">mailboxSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff380-104">[用户](user.md)的主邮箱的设置。</span><span class="sxs-lookup"><span data-stu-id="ff380-104">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="ff380-105">您可以通过查询用户的**mailboxSettings**属性来[获取](../api/user-get-mailboxsettings.md)或[更新](../api/user-update-mailboxsettings.md)用户的邮箱设置。</span><span class="sxs-lookup"><span data-stu-id="ff380-105">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="ff380-106">属性</span><span class="sxs-lookup"><span data-stu-id="ff380-106">Properties</span></span>
| <span data-ttu-id="ff380-107">属性</span><span class="sxs-lookup"><span data-stu-id="ff380-107">Property</span></span>     | <span data-ttu-id="ff380-108">类型</span><span class="sxs-lookup"><span data-stu-id="ff380-108">Type</span></span>   |<span data-ttu-id="ff380-109">描述</span><span class="sxs-lookup"><span data-stu-id="ff380-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff380-110">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="ff380-110">archiveFolder</span></span>|<span data-ttu-id="ff380-111">string</span><span class="sxs-lookup"><span data-stu-id="ff380-111">string</span></span>|<span data-ttu-id="ff380-112">用户存档文件夹的文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="ff380-112">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="ff380-113">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="ff380-113">automaticRepliesSetting</span></span>|[<span data-ttu-id="ff380-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="ff380-114">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="ff380-115">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。</span><span class="sxs-lookup"><span data-stu-id="ff380-115">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="ff380-116">dateFormat</span><span class="sxs-lookup"><span data-stu-id="ff380-116">dateFormat</span></span>|<span data-ttu-id="ff380-117">string</span><span class="sxs-lookup"><span data-stu-id="ff380-117">string</span></span>|<span data-ttu-id="ff380-118">用户邮箱的日期格式。</span><span class="sxs-lookup"><span data-stu-id="ff380-118">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="ff380-119">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="ff380-119">delegateMeetingMessageDeliveryOptions</span></span>|<span data-ttu-id="ff380-120">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="ff380-120">delegateMeetingMessageDeliveryOptions</span></span>| <span data-ttu-id="ff380-121">如果用户具有日历代理，则指定代理、邮箱所有者，还是同时接收会议邮件和会议响应。</span><span class="sxs-lookup"><span data-stu-id="ff380-121">If the user has a calendar delegate, this specifies whether the delegate, mailbox owner, or both receive meeting messages and meeting responses.</span></span> <span data-ttu-id="ff380-122">可取值为：`sendToDelegateAndInformationToPrincipal`、`sendToDelegateAndPrincipal`、`sendToDelegateOnly`。</span><span class="sxs-lookup"><span data-stu-id="ff380-122">Possible values are: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span></span> <span data-ttu-id="ff380-123">默认值为`sendToDelegateOnly`。</span><span class="sxs-lookup"><span data-stu-id="ff380-123">The default is `sendToDelegateOnly`.</span></span>|
|<span data-ttu-id="ff380-124">语言</span><span class="sxs-lookup"><span data-stu-id="ff380-124">language</span></span>|[<span data-ttu-id="ff380-125">localeInfo</span><span class="sxs-lookup"><span data-stu-id="ff380-125">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="ff380-126">用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="ff380-126">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="ff380-127">timeFormat</span><span class="sxs-lookup"><span data-stu-id="ff380-127">timeFormat</span></span>|<span data-ttu-id="ff380-128">string</span><span class="sxs-lookup"><span data-stu-id="ff380-128">string</span></span>|<span data-ttu-id="ff380-129">用户邮箱的时间格式。</span><span class="sxs-lookup"><span data-stu-id="ff380-129">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="ff380-130">timeZone</span><span class="sxs-lookup"><span data-stu-id="ff380-130">timeZone</span></span>|<span data-ttu-id="ff380-131">string</span><span class="sxs-lookup"><span data-stu-id="ff380-131">string</span></span>|<span data-ttu-id="ff380-132">用户邮箱的默认时区。</span><span class="sxs-lookup"><span data-stu-id="ff380-132">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="ff380-133">workingHours</span><span class="sxs-lookup"><span data-stu-id="ff380-133">workingHours</span></span>|[<span data-ttu-id="ff380-134">workingHours</span><span class="sxs-lookup"><span data-stu-id="ff380-134">workingHours</span></span>](workinghours.md)|<span data-ttu-id="ff380-135">特定时区用户一周的工作天数和小时数。</span><span class="sxs-lookup"><span data-stu-id="ff380-135">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff380-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff380-136">JSON representation</span></span>

<span data-ttu-id="ff380-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff380-137">Here is a JSON representation of the resource.</span></span>

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
