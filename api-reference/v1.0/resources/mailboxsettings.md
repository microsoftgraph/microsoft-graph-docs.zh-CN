---
title: mailboxSettings 资源类型
description: 已登录用户的主邮箱的设置。
localization_priority: Normal
ms.openlocfilehash: d4df71930a26c711c59f164aca5090bda809b503
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826997"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="76bd2-103">mailboxSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="76bd2-103">mailboxSettings resource type</span></span>

<span data-ttu-id="76bd2-104">已登录用户的主邮箱的设置。</span><span class="sxs-lookup"><span data-stu-id="76bd2-104">Settings for the primary mailbox of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="76bd2-105">属性</span><span class="sxs-lookup"><span data-stu-id="76bd2-105">Properties</span></span>
| <span data-ttu-id="76bd2-106">属性</span><span class="sxs-lookup"><span data-stu-id="76bd2-106">Property</span></span>     | <span data-ttu-id="76bd2-107">类型</span><span class="sxs-lookup"><span data-stu-id="76bd2-107">Type</span></span>   |<span data-ttu-id="76bd2-108">说明</span><span class="sxs-lookup"><span data-stu-id="76bd2-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76bd2-109">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="76bd2-109">archiveFolder</span></span>|<span data-ttu-id="76bd2-110">string</span><span class="sxs-lookup"><span data-stu-id="76bd2-110">string</span></span>|<span data-ttu-id="76bd2-111">用户存档文件夹的文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="76bd2-111">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="76bd2-112">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="76bd2-112">automaticRepliesSetting</span></span>|[<span data-ttu-id="76bd2-113">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="76bd2-113">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="76bd2-114">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。</span><span class="sxs-lookup"><span data-stu-id="76bd2-114">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="76bd2-115">语言</span><span class="sxs-lookup"><span data-stu-id="76bd2-115">language</span></span>|[<span data-ttu-id="76bd2-116">localeInfo</span><span class="sxs-lookup"><span data-stu-id="76bd2-116">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="76bd2-117">用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="76bd2-117">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="76bd2-118">timeZone</span><span class="sxs-lookup"><span data-stu-id="76bd2-118">timeZone</span></span>|<span data-ttu-id="76bd2-119">string</span><span class="sxs-lookup"><span data-stu-id="76bd2-119">string</span></span>|<span data-ttu-id="76bd2-120">用户邮箱的默认时区。</span><span class="sxs-lookup"><span data-stu-id="76bd2-120">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="76bd2-121">workingHours</span><span class="sxs-lookup"><span data-stu-id="76bd2-121">workingHours</span></span>|[<span data-ttu-id="76bd2-122">workingHours</span><span class="sxs-lookup"><span data-stu-id="76bd2-122">workingHours</span></span>](workinghours.md)|<span data-ttu-id="76bd2-123">特定时区用户一周的工作天数和小时数。</span><span class="sxs-lookup"><span data-stu-id="76bd2-123">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="76bd2-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76bd2-124">JSON representation</span></span>

<span data-ttu-id="76bd2-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76bd2-125">Here is a JSON representation of the resource.</span></span>

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
