---
title: chatMessagePolicyViolation 资源类型
description: 表示聊天消息上的策略违反。 策略违反通常由 DLP 应用程序或 DLP (数据丢失) 设置。
author: RamjotSingh
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9c65b6dd1d07db43286a8cf9923f4a94f0855b34
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582268"
---
# <a name="chatmessagepolicyviolation-resource-type"></a><span data-ttu-id="dc89f-104">chatMessagePolicyViolation 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc89f-104">chatMessagePolicyViolation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc89f-105">表示聊天消息上的策略违反。</span><span class="sxs-lookup"><span data-stu-id="dc89f-105">Represents a policy violation on a chat message.</span></span> <span data-ttu-id="dc89f-106">策略违反通常由 DLP 应用程序或 DLP (数据丢失) 设置。</span><span class="sxs-lookup"><span data-stu-id="dc89f-106">Policy violations are typically set by a data loss prevention (DLP) application.</span></span> <span data-ttu-id="dc89f-107">DLP 应用程序监视包含用户不应该发送的数据的消息的聊天。</span><span class="sxs-lookup"><span data-stu-id="dc89f-107">DLP applications monitor chats for messages that contain data that users aren't supposed to send.</span></span>

## <a name="properties"></a><span data-ttu-id="dc89f-108">属性</span><span class="sxs-lookup"><span data-stu-id="dc89f-108">Properties</span></span>

| <span data-ttu-id="dc89f-109">属性</span><span class="sxs-lookup"><span data-stu-id="dc89f-109">Property</span></span>   | <span data-ttu-id="dc89f-110">类型</span><span class="sxs-lookup"><span data-stu-id="dc89f-110">Type</span></span> |<span data-ttu-id="dc89f-111">说明</span><span class="sxs-lookup"><span data-stu-id="dc89f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc89f-112">dlpAction</span><span class="sxs-lookup"><span data-stu-id="dc89f-112">dlpAction</span></span>|<span data-ttu-id="dc89f-113">**chatMessagePolicyViolationDlpActionType**</span><span class="sxs-lookup"><span data-stu-id="dc89f-113">**chatMessagePolicyViolationDlpActionType**</span></span>|<span data-ttu-id="dc89f-114">DLP 提供程序对包含敏感内容的邮件采取的操作。</span><span class="sxs-lookup"><span data-stu-id="dc89f-114">The action taken by the DLP provider on the message with sensitive content.</span></span> <span data-ttu-id="dc89f-115">支持的值为：</span><span class="sxs-lookup"><span data-stu-id="dc89f-115">Supported values are:</span></span> <li><span data-ttu-id="dc89f-116">无</span><span class="sxs-lookup"><span data-stu-id="dc89f-116">None</span></span></li><li><span data-ttu-id="dc89f-117">NotifySender -- 通知发件人违反，但允许读者阅读邮件。</span><span class="sxs-lookup"><span data-stu-id="dc89f-117">NotifySender -- Inform the sender of the violation but allow readers to read the message.</span></span></li><li><span data-ttu-id="dc89f-118">BlockAccess -- 阻止读者阅读邮件。</span><span class="sxs-lookup"><span data-stu-id="dc89f-118">BlockAccess -- Block readers from reading the message.</span></span></li><li><span data-ttu-id="dc89f-119">BlockAccessExternal -- 阻止组织外部的用户阅读邮件，同时允许组织内部的用户阅读邮件。</span><span class="sxs-lookup"><span data-stu-id="dc89f-119">BlockAccessExternal -- Block users outside the organization from reading the message, while allowing users within the organization to read the message.</span></span></li>|
|<span data-ttu-id="dc89f-120">justificationText</span><span class="sxs-lookup"><span data-stu-id="dc89f-120">justificationText</span></span>|<span data-ttu-id="dc89f-121">string</span><span class="sxs-lookup"><span data-stu-id="dc89f-121">string</span></span>|<span data-ttu-id="dc89f-122">替代策略违反时邮件发件人提供的理由文本。</span><span class="sxs-lookup"><span data-stu-id="dc89f-122">Justification text provided by the sender of the message when overriding a policy violation.</span></span>|
|<span data-ttu-id="dc89f-123">policyTip</span><span class="sxs-lookup"><span data-stu-id="dc89f-123">policyTip</span></span>|[<span data-ttu-id="dc89f-124">chatMessagePolicyViolationPolicyTip</span><span class="sxs-lookup"><span data-stu-id="dc89f-124">chatMessagePolicyViolationPolicyTip</span></span>](chatmessagepolicyviolationpolicytip.md)|<span data-ttu-id="dc89f-125">要向邮件发件人显示有关邮件被标记为违反的原因的信息。</span><span class="sxs-lookup"><span data-stu-id="dc89f-125">Information to display to the message sender about why the message was flagged as a violation.</span></span> |
|<span data-ttu-id="dc89f-126">userAction</span><span class="sxs-lookup"><span data-stu-id="dc89f-126">userAction</span></span>|<span data-ttu-id="dc89f-127">**chatMessagePolicyViolationUserActionType**</span><span class="sxs-lookup"><span data-stu-id="dc89f-127">**chatMessagePolicyViolationUserActionType**</span></span>|<span data-ttu-id="dc89f-128">指示用户对 DLP 提供程序阻止的邮件采取的操作。</span><span class="sxs-lookup"><span data-stu-id="dc89f-128">Indicates the action taken by the user on a message blocked by the DLP provider.</span></span> <span data-ttu-id="dc89f-129">支持的值为：</span><span class="sxs-lookup"><span data-stu-id="dc89f-129">Supported values are:</span></span> <li><span data-ttu-id="dc89f-130">无</span><span class="sxs-lookup"><span data-stu-id="dc89f-130">None</span></span></li><li><span data-ttu-id="dc89f-131">Override</span><span class="sxs-lookup"><span data-stu-id="dc89f-131">Override</span></span></li><li><span data-ttu-id="dc89f-132">ReportFalsePositive</span><span class="sxs-lookup"><span data-stu-id="dc89f-132">ReportFalsePositive</span></span></li><span data-ttu-id="dc89f-133">当 DLP 提供程序更新邮件以阻止敏感内容时，不需要 userAction。</span><span class="sxs-lookup"><span data-stu-id="dc89f-133">When the DLP provider is updating the message for blocking sensitive content, userAction is not required.</span></span>|
|<span data-ttu-id="dc89f-134">verdictDetails</span><span class="sxs-lookup"><span data-stu-id="dc89f-134">verdictDetails</span></span>|<span data-ttu-id="dc89f-135">**chatMessagePolicyViolationVerdictDetailsType**</span><span class="sxs-lookup"><span data-stu-id="dc89f-135">**chatMessagePolicyViolationVerdictDetailsType**</span></span>|<span data-ttu-id="dc89f-136">指示发件人为响应策略违反可能采取的操作。</span><span class="sxs-lookup"><span data-stu-id="dc89f-136">Indicates what actions the sender may take in response to the policy violation.</span></span> <span data-ttu-id="dc89f-137">支持的值为：</span><span class="sxs-lookup"><span data-stu-id="dc89f-137">Supported values are:</span></span> <li><span data-ttu-id="dc89f-138">无</span><span class="sxs-lookup"><span data-stu-id="dc89f-138">None</span></span></li><li><span data-ttu-id="dc89f-139">AllowFalsePositiveOverride -- 允许发件人在 DLP 应用及其规则中声明策略Violation 为错误，并允许读者在 dlpAction 隐藏邮件时再次查看邮件。</span><span class="sxs-lookup"><span data-stu-id="dc89f-139">AllowFalsePositiveOverride -- Allows the sender to declare the policyViolation to be an error in the DLP app and its rules, and allow readers to see the message again if the dlpAction had hidden it.</span></span></li><li><span data-ttu-id="dc89f-140">AllowOverrideWithoutJustification -- 允许发件人过度处理 DLP 冲突，并允许读者在 dlpAction 隐藏邮件时再次查看邮件，而无需提供这样做的说明。</span><span class="sxs-lookup"><span data-stu-id="dc89f-140">AllowOverrideWithoutJustification -- Allows the sender to overriide the DLP violation and allow readers to see the message again if the dlpAction had hidden it, without needing to provide an explanation for doing so.</span></span> </li><li><span data-ttu-id="dc89f-141">AllowOverrideWithJustification -- 允许发件人过度处理 DLP 冲突，并允许读者在 dlpAction 隐藏邮件后再次查看邮件，并提供这样做的说明。</span><span class="sxs-lookup"><span data-stu-id="dc89f-141">AllowOverrideWithJustification -- Allows the sender to overriide the DLP violation and allow readers to see the message again if the dlpAction had hidden it, after providing an explanation for doing so.</span></span></li><span data-ttu-id="dc89f-142">AllowOverrideWithoutJustification 和 AllowOverrideWithJustification 是互斥的。</span><span class="sxs-lookup"><span data-stu-id="dc89f-142">AllowOverrideWithoutJustification and AllowOverrideWithJustification are mutually exclusive.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="dc89f-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc89f-143">JSON representation</span></span>

<span data-ttu-id="dc89f-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc89f-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userAction",
    "justificationText"
  ],
  "@odata.type": "microsoft.graph.chatMessagePolicyViolation"
}-->

```json
{
  "dlpAction": "string",
  "justificationText": "string",
  "policyTip": {"@odata.type": "microsoft.graph.chatMessagePolicyViolationPolicyTip"},
  "userAction": "string",
  "verdictDetails": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat message policy violation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
