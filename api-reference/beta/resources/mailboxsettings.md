---
title: mailboxSettings 资源类型
description: 已登录用户的主邮箱的设置。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: bf5ca7b6e9a653946f5ea1ff0a302c8499f2e02d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345122"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="83243-103">mailboxSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="83243-103">mailboxSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83243-104">已登录用户的主邮箱的设置。</span><span class="sxs-lookup"><span data-stu-id="83243-104">Settings for the primary mailbox of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="83243-105">属性</span><span class="sxs-lookup"><span data-stu-id="83243-105">Properties</span></span>
| <span data-ttu-id="83243-106">属性</span><span class="sxs-lookup"><span data-stu-id="83243-106">Property</span></span>     | <span data-ttu-id="83243-107">类型</span><span class="sxs-lookup"><span data-stu-id="83243-107">Type</span></span>   |<span data-ttu-id="83243-108">说明</span><span class="sxs-lookup"><span data-stu-id="83243-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83243-109">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="83243-109">archiveFolder</span></span>|<span data-ttu-id="83243-110">string</span><span class="sxs-lookup"><span data-stu-id="83243-110">string</span></span>|<span data-ttu-id="83243-111">用户存档文件夹的文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="83243-111">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="83243-112">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="83243-112">automaticRepliesSetting</span></span>|[<span data-ttu-id="83243-113">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="83243-113">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="83243-114">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。</span><span class="sxs-lookup"><span data-stu-id="83243-114">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="83243-115">语言</span><span class="sxs-lookup"><span data-stu-id="83243-115">language</span></span>|[<span data-ttu-id="83243-116">localeInfo</span><span class="sxs-lookup"><span data-stu-id="83243-116">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="83243-117">用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="83243-117">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="83243-118">timeZone</span><span class="sxs-lookup"><span data-stu-id="83243-118">timeZone</span></span>|<span data-ttu-id="83243-119">string</span><span class="sxs-lookup"><span data-stu-id="83243-119">string</span></span>|<span data-ttu-id="83243-120">用户邮箱的默认时区。</span><span class="sxs-lookup"><span data-stu-id="83243-120">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="83243-121">workingHours</span><span class="sxs-lookup"><span data-stu-id="83243-121">workingHours</span></span>|[<span data-ttu-id="83243-122">workingHours</span><span class="sxs-lookup"><span data-stu-id="83243-122">workingHours</span></span>](workinghours.md)|<span data-ttu-id="83243-123">特定时区用户一周的工作天数和小时数。</span><span class="sxs-lookup"><span data-stu-id="83243-123">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83243-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83243-124">JSON representation</span></span>

<span data-ttu-id="83243-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83243-125">Here is a JSON representation of the resource.</span></span>

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
