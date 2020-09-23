---
title: chatMessagePolicyViolation 资源类型
description: 表示聊天消息上的策略冲突。 策略冲突通常由数据丢失防护 (DLP) 应用程序设置。
author: laujan
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4ebe7acbb53793fdaac636e083b56f8acec36630
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223940"
---
# <a name="chatmessagepolicyviolation-resource-type"></a><span data-ttu-id="212d2-104">chatMessagePolicyViolation 资源类型</span><span class="sxs-lookup"><span data-stu-id="212d2-104">chatMessagePolicyViolation resource type</span></span>

<span data-ttu-id="212d2-105">代表聊天消息上的策略违规。</span><span class="sxs-lookup"><span data-stu-id="212d2-105">Represents a policy violation on a chat message.</span></span> <span data-ttu-id="212d2-106">策略冲突通常由数据丢失防护 (DLP) 应用程序设置。</span><span class="sxs-lookup"><span data-stu-id="212d2-106">Policy violations are typically set by a data loss prevention (DLP) application.</span></span> <span data-ttu-id="212d2-107">DLP 应用程序监视包含用户不应发送的数据的邮件的聊天。</span><span class="sxs-lookup"><span data-stu-id="212d2-107">DLP applications monitor chats for messages that contain data that users aren't supposed to send.</span></span>

## <a name="properties"></a><span data-ttu-id="212d2-108">属性</span><span class="sxs-lookup"><span data-stu-id="212d2-108">Properties</span></span>

| <span data-ttu-id="212d2-109">属性</span><span class="sxs-lookup"><span data-stu-id="212d2-109">Property</span></span>   | <span data-ttu-id="212d2-110">类型</span><span class="sxs-lookup"><span data-stu-id="212d2-110">Type</span></span> |<span data-ttu-id="212d2-111">说明</span><span class="sxs-lookup"><span data-stu-id="212d2-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="212d2-112">dlpAction</span><span class="sxs-lookup"><span data-stu-id="212d2-112">dlpAction</span></span>|<span data-ttu-id="212d2-113">**chatMessagePolicyViolationDlpActionType**</span><span class="sxs-lookup"><span data-stu-id="212d2-113">**chatMessagePolicyViolationDlpActionType**</span></span>|<span data-ttu-id="212d2-114">DLP 提供程序对包含敏感内容的邮件执行的操作。</span><span class="sxs-lookup"><span data-stu-id="212d2-114">The action taken by the DLP provider on the message with sensitive content.</span></span> <span data-ttu-id="212d2-115">支持的值为：</span><span class="sxs-lookup"><span data-stu-id="212d2-115">Supported values are:</span></span> <li><span data-ttu-id="212d2-116">无</span><span class="sxs-lookup"><span data-stu-id="212d2-116">None</span></span></li><li><span data-ttu-id="212d2-117">NotifySender--将冲突的发件人通知给发件人，但允许读者阅读邮件。</span><span class="sxs-lookup"><span data-stu-id="212d2-117">NotifySender -- Inform the sender of the violation but allow readers to read the message.</span></span></li><li><span data-ttu-id="212d2-118">BlockAccess--阻止读者阅读邮件。</span><span class="sxs-lookup"><span data-stu-id="212d2-118">BlockAccess -- Block readers from reading the message.</span></span></li><li><span data-ttu-id="212d2-119">BlockAccessExternal--阻止组织外部的用户阅读邮件，同时允许组织内的用户阅读邮件。</span><span class="sxs-lookup"><span data-stu-id="212d2-119">BlockAccessExternal -- Block users outside the organization from reading the message, while allowing users within the organization to read the message.</span></span></li>|
|<span data-ttu-id="212d2-120">justificationText</span><span class="sxs-lookup"><span data-stu-id="212d2-120">justificationText</span></span>|<span data-ttu-id="212d2-121">string</span><span class="sxs-lookup"><span data-stu-id="212d2-121">string</span></span>|<span data-ttu-id="212d2-122">覆盖策略违规时邮件发件人提供的两端对齐文本。</span><span class="sxs-lookup"><span data-stu-id="212d2-122">Justification text provided by the sender of the message when overriding a policy violation.</span></span>|
|<span data-ttu-id="212d2-123">policyTip</span><span class="sxs-lookup"><span data-stu-id="212d2-123">policyTip</span></span>|[<span data-ttu-id="212d2-124">chatMessagePolicyViolationPolicyTip</span><span class="sxs-lookup"><span data-stu-id="212d2-124">chatMessagePolicyViolationPolicyTip</span></span>](chatmessagepolicyviolationpolicytip.md)|<span data-ttu-id="212d2-125">向邮件发件人显示邮件被标记为冲突的原因的信息。</span><span class="sxs-lookup"><span data-stu-id="212d2-125">Information to display to the message sender about why the message was flagged as a violation.</span></span> |
|<span data-ttu-id="212d2-126">userAction</span><span class="sxs-lookup"><span data-stu-id="212d2-126">userAction</span></span>|<span data-ttu-id="212d2-127">**chatMessagePolicyViolationUserActionType**</span><span class="sxs-lookup"><span data-stu-id="212d2-127">**chatMessagePolicyViolationUserActionType**</span></span>|<span data-ttu-id="212d2-128">指示用户对 DLP 提供程序阻止的邮件执行的操作。</span><span class="sxs-lookup"><span data-stu-id="212d2-128">Indicates the action taken by the user on a message blocked by the DLP provider.</span></span> <span data-ttu-id="212d2-129">支持的值为：</span><span class="sxs-lookup"><span data-stu-id="212d2-129">Supported values are:</span></span> <li><span data-ttu-id="212d2-130">无</span><span class="sxs-lookup"><span data-stu-id="212d2-130">None</span></span></li><li><span data-ttu-id="212d2-131">Override</span><span class="sxs-lookup"><span data-stu-id="212d2-131">Override</span></span></li><li><span data-ttu-id="212d2-132">ReportFalsePositive</span><span class="sxs-lookup"><span data-stu-id="212d2-132">ReportFalsePositive</span></span></li><span data-ttu-id="212d2-133">当 DLP 提供程序更新邮件以阻止敏感内容时，userAction 不是必需的。</span><span class="sxs-lookup"><span data-stu-id="212d2-133">When the DLP provider is updating the message for blocking sensitive content, userAction is not required.</span></span>|
|<span data-ttu-id="212d2-134">verdictDetails</span><span class="sxs-lookup"><span data-stu-id="212d2-134">verdictDetails</span></span>|<span data-ttu-id="212d2-135">**chatMessagePolicyViolationVerdictDetailsType**</span><span class="sxs-lookup"><span data-stu-id="212d2-135">**chatMessagePolicyViolationVerdictDetailsType**</span></span>|<span data-ttu-id="212d2-136">指示发件人在响应策略冲突时可能采取的操作。</span><span class="sxs-lookup"><span data-stu-id="212d2-136">Indicates what actions the sender may take in response to the policy violation.</span></span> <span data-ttu-id="212d2-137">支持的值为：</span><span class="sxs-lookup"><span data-stu-id="212d2-137">Supported values are:</span></span> <li><span data-ttu-id="212d2-138">无</span><span class="sxs-lookup"><span data-stu-id="212d2-138">None</span></span></li><li><span data-ttu-id="212d2-139">AllowFalsePositiveOverride--允许发件人将 policyViolation 声明为 DLP 应用及其规则中的错误，并允许读者在 dlpAction 隐藏邮件时再次查看邮件。</span><span class="sxs-lookup"><span data-stu-id="212d2-139">AllowFalsePositiveOverride -- Allows the sender to declare the policyViolation to be an error in the DLP app and its rules, and allow readers to see the message again if the dlpAction had hidden it.</span></span></li><li><span data-ttu-id="212d2-140">AllowOverrideWithoutJustification--允许发件人 overriide DLP 违规，并允许读者在 dlpAction 隐藏邮件时再次查看邮件，而无需提供有关此操作的说明。</span><span class="sxs-lookup"><span data-stu-id="212d2-140">AllowOverrideWithoutJustification -- Allows the sender to overriide the DLP violation and allow readers to see the message again if the dlpAction had hidden it, without needing to provide an explanation for doing so.</span></span> </li><li><span data-ttu-id="212d2-141">AllowOverrideWithJustification--允许发件人 overriide DLP 违规，并允许读者在提供这样做的说明之后再次查看该邮件（如果 dlpAction 已隐藏）。</span><span class="sxs-lookup"><span data-stu-id="212d2-141">AllowOverrideWithJustification -- Allows the sender to overriide the DLP violation and allow readers to see the message again if the dlpAction had hidden it, after providing an explanation for doing so.</span></span></li><span data-ttu-id="212d2-142">AllowOverrideWithoutJustification 和 AllowOverrideWithJustification 是相互排斥的。</span><span class="sxs-lookup"><span data-stu-id="212d2-142">AllowOverrideWithoutJustification and AllowOverrideWithJustification are mutually exclusive.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="212d2-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="212d2-143">JSON representation</span></span>

<span data-ttu-id="212d2-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="212d2-144">The following is a JSON representation of the resource.</span></span>

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
