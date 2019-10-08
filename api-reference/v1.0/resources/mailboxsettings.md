---
title: mailboxSettings 资源类型
description: 已登录用户的主邮箱的设置。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 12dc1a5992146c23ac6f2858fd7ee0b3508e455a
ms.sourcegitcommit: f23cc661a0e30d01a6b59cfdae90768c55b80ae2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/08/2019
ms.locfileid: "37418298"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="ac54e-103">mailboxSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="ac54e-103">mailboxSettings resource type</span></span>

<span data-ttu-id="ac54e-104">[用户](user.md)的主邮箱的设置。</span><span class="sxs-lookup"><span data-stu-id="ac54e-104">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="ac54e-105">您可以通过查询用户的**mailboxSettings**属性来[获取](../api/user-get-mailboxsettings.md)或[更新](../api/user-update-mailboxsettings.md)用户的邮箱设置。</span><span class="sxs-lookup"><span data-stu-id="ac54e-105">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="ac54e-106">属性</span><span class="sxs-lookup"><span data-stu-id="ac54e-106">Properties</span></span>
| <span data-ttu-id="ac54e-107">属性</span><span class="sxs-lookup"><span data-stu-id="ac54e-107">Property</span></span>     | <span data-ttu-id="ac54e-108">类型</span><span class="sxs-lookup"><span data-stu-id="ac54e-108">Type</span></span>   |<span data-ttu-id="ac54e-109">说明</span><span class="sxs-lookup"><span data-stu-id="ac54e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac54e-110">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="ac54e-110">archiveFolder</span></span>|<span data-ttu-id="ac54e-111">string</span><span class="sxs-lookup"><span data-stu-id="ac54e-111">string</span></span>|<span data-ttu-id="ac54e-112">用户存档文件夹的文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="ac54e-112">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="ac54e-113">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="ac54e-113">automaticRepliesSetting</span></span>|[<span data-ttu-id="ac54e-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="ac54e-114">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="ac54e-115">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。</span><span class="sxs-lookup"><span data-stu-id="ac54e-115">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="ac54e-116">dateFormat</span><span class="sxs-lookup"><span data-stu-id="ac54e-116">dateFormat</span></span>|<span data-ttu-id="ac54e-117">string</span><span class="sxs-lookup"><span data-stu-id="ac54e-117">string</span></span>|<span data-ttu-id="ac54e-118">用户邮箱的日期格式。</span><span class="sxs-lookup"><span data-stu-id="ac54e-118">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="ac54e-119">语言</span><span class="sxs-lookup"><span data-stu-id="ac54e-119">language</span></span>|[<span data-ttu-id="ac54e-120">localeInfo</span><span class="sxs-lookup"><span data-stu-id="ac54e-120">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="ac54e-121">用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="ac54e-121">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="ac54e-122">timeFormat</span><span class="sxs-lookup"><span data-stu-id="ac54e-122">timeFormat</span></span>|<span data-ttu-id="ac54e-123">string</span><span class="sxs-lookup"><span data-stu-id="ac54e-123">string</span></span>|<span data-ttu-id="ac54e-124">用户邮箱的时间格式。</span><span class="sxs-lookup"><span data-stu-id="ac54e-124">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="ac54e-125">timeZone</span><span class="sxs-lookup"><span data-stu-id="ac54e-125">timeZone</span></span>|<span data-ttu-id="ac54e-126">string</span><span class="sxs-lookup"><span data-stu-id="ac54e-126">string</span></span>|<span data-ttu-id="ac54e-127">用户邮箱的默认时区。</span><span class="sxs-lookup"><span data-stu-id="ac54e-127">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="ac54e-128">workingHours</span><span class="sxs-lookup"><span data-stu-id="ac54e-128">workingHours</span></span>|[<span data-ttu-id="ac54e-129">workingHours</span><span class="sxs-lookup"><span data-stu-id="ac54e-129">workingHours</span></span>](workinghours.md)|<span data-ttu-id="ac54e-130">特定时区用户一周的工作天数和小时数。</span><span class="sxs-lookup"><span data-stu-id="ac54e-130">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ac54e-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ac54e-131">JSON representation</span></span>

<span data-ttu-id="ac54e-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac54e-132">Here is a JSON representation of the resource.</span></span>

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
