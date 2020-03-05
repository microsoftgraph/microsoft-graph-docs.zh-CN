---
title: messageRuleActions 资源类型
description: 表示适用于规则的一组操作。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 945656aa89fd5786ce4f072fe85ec196d1e6ce48
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522664"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="cbf49-103">messageRuleActions 资源类型</span><span class="sxs-lookup"><span data-stu-id="cbf49-103">messageRuleActions resource type</span></span>

<span data-ttu-id="cbf49-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="cbf49-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbf49-105">表示适用于规则的一组操作。</span><span class="sxs-lookup"><span data-stu-id="cbf49-105">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="cbf49-106">属性</span><span class="sxs-lookup"><span data-stu-id="cbf49-106">Properties</span></span>
| <span data-ttu-id="cbf49-107">属性</span><span class="sxs-lookup"><span data-stu-id="cbf49-107">Property</span></span>     | <span data-ttu-id="cbf49-108">类型</span><span class="sxs-lookup"><span data-stu-id="cbf49-108">Type</span></span>   |<span data-ttu-id="cbf49-109">说明</span><span class="sxs-lookup"><span data-stu-id="cbf49-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cbf49-110">assignCategories</span><span class="sxs-lookup"><span data-stu-id="cbf49-110">assignCategories</span></span> | <span data-ttu-id="cbf49-111">String 集合</span><span class="sxs-lookup"><span data-stu-id="cbf49-111">String collection</span></span> | <span data-ttu-id="cbf49-112">分配给邮件的类别列表。</span><span class="sxs-lookup"><span data-stu-id="cbf49-112">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="cbf49-113">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="cbf49-113">copyToFolder</span></span> | <span data-ttu-id="cbf49-114">String</span><span class="sxs-lookup"><span data-stu-id="cbf49-114">String</span></span> | <span data-ttu-id="cbf49-115">将邮件复制到其中的文件夹的 ID。</span><span class="sxs-lookup"><span data-stu-id="cbf49-115">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="cbf49-116">delete</span><span class="sxs-lookup"><span data-stu-id="cbf49-116">delete</span></span> | <span data-ttu-id="cbf49-117">布尔</span><span class="sxs-lookup"><span data-stu-id="cbf49-117">Boolean</span></span> | <span data-ttu-id="cbf49-118">指示邮件是否应移动到“已删除项目”文件夹。</span><span class="sxs-lookup"><span data-stu-id="cbf49-118">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="cbf49-119">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="cbf49-119">forwardAsAttachmentTo</span></span> | <span data-ttu-id="cbf49-120">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="cbf49-120">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="cbf49-121">应以附件形式接收转发邮件的收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="cbf49-121">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="cbf49-122">forwardTo</span><span class="sxs-lookup"><span data-stu-id="cbf49-122">forwardTo</span></span> | <span data-ttu-id="cbf49-123">[recipient](recipient.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cbf49-123">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="cbf49-124">应接收转发邮件的收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="cbf49-124">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="cbf49-125">markAsRead</span><span class="sxs-lookup"><span data-stu-id="cbf49-125">markAsRead</span></span> | <span data-ttu-id="cbf49-126">布尔</span><span class="sxs-lookup"><span data-stu-id="cbf49-126">Boolean</span></span> | <span data-ttu-id="cbf49-127">指示是否应将邮件标记为已读。</span><span class="sxs-lookup"><span data-stu-id="cbf49-127">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="cbf49-128">markImportance</span><span class="sxs-lookup"><span data-stu-id="cbf49-128">markImportance</span></span> | <span data-ttu-id="cbf49-129">String</span><span class="sxs-lookup"><span data-stu-id="cbf49-129">String</span></span> | <span data-ttu-id="cbf49-130">设置邮件重要性，可以是：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="cbf49-130">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="cbf49-131">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="cbf49-131">moveToFolder</span></span> |  <span data-ttu-id="cbf49-132">String</span><span class="sxs-lookup"><span data-stu-id="cbf49-132">String</span></span>| <span data-ttu-id="cbf49-133">邮件将移至其中的文件夹的 ID。</span><span class="sxs-lookup"><span data-stu-id="cbf49-133">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="cbf49-134">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="cbf49-134">permanentDelete</span></span> | <span data-ttu-id="cbf49-135">布尔</span><span class="sxs-lookup"><span data-stu-id="cbf49-135">Boolean</span></span> | <span data-ttu-id="cbf49-136">指示邮件是否应永久删除且不保存到“已删除项目”文件夹。</span><span class="sxs-lookup"><span data-stu-id="cbf49-136">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="cbf49-137">redirectTo</span><span class="sxs-lookup"><span data-stu-id="cbf49-137">redirectTo</span></span> | [<span data-ttu-id="cbf49-138">recipient</span><span class="sxs-lookup"><span data-stu-id="cbf49-138">recipient</span></span>](recipient.md) | <span data-ttu-id="cbf49-139">邮件应重定向到的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="cbf49-139">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="cbf49-140">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="cbf49-140">stopProcessingRules</span></span> | <span data-ttu-id="cbf49-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbf49-141">Boolean</span></span> | <span data-ttu-id="cbf49-142">指示是否应对后续规则进行评估。</span><span class="sxs-lookup"><span data-stu-id="cbf49-142">Indicates whether subsequent rules should be evaluated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="cbf49-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cbf49-143">JSON representation</span></span>
<span data-ttu-id="cbf49-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cbf49-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRuleActions"
}-->

```json
{
  "assignCategories": ["String"],
  "copyToFolder": "String",
  "delete": "Boolean",
  "forwardAsAttachmentTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "forwardTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "markAsRead": "Boolean",
  "markImportance": "String",
  "moveToFolder": "String",
  "permanentDelete": "Boolean",
  "redirectTo": {"@odata.type": "microsoft.graph.recipient"},
  "stopProcessingRules": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
