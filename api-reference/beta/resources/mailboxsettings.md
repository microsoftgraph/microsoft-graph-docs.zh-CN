---
title: mailboxSettings 资源类型
description: 已登录用户的主邮箱的设置。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0df39f5fb94f648e8d5c5a8b0ff9a10c7a9a7efa
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939283"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="d0c09-103">mailboxSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="d0c09-103">mailboxSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0c09-104">[用户](user.md)的主邮箱的设置。</span><span class="sxs-lookup"><span data-stu-id="d0c09-104">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="d0c09-105">您可以通过查询用户的**mailboxSettings**属性来[获取](../api/user-get-mailboxsettings.md)或[更新](../api/user-update-mailboxsettings.md)用户的邮箱设置。</span><span class="sxs-lookup"><span data-stu-id="d0c09-105">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="d0c09-106">属性</span><span class="sxs-lookup"><span data-stu-id="d0c09-106">Properties</span></span>
| <span data-ttu-id="d0c09-107">属性</span><span class="sxs-lookup"><span data-stu-id="d0c09-107">Property</span></span>     | <span data-ttu-id="d0c09-108">类型</span><span class="sxs-lookup"><span data-stu-id="d0c09-108">Type</span></span>   |<span data-ttu-id="d0c09-109">描述</span><span class="sxs-lookup"><span data-stu-id="d0c09-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0c09-110">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="d0c09-110">archiveFolder</span></span>|<span data-ttu-id="d0c09-111">string</span><span class="sxs-lookup"><span data-stu-id="d0c09-111">string</span></span>|<span data-ttu-id="d0c09-112">用户存档文件夹的文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="d0c09-112">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="d0c09-113">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="d0c09-113">automaticRepliesSetting</span></span>|[<span data-ttu-id="d0c09-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="d0c09-114">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="d0c09-115">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。</span><span class="sxs-lookup"><span data-stu-id="d0c09-115">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="d0c09-116">dateFormat</span><span class="sxs-lookup"><span data-stu-id="d0c09-116">dateFormat</span></span>|<span data-ttu-id="d0c09-117">string</span><span class="sxs-lookup"><span data-stu-id="d0c09-117">string</span></span>|<span data-ttu-id="d0c09-118">用户邮箱的日期格式。</span><span class="sxs-lookup"><span data-stu-id="d0c09-118">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="d0c09-119">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="d0c09-119">delegateMeetingMessageDeliveryOptions</span></span>|<span data-ttu-id="d0c09-120">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="d0c09-120">delegateMeetingMessageDeliveryOptions</span></span>| <span data-ttu-id="d0c09-121">如果用户具有日历代理，则指定代理、邮箱所有者，还是同时接收会议邮件和会议响应。</span><span class="sxs-lookup"><span data-stu-id="d0c09-121">If the user has a calendar delegate, this specifies whether the delegate, mailbox owner, or both receive meeting messages and meeting responses.</span></span> <span data-ttu-id="d0c09-122">可取值为：`sendToDelegateAndInformationToPrincipal`、`sendToDelegateAndPrincipal`、`sendToDelegateOnly`。</span><span class="sxs-lookup"><span data-stu-id="d0c09-122">Possible values are: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span></span>|
|<span data-ttu-id="d0c09-123">语言</span><span class="sxs-lookup"><span data-stu-id="d0c09-123">language</span></span>|[<span data-ttu-id="d0c09-124">localeInfo</span><span class="sxs-lookup"><span data-stu-id="d0c09-124">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="d0c09-125">用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="d0c09-125">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="d0c09-126">timeFormat</span><span class="sxs-lookup"><span data-stu-id="d0c09-126">timeFormat</span></span>|<span data-ttu-id="d0c09-127">string</span><span class="sxs-lookup"><span data-stu-id="d0c09-127">string</span></span>|<span data-ttu-id="d0c09-128">用户邮箱的时间格式。</span><span class="sxs-lookup"><span data-stu-id="d0c09-128">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="d0c09-129">timeZone</span><span class="sxs-lookup"><span data-stu-id="d0c09-129">timeZone</span></span>|<span data-ttu-id="d0c09-130">string</span><span class="sxs-lookup"><span data-stu-id="d0c09-130">string</span></span>|<span data-ttu-id="d0c09-131">用户邮箱的默认时区。</span><span class="sxs-lookup"><span data-stu-id="d0c09-131">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="d0c09-132">workingHours</span><span class="sxs-lookup"><span data-stu-id="d0c09-132">workingHours</span></span>|[<span data-ttu-id="d0c09-133">workingHours</span><span class="sxs-lookup"><span data-stu-id="d0c09-133">workingHours</span></span>](workinghours.md)|<span data-ttu-id="d0c09-134">特定时区用户一周的工作天数和小时数。</span><span class="sxs-lookup"><span data-stu-id="d0c09-134">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0c09-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0c09-135">JSON representation</span></span>

<span data-ttu-id="d0c09-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0c09-136">Here is a JSON representation of the resource.</span></span>

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
