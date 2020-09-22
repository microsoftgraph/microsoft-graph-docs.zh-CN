---
title: mailboxSettings 资源类型
description: 已登录用户的主邮箱的设置。
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c3ff60d591257929d2856720ad298231d2afb944
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095020"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="c8cbf-103">mailboxSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="c8cbf-103">mailboxSettings resource type</span></span>

<span data-ttu-id="c8cbf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8cbf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8cbf-105">[用户](user.md)的主邮箱的设置。</span><span class="sxs-lookup"><span data-stu-id="c8cbf-105">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="c8cbf-106">您可以通过查询用户的**mailboxSettings**属性来[获取](../api/user-get-mailboxsettings.md)或[更新](../api/user-update-mailboxsettings.md)用户的邮箱设置。</span><span class="sxs-lookup"><span data-stu-id="c8cbf-106">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="c8cbf-107">属性</span><span class="sxs-lookup"><span data-stu-id="c8cbf-107">Properties</span></span>
| <span data-ttu-id="c8cbf-108">属性</span><span class="sxs-lookup"><span data-stu-id="c8cbf-108">Property</span></span>     | <span data-ttu-id="c8cbf-109">类型</span><span class="sxs-lookup"><span data-stu-id="c8cbf-109">Type</span></span>   |<span data-ttu-id="c8cbf-110">说明</span><span class="sxs-lookup"><span data-stu-id="c8cbf-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8cbf-111">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="c8cbf-111">archiveFolder</span></span>|<span data-ttu-id="c8cbf-112">string</span><span class="sxs-lookup"><span data-stu-id="c8cbf-112">string</span></span>|<span data-ttu-id="c8cbf-113">用户存档文件夹的文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="c8cbf-113">Folder ID of an archive folder for the user.</span></span> <span data-ttu-id="c8cbf-114">只读。</span><span class="sxs-lookup"><span data-stu-id="c8cbf-114">Read only.</span></span>|
|<span data-ttu-id="c8cbf-115">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="c8cbf-115">automaticRepliesSetting</span></span>|[<span data-ttu-id="c8cbf-116">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="c8cbf-116">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="c8cbf-117">自动通知发件人有传入电子邮件（包含一封来自已登录用户的邮件）的配置设置。</span><span class="sxs-lookup"><span data-stu-id="c8cbf-117">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="c8cbf-118">dateFormat</span><span class="sxs-lookup"><span data-stu-id="c8cbf-118">dateFormat</span></span>|<span data-ttu-id="c8cbf-119">string</span><span class="sxs-lookup"><span data-stu-id="c8cbf-119">string</span></span>|<span data-ttu-id="c8cbf-120">用户邮箱的日期格式。</span><span class="sxs-lookup"><span data-stu-id="c8cbf-120">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="c8cbf-121">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="c8cbf-121">delegateMeetingMessageDeliveryOptions</span></span>|<span data-ttu-id="c8cbf-122">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="c8cbf-122">delegateMeetingMessageDeliveryOptions</span></span>| <span data-ttu-id="c8cbf-123">如果用户具有日历代理，则指定代理、邮箱所有者，还是同时接收会议邮件和会议响应。</span><span class="sxs-lookup"><span data-stu-id="c8cbf-123">If the user has a calendar delegate, this specifies whether the delegate, mailbox owner, or both receive meeting messages and meeting responses.</span></span> <span data-ttu-id="c8cbf-124">可取值为：`sendToDelegateAndInformationToPrincipal`、`sendToDelegateAndPrincipal`、`sendToDelegateOnly`。</span><span class="sxs-lookup"><span data-stu-id="c8cbf-124">Possible values are: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span></span> <span data-ttu-id="c8cbf-125">默认值为 `sendToDelegateOnly` 。</span><span class="sxs-lookup"><span data-stu-id="c8cbf-125">The default is `sendToDelegateOnly`.</span></span>|
|<span data-ttu-id="c8cbf-126">语言</span><span class="sxs-lookup"><span data-stu-id="c8cbf-126">language</span></span>|[<span data-ttu-id="c8cbf-127">localeInfo</span><span class="sxs-lookup"><span data-stu-id="c8cbf-127">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="c8cbf-128">用户的区域设置信息，包括首选语言和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="c8cbf-128">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="c8cbf-129">timeFormat</span><span class="sxs-lookup"><span data-stu-id="c8cbf-129">timeFormat</span></span>|<span data-ttu-id="c8cbf-130">string</span><span class="sxs-lookup"><span data-stu-id="c8cbf-130">string</span></span>|<span data-ttu-id="c8cbf-131">用户邮箱的时间格式。</span><span class="sxs-lookup"><span data-stu-id="c8cbf-131">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="c8cbf-132">timeZone</span><span class="sxs-lookup"><span data-stu-id="c8cbf-132">timeZone</span></span>|<span data-ttu-id="c8cbf-133">string</span><span class="sxs-lookup"><span data-stu-id="c8cbf-133">string</span></span>|<span data-ttu-id="c8cbf-134">用户邮箱的默认时区。</span><span class="sxs-lookup"><span data-stu-id="c8cbf-134">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="c8cbf-135">workingHours</span><span class="sxs-lookup"><span data-stu-id="c8cbf-135">workingHours</span></span>|[<span data-ttu-id="c8cbf-136">workingHours</span><span class="sxs-lookup"><span data-stu-id="c8cbf-136">workingHours</span></span>](workinghours.md)|<span data-ttu-id="c8cbf-137">特定时区用户一周的工作天数和小时数。</span><span class="sxs-lookup"><span data-stu-id="c8cbf-137">The days of the week and hours in a specific time zone that the user works.</span></span>|
|<span data-ttu-id="c8cbf-138">userPurpose</span><span class="sxs-lookup"><span data-stu-id="c8cbf-138">userPurpose</span></span>|[<span data-ttu-id="c8cbf-139">userPurpose</span><span class="sxs-lookup"><span data-stu-id="c8cbf-139">userPurpose</span></span>](userpurpose.md)|<span data-ttu-id="c8cbf-140">邮箱的用途。</span><span class="sxs-lookup"><span data-stu-id="c8cbf-140">The purpose of the mailbox.</span></span> <span data-ttu-id="c8cbf-141">用于将单个用户的邮箱与 Exchange Online 中的共享邮箱和设备邮箱区分开来。</span><span class="sxs-lookup"><span data-stu-id="c8cbf-141">Used to differentiate a mailbox for a single user from a shared mailbox and equipment mailbox in Exchange Online.</span></span> <span data-ttu-id="c8cbf-142">只读。</span><span class="sxs-lookup"><span data-stu-id="c8cbf-142">Read only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c8cbf-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c8cbf-143">JSON representation</span></span>

<span data-ttu-id="c8cbf-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8cbf-144">Here is a JSON representation of the resource.</span></span>

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
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"},
  "userPurpose": {"@odata.type": "microsoft.graph.userPurpose"}
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


