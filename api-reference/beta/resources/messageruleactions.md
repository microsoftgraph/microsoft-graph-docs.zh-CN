---
title: messageRuleActions 资源类型
description: 表示适用于规则的一组操作。
author: angelgolfer-ms
ms.openlocfilehash: 515d31ff8c11b95a3aa0042449d22df883e0eecf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314992"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="764da-103">messageRuleActions 资源类型</span><span class="sxs-lookup"><span data-stu-id="764da-103">messageRuleActions resource type</span></span>

> <span data-ttu-id="764da-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="764da-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="764da-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="764da-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="764da-106">表示适用于规则的一组操作。</span><span class="sxs-lookup"><span data-stu-id="764da-106">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="764da-107">属性</span><span class="sxs-lookup"><span data-stu-id="764da-107">Properties</span></span>
| <span data-ttu-id="764da-108">属性</span><span class="sxs-lookup"><span data-stu-id="764da-108">Property</span></span>     | <span data-ttu-id="764da-109">类型</span><span class="sxs-lookup"><span data-stu-id="764da-109">Type</span></span>   |<span data-ttu-id="764da-110">说明</span><span class="sxs-lookup"><span data-stu-id="764da-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="764da-111">assignCategories</span><span class="sxs-lookup"><span data-stu-id="764da-111">assignCategories</span></span> | <span data-ttu-id="764da-112">String 集合</span><span class="sxs-lookup"><span data-stu-id="764da-112">String collection</span></span> | <span data-ttu-id="764da-113">分配给邮件的类别列表。</span><span class="sxs-lookup"><span data-stu-id="764da-113">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="764da-114">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="764da-114">copyToFolder</span></span> | <span data-ttu-id="764da-115">String</span><span class="sxs-lookup"><span data-stu-id="764da-115">String</span></span> | <span data-ttu-id="764da-116">将邮件复制到其中的文件夹的 ID。</span><span class="sxs-lookup"><span data-stu-id="764da-116">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="764da-117">delete</span><span class="sxs-lookup"><span data-stu-id="764da-117">delete</span></span> | <span data-ttu-id="764da-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="764da-118">Boolean</span></span> | <span data-ttu-id="764da-119">指示邮件是否应移动到“已删除项目”文件夹。</span><span class="sxs-lookup"><span data-stu-id="764da-119">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="764da-120">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="764da-120">forwardAsAttachmentTo</span></span> | <span data-ttu-id="764da-121">[recipient](recipient.md) 集合</span><span class="sxs-lookup"><span data-stu-id="764da-121">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="764da-122">应以附件形式接收转发邮件的收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="764da-122">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="764da-123">forwardTo</span><span class="sxs-lookup"><span data-stu-id="764da-123">forwardTo</span></span> | <span data-ttu-id="764da-124">[recipient](recipient.md) 集合</span><span class="sxs-lookup"><span data-stu-id="764da-124">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="764da-125">应接收转发邮件的收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="764da-125">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="764da-126">markAsRead</span><span class="sxs-lookup"><span data-stu-id="764da-126">markAsRead</span></span> | <span data-ttu-id="764da-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="764da-127">Boolean</span></span> | <span data-ttu-id="764da-128">指示是否应将邮件标记为已读。</span><span class="sxs-lookup"><span data-stu-id="764da-128">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="764da-129">markImportance</span><span class="sxs-lookup"><span data-stu-id="764da-129">markImportance</span></span> | <span data-ttu-id="764da-130">String</span><span class="sxs-lookup"><span data-stu-id="764da-130">String</span></span> | <span data-ttu-id="764da-131">设置邮件重要性，可以是：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="764da-131">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="764da-132">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="764da-132">moveToFolder</span></span> |  <span data-ttu-id="764da-133">String</span><span class="sxs-lookup"><span data-stu-id="764da-133">String</span></span>| <span data-ttu-id="764da-134">邮件将移至其中的文件夹的 ID。</span><span class="sxs-lookup"><span data-stu-id="764da-134">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="764da-135">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="764da-135">permanentDelete</span></span> | <span data-ttu-id="764da-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="764da-136">Boolean</span></span> | <span data-ttu-id="764da-137">指示邮件是否应永久删除且不保存到“已删除项目”文件夹。</span><span class="sxs-lookup"><span data-stu-id="764da-137">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="764da-138">redirectTo</span><span class="sxs-lookup"><span data-stu-id="764da-138">redirectTo</span></span> | [<span data-ttu-id="764da-139">recipient</span><span class="sxs-lookup"><span data-stu-id="764da-139">recipient</span></span>](recipient.md) | <span data-ttu-id="764da-140">邮件应重定向到的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="764da-140">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="764da-141">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="764da-141">stopProcessingRules</span></span> | <span data-ttu-id="764da-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="764da-142">Boolean</span></span> | <span data-ttu-id="764da-143">指示是否应对后续规则进行评估。</span><span class="sxs-lookup"><span data-stu-id="764da-143">Indicates whether subsequent rules should be evaluated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="764da-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="764da-144">JSON representation</span></span>
<span data-ttu-id="764da-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="764da-145">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->