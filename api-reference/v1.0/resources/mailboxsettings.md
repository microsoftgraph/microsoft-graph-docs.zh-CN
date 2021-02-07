---
title: mailboxSettings 资源类型
description: 已登录用户的主邮箱的设置。
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8f233906cb17869acabd06cee8f83739e194d7a5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128358"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="3b6eb-103">mailboxSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b6eb-103">mailboxSettings resource type</span></span>

<span data-ttu-id="3b6eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b6eb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3b6eb-105">用户的主邮箱 [的设置](user.md)。</span><span class="sxs-lookup"><span data-stu-id="3b6eb-105">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="3b6eb-106">可以通过 [查询](../api/user-get-mailboxsettings.md)[用户的](../api/user-update-mailboxsettings.md) **mailboxSettings** 属性获取或更新用户的邮箱设置。</span><span class="sxs-lookup"><span data-stu-id="3b6eb-106">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="3b6eb-107">属性</span><span class="sxs-lookup"><span data-stu-id="3b6eb-107">Properties</span></span>
| <span data-ttu-id="3b6eb-108">属性</span><span class="sxs-lookup"><span data-stu-id="3b6eb-108">Property</span></span>     | <span data-ttu-id="3b6eb-109">类型</span><span class="sxs-lookup"><span data-stu-id="3b6eb-109">Type</span></span>   |<span data-ttu-id="3b6eb-110">说明</span><span class="sxs-lookup"><span data-stu-id="3b6eb-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b6eb-111">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="3b6eb-111">archiveFolder</span></span>|<span data-ttu-id="3b6eb-112">string</span><span class="sxs-lookup"><span data-stu-id="3b6eb-112">string</span></span>|<span data-ttu-id="3b6eb-113">用户存档文件夹的文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="3b6eb-113">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="3b6eb-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="3b6eb-114">automaticRepliesSetting</span></span>|[<span data-ttu-id="3b6eb-115">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="3b6eb-115">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="3b6eb-116">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。</span><span class="sxs-lookup"><span data-stu-id="3b6eb-116">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="3b6eb-117">dateFormat</span><span class="sxs-lookup"><span data-stu-id="3b6eb-117">dateFormat</span></span>|<span data-ttu-id="3b6eb-118">string</span><span class="sxs-lookup"><span data-stu-id="3b6eb-118">string</span></span>|<span data-ttu-id="3b6eb-119">用户邮箱的日期格式。</span><span class="sxs-lookup"><span data-stu-id="3b6eb-119">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="3b6eb-120">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="3b6eb-120">delegateMeetingMessageDeliveryOptions</span></span>|<span data-ttu-id="3b6eb-121">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="3b6eb-121">delegateMeetingMessageDeliveryOptions</span></span>| <span data-ttu-id="3b6eb-122">如果用户具有日历代理，则指定代理、邮箱所有者还是同时接收会议邮件和会议响应。</span><span class="sxs-lookup"><span data-stu-id="3b6eb-122">If the user has a calendar delegate, this specifies whether the delegate, mailbox owner, or both receive meeting messages and meeting responses.</span></span> <span data-ttu-id="3b6eb-123">可取值为：`sendToDelegateAndInformationToPrincipal`、`sendToDelegateAndPrincipal`、`sendToDelegateOnly`。</span><span class="sxs-lookup"><span data-stu-id="3b6eb-123">Possible values are: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span></span>|
|<span data-ttu-id="3b6eb-124">语言</span><span class="sxs-lookup"><span data-stu-id="3b6eb-124">language</span></span>|[<span data-ttu-id="3b6eb-125">localeInfo</span><span class="sxs-lookup"><span data-stu-id="3b6eb-125">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="3b6eb-126">用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="3b6eb-126">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="3b6eb-127">timeFormat</span><span class="sxs-lookup"><span data-stu-id="3b6eb-127">timeFormat</span></span>|<span data-ttu-id="3b6eb-128">string</span><span class="sxs-lookup"><span data-stu-id="3b6eb-128">string</span></span>|<span data-ttu-id="3b6eb-129">用户邮箱的时间格式。</span><span class="sxs-lookup"><span data-stu-id="3b6eb-129">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="3b6eb-130">timeZone</span><span class="sxs-lookup"><span data-stu-id="3b6eb-130">timeZone</span></span>|<span data-ttu-id="3b6eb-131">string</span><span class="sxs-lookup"><span data-stu-id="3b6eb-131">string</span></span>|<span data-ttu-id="3b6eb-132">用户邮箱的默认时区。</span><span class="sxs-lookup"><span data-stu-id="3b6eb-132">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="3b6eb-133">workingHours</span><span class="sxs-lookup"><span data-stu-id="3b6eb-133">workingHours</span></span>|[<span data-ttu-id="3b6eb-134">workingHours</span><span class="sxs-lookup"><span data-stu-id="3b6eb-134">workingHours</span></span>](workinghours.md)|<span data-ttu-id="3b6eb-135">特定时区用户一周的工作天数和小时数。</span><span class="sxs-lookup"><span data-stu-id="3b6eb-135">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3b6eb-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b6eb-136">JSON representation</span></span>

<span data-ttu-id="3b6eb-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b6eb-137">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

