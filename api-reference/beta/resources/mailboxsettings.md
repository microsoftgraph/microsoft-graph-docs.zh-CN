---
title: mailboxSettings 资源类型
description: 已登录用户的主邮箱的设置。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 6ad2a215270e712e8438e9d2b4b8ce2803477192
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980123"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="9d302-103">mailboxSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d302-103">mailboxSettings resource type</span></span>

> <span data-ttu-id="9d302-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9d302-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d302-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9d302-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9d302-106">已登录用户的主邮箱的设置。</span><span class="sxs-lookup"><span data-stu-id="9d302-106">Settings for the primary mailbox of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="9d302-107">属性</span><span class="sxs-lookup"><span data-stu-id="9d302-107">Properties</span></span>
| <span data-ttu-id="9d302-108">属性</span><span class="sxs-lookup"><span data-stu-id="9d302-108">Property</span></span>     | <span data-ttu-id="9d302-109">类型</span><span class="sxs-lookup"><span data-stu-id="9d302-109">Type</span></span>   |<span data-ttu-id="9d302-110">说明</span><span class="sxs-lookup"><span data-stu-id="9d302-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d302-111">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="9d302-111">archiveFolder</span></span>|<span data-ttu-id="9d302-112">string</span><span class="sxs-lookup"><span data-stu-id="9d302-112">string</span></span>|<span data-ttu-id="9d302-113">用户存档文件夹的文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="9d302-113">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="9d302-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="9d302-114">automaticRepliesSetting</span></span>|[<span data-ttu-id="9d302-115">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="9d302-115">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="9d302-116">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。</span><span class="sxs-lookup"><span data-stu-id="9d302-116">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="9d302-117">语言</span><span class="sxs-lookup"><span data-stu-id="9d302-117">language</span></span>|[<span data-ttu-id="9d302-118">localeInfo</span><span class="sxs-lookup"><span data-stu-id="9d302-118">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="9d302-119">用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="9d302-119">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="9d302-120">timeZone</span><span class="sxs-lookup"><span data-stu-id="9d302-120">timeZone</span></span>|<span data-ttu-id="9d302-121">string</span><span class="sxs-lookup"><span data-stu-id="9d302-121">string</span></span>|<span data-ttu-id="9d302-122">用户邮箱的默认时区。</span><span class="sxs-lookup"><span data-stu-id="9d302-122">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="9d302-123">workingHours</span><span class="sxs-lookup"><span data-stu-id="9d302-123">workingHours</span></span>|[<span data-ttu-id="9d302-124">workingHours</span><span class="sxs-lookup"><span data-stu-id="9d302-124">workingHours</span></span>](workinghours.md)|<span data-ttu-id="9d302-125">特定时区用户一周的工作天数和小时数。</span><span class="sxs-lookup"><span data-stu-id="9d302-125">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d302-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d302-126">JSON representation</span></span>

<span data-ttu-id="9d302-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d302-127">Here is a JSON representation of the resource.</span></span>

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
