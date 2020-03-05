---
title: mailboxSettings 资源类型
description: 已登录用户的主邮箱的设置。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 99097c026ef219e82a34a6c7b043cf70d36c965d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447505"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="4cc34-103">mailboxSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="4cc34-103">mailboxSettings resource type</span></span>

<span data-ttu-id="4cc34-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4cc34-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4cc34-105">[用户](user.md)的主邮箱的设置。</span><span class="sxs-lookup"><span data-stu-id="4cc34-105">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="4cc34-106">您可以通过查询用户的**mailboxSettings**属性来[获取](../api/user-get-mailboxsettings.md)或[更新](../api/user-update-mailboxsettings.md)用户的邮箱设置。</span><span class="sxs-lookup"><span data-stu-id="4cc34-106">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="4cc34-107">属性</span><span class="sxs-lookup"><span data-stu-id="4cc34-107">Properties</span></span>
| <span data-ttu-id="4cc34-108">属性</span><span class="sxs-lookup"><span data-stu-id="4cc34-108">Property</span></span>     | <span data-ttu-id="4cc34-109">类型</span><span class="sxs-lookup"><span data-stu-id="4cc34-109">Type</span></span>   |<span data-ttu-id="4cc34-110">说明</span><span class="sxs-lookup"><span data-stu-id="4cc34-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4cc34-111">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="4cc34-111">archiveFolder</span></span>|<span data-ttu-id="4cc34-112">string</span><span class="sxs-lookup"><span data-stu-id="4cc34-112">string</span></span>|<span data-ttu-id="4cc34-113">用户存档文件夹的文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="4cc34-113">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="4cc34-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="4cc34-114">automaticRepliesSetting</span></span>|[<span data-ttu-id="4cc34-115">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="4cc34-115">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="4cc34-116">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。</span><span class="sxs-lookup"><span data-stu-id="4cc34-116">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="4cc34-117">dateFormat</span><span class="sxs-lookup"><span data-stu-id="4cc34-117">dateFormat</span></span>|<span data-ttu-id="4cc34-118">string</span><span class="sxs-lookup"><span data-stu-id="4cc34-118">string</span></span>|<span data-ttu-id="4cc34-119">用户邮箱的日期格式。</span><span class="sxs-lookup"><span data-stu-id="4cc34-119">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="4cc34-120">语言</span><span class="sxs-lookup"><span data-stu-id="4cc34-120">language</span></span>|[<span data-ttu-id="4cc34-121">localeInfo</span><span class="sxs-lookup"><span data-stu-id="4cc34-121">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="4cc34-122">用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="4cc34-122">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="4cc34-123">timeFormat</span><span class="sxs-lookup"><span data-stu-id="4cc34-123">timeFormat</span></span>|<span data-ttu-id="4cc34-124">string</span><span class="sxs-lookup"><span data-stu-id="4cc34-124">string</span></span>|<span data-ttu-id="4cc34-125">用户邮箱的时间格式。</span><span class="sxs-lookup"><span data-stu-id="4cc34-125">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="4cc34-126">timeZone</span><span class="sxs-lookup"><span data-stu-id="4cc34-126">timeZone</span></span>|<span data-ttu-id="4cc34-127">string</span><span class="sxs-lookup"><span data-stu-id="4cc34-127">string</span></span>|<span data-ttu-id="4cc34-128">用户邮箱的默认时区。</span><span class="sxs-lookup"><span data-stu-id="4cc34-128">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="4cc34-129">workingHours</span><span class="sxs-lookup"><span data-stu-id="4cc34-129">workingHours</span></span>|[<span data-ttu-id="4cc34-130">workingHours</span><span class="sxs-lookup"><span data-stu-id="4cc34-130">workingHours</span></span>](workinghours.md)|<span data-ttu-id="4cc34-131">特定时区用户一周的工作天数和小时数。</span><span class="sxs-lookup"><span data-stu-id="4cc34-131">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4cc34-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4cc34-132">JSON representation</span></span>

<span data-ttu-id="4cc34-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4cc34-133">Here is a JSON representation of the resource.</span></span>

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
