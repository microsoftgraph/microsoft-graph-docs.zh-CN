---
title: chatMessagePolicyViolationPolicyTip 资源类型
description: 表示 chatMessagePolicyViolation 对象上的策略提示的属性。 策略提示向发件人提供有关策略冲突的信息。
author: laujan
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1ccc3680f5b0365e1f54e9b82743b6906750b272
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223935"
---
# <a name="chatmessagepolicytip-resource-type"></a><span data-ttu-id="3cb08-104">chatMessagePolicyTip 资源类型</span><span class="sxs-lookup"><span data-stu-id="3cb08-104">chatMessagePolicyTip resource type</span></span>

<span data-ttu-id="3cb08-105">表示 [chatMessagePolicyViolation](chatmessagepolicyviolation.md) 对象上的策略提示的属性。</span><span class="sxs-lookup"><span data-stu-id="3cb08-105">Represents the properties of a policy tip on a [chatMessagePolicyViolation](chatmessagepolicyviolation.md) object.</span></span> <span data-ttu-id="3cb08-106">策略提示向发件人提供有关策略冲突的信息。</span><span class="sxs-lookup"><span data-stu-id="3cb08-106">Policy tips provide the sender with information about the policy violation.</span></span>
<span data-ttu-id="3cb08-107">策略提示通常由数据丢失防护 (DLP) 应用程序设置，该应用程序监视包含用户不应发送的数据的邮件。</span><span class="sxs-lookup"><span data-stu-id="3cb08-107">Policy tips are typically set by a data loss prevention (DLP) app which watches for messages that contain data that users aren't supposed to send.</span></span>

## <a name="properties"></a><span data-ttu-id="3cb08-108">属性</span><span class="sxs-lookup"><span data-stu-id="3cb08-108">Properties</span></span>

| <span data-ttu-id="3cb08-109">属性</span><span class="sxs-lookup"><span data-stu-id="3cb08-109">Property</span></span>   | <span data-ttu-id="3cb08-110">类型</span><span class="sxs-lookup"><span data-stu-id="3cb08-110">Type</span></span> |<span data-ttu-id="3cb08-111">说明</span><span class="sxs-lookup"><span data-stu-id="3cb08-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3cb08-112">complianceUrl</span><span class="sxs-lookup"><span data-stu-id="3cb08-112">complianceUrl</span></span>|<span data-ttu-id="3cb08-113">string</span><span class="sxs-lookup"><span data-stu-id="3cb08-113">string</span></span>|<span data-ttu-id="3cb08-114">用户可访问的 URL，以了解有关组织的数据丢失防护策略的信息。</span><span class="sxs-lookup"><span data-stu-id="3cb08-114">The URL a user can visit to read about the data loss prevention policies for the organization.</span></span> <span data-ttu-id="3cb08-115"> (ie，有关用户在聊天中不应说出的策略) </span><span class="sxs-lookup"><span data-stu-id="3cb08-115">(ie, policies about what users shouldn't say in chats)</span></span>|
|<span data-ttu-id="3cb08-116">generalText</span><span class="sxs-lookup"><span data-stu-id="3cb08-116">generalText</span></span>|<span data-ttu-id="3cb08-117">string</span><span class="sxs-lookup"><span data-stu-id="3cb08-117">string</span></span>|<span data-ttu-id="3cb08-118">向邮件发件人显示的说明性文本。</span><span class="sxs-lookup"><span data-stu-id="3cb08-118">Explanatory text shown to the sender of the message.</span></span>|
|<span data-ttu-id="3cb08-119">matchedConditionDescriptions</span><span class="sxs-lookup"><span data-stu-id="3cb08-119">matchedConditionDescriptions</span></span>|<span data-ttu-id="3cb08-120">string 集合</span><span class="sxs-lookup"><span data-stu-id="3cb08-120">string collection</span></span>|<span data-ttu-id="3cb08-121">数据丢失防护应用程序检测到的消息中的不正确数据的列表。</span><span class="sxs-lookup"><span data-stu-id="3cb08-121">The list of improper data in the message that was detected by the data loss prevention app.</span></span> <span data-ttu-id="3cb08-122">每个 DLP 应用定义其自己的条件，例如 "信用卡号" 和 "社会保险号"。</span><span class="sxs-lookup"><span data-stu-id="3cb08-122">Each DLP app defines its own conditions, examples include "Credit Card Number" and "Social Security Number".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3cb08-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3cb08-123">JSON representation</span></span>

<span data-ttu-id="3cb08-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3cb08-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "generalText"
  ],
  "@odata.type": "microsoft.graph.chatMessagePolicyViolationPolicyTip"
}-->

```json
{
  "complianceUrl": "string",
  "generalText": "string",
  "matchedConditionDescriptions": ["string 1", "string 2"]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "policy violation policy tip resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
