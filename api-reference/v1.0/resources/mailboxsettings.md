---
title: mailboxSettings 资源类型
description: 已登录用户的主邮箱的设置。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a9fb455d2a67835ff1a3a10f89ee188a21e9956b
ms.sourcegitcommit: 3e7769ad097e9c34233fa5fea83afa23c34e14a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822779"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="80c0d-103">mailboxSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="80c0d-103">mailboxSettings resource type</span></span>

<span data-ttu-id="80c0d-104">[用户](user.md)的主邮箱的设置。</span><span class="sxs-lookup"><span data-stu-id="80c0d-104">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="80c0d-105">您可以通过查询用户的**mailboxSettings**属性来[获取](../api/user-get-mailboxsettings.md)或[更新](../api/user-update-mailboxsettings.md)用户的邮箱设置。</span><span class="sxs-lookup"><span data-stu-id="80c0d-105">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="80c0d-106">属性</span><span class="sxs-lookup"><span data-stu-id="80c0d-106">Properties</span></span>
| <span data-ttu-id="80c0d-107">属性</span><span class="sxs-lookup"><span data-stu-id="80c0d-107">Property</span></span>     | <span data-ttu-id="80c0d-108">类型</span><span class="sxs-lookup"><span data-stu-id="80c0d-108">Type</span></span>   |<span data-ttu-id="80c0d-109">说明</span><span class="sxs-lookup"><span data-stu-id="80c0d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80c0d-110">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="80c0d-110">archiveFolder</span></span>|<span data-ttu-id="80c0d-111">string</span><span class="sxs-lookup"><span data-stu-id="80c0d-111">string</span></span>|<span data-ttu-id="80c0d-112">用户存档文件夹的文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="80c0d-112">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="80c0d-113">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="80c0d-113">automaticRepliesSetting</span></span>|[<span data-ttu-id="80c0d-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="80c0d-114">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="80c0d-115">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。</span><span class="sxs-lookup"><span data-stu-id="80c0d-115">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="80c0d-116">语言</span><span class="sxs-lookup"><span data-stu-id="80c0d-116">language</span></span>|[<span data-ttu-id="80c0d-117">localeInfo</span><span class="sxs-lookup"><span data-stu-id="80c0d-117">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="80c0d-118">用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="80c0d-118">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="80c0d-119">timeZone</span><span class="sxs-lookup"><span data-stu-id="80c0d-119">timeZone</span></span>|<span data-ttu-id="80c0d-120">string</span><span class="sxs-lookup"><span data-stu-id="80c0d-120">string</span></span>|<span data-ttu-id="80c0d-121">用户邮箱的默认时区。</span><span class="sxs-lookup"><span data-stu-id="80c0d-121">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="80c0d-122">workingHours</span><span class="sxs-lookup"><span data-stu-id="80c0d-122">workingHours</span></span>|[<span data-ttu-id="80c0d-123">workingHours</span><span class="sxs-lookup"><span data-stu-id="80c0d-123">workingHours</span></span>](workinghours.md)|<span data-ttu-id="80c0d-124">特定时区用户一周的工作天数和小时数。</span><span class="sxs-lookup"><span data-stu-id="80c0d-124">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="80c0d-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80c0d-125">JSON representation</span></span>

<span data-ttu-id="80c0d-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80c0d-126">Here is a JSON representation of the resource.</span></span>

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
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
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
