---
title: messageRuleActions 资源类型
description: 表示适用于规则的一组操作。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: bc74f435533a679263d144478334738f73c79f34
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036125"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="99c8f-103">messageRuleActions 资源类型</span><span class="sxs-lookup"><span data-stu-id="99c8f-103">messageRuleActions resource type</span></span>


<span data-ttu-id="99c8f-104">表示适用于规则的一组操作。</span><span class="sxs-lookup"><span data-stu-id="99c8f-104">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="99c8f-105">属性</span><span class="sxs-lookup"><span data-stu-id="99c8f-105">Properties</span></span>
| <span data-ttu-id="99c8f-106">属性</span><span class="sxs-lookup"><span data-stu-id="99c8f-106">Property</span></span>     | <span data-ttu-id="99c8f-107">类型</span><span class="sxs-lookup"><span data-stu-id="99c8f-107">Type</span></span>   |<span data-ttu-id="99c8f-108">说明</span><span class="sxs-lookup"><span data-stu-id="99c8f-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="99c8f-109">assignCategories</span><span class="sxs-lookup"><span data-stu-id="99c8f-109">assignCategories</span></span> | <span data-ttu-id="99c8f-110">String 集合</span><span class="sxs-lookup"><span data-stu-id="99c8f-110">String collection</span></span> | <span data-ttu-id="99c8f-111">分配给邮件的类别列表。</span><span class="sxs-lookup"><span data-stu-id="99c8f-111">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="99c8f-112">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="99c8f-112">copyToFolder</span></span> | <span data-ttu-id="99c8f-113">String</span><span class="sxs-lookup"><span data-stu-id="99c8f-113">String</span></span> | <span data-ttu-id="99c8f-114">将邮件复制到其中的文件夹的 ID。</span><span class="sxs-lookup"><span data-stu-id="99c8f-114">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="99c8f-115">delete</span><span class="sxs-lookup"><span data-stu-id="99c8f-115">delete</span></span> | <span data-ttu-id="99c8f-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="99c8f-116">Boolean</span></span> | <span data-ttu-id="99c8f-117">指示邮件是否应移动到“已删除项目”文件夹。</span><span class="sxs-lookup"><span data-stu-id="99c8f-117">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="99c8f-118">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="99c8f-118">forwardAsAttachmentTo</span></span> | <span data-ttu-id="99c8f-119">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="99c8f-119">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="99c8f-120">应以附件形式接收转发邮件的收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="99c8f-120">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="99c8f-121">forwardTo</span><span class="sxs-lookup"><span data-stu-id="99c8f-121">forwardTo</span></span> | <span data-ttu-id="99c8f-122">[recipient](recipient.md) 集合</span><span class="sxs-lookup"><span data-stu-id="99c8f-122">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="99c8f-123">应接收转发邮件的收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="99c8f-123">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="99c8f-124">markAsRead</span><span class="sxs-lookup"><span data-stu-id="99c8f-124">markAsRead</span></span> | <span data-ttu-id="99c8f-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="99c8f-125">Boolean</span></span> | <span data-ttu-id="99c8f-126">指示是否应将邮件标记为已读。</span><span class="sxs-lookup"><span data-stu-id="99c8f-126">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="99c8f-127">markImportance</span><span class="sxs-lookup"><span data-stu-id="99c8f-127">markImportance</span></span> | <span data-ttu-id="99c8f-128">importance</span><span class="sxs-lookup"><span data-stu-id="99c8f-128">importance</span></span> | <span data-ttu-id="99c8f-129">设置邮件重要性，可以是：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="99c8f-129">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="99c8f-130">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="99c8f-130">moveToFolder</span></span> |  <span data-ttu-id="99c8f-131">String</span><span class="sxs-lookup"><span data-stu-id="99c8f-131">String</span></span>| <span data-ttu-id="99c8f-132">邮件将移至其中的文件夹的 ID。</span><span class="sxs-lookup"><span data-stu-id="99c8f-132">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="99c8f-133">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="99c8f-133">permanentDelete</span></span> | <span data-ttu-id="99c8f-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="99c8f-134">Boolean</span></span> | <span data-ttu-id="99c8f-135">指示邮件是否应永久删除且不保存到“已删除项目”文件夹。</span><span class="sxs-lookup"><span data-stu-id="99c8f-135">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="99c8f-136">redirectTo</span><span class="sxs-lookup"><span data-stu-id="99c8f-136">redirectTo</span></span> | <span data-ttu-id="99c8f-137">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="99c8f-137">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="99c8f-138">应将邮件重定向到的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="99c8f-138">The email addresses to which a message should be redirected.</span></span> |
| <span data-ttu-id="99c8f-139">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="99c8f-139">stopProcessingRules</span></span> | <span data-ttu-id="99c8f-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="99c8f-140">Boolean</span></span> | <span data-ttu-id="99c8f-141">指示是否应对后续规则进行评估。</span><span class="sxs-lookup"><span data-stu-id="99c8f-141">Indicates whether subsequent rules should be evaluated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="99c8f-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99c8f-142">JSON representation</span></span>
<span data-ttu-id="99c8f-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99c8f-143">Here is a JSON representation of the resource.</span></span>

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
  "redirectTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "stopProcessingRules": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
