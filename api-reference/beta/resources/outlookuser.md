---
title: outlookUser 资源类型
description: 表示用户可用的 Outlook 服务。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: eadd5947a03fce69f790e2e9f0a4d738078002cd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522065"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="97eb4-103">outlookUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="97eb4-103">outlookUser resource type</span></span>

<span data-ttu-id="97eb4-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="97eb4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97eb4-105">表示用户可用的 Outlook 服务。</span><span class="sxs-lookup"><span data-stu-id="97eb4-105">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="97eb4-106">方法</span><span class="sxs-lookup"><span data-stu-id="97eb4-106">Methods</span></span>

| <span data-ttu-id="97eb4-107">方法</span><span class="sxs-lookup"><span data-stu-id="97eb4-107">Method</span></span>           | <span data-ttu-id="97eb4-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="97eb4-108">Return Type</span></span>    |<span data-ttu-id="97eb4-109">说明</span><span class="sxs-lookup"><span data-stu-id="97eb4-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="97eb4-110">Create category</span><span class="sxs-lookup"><span data-stu-id="97eb4-110">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="97eb4-111">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="97eb4-111">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="97eb4-112">在用户主类别列表中创建 **outlookCategory** 对象。</span><span class="sxs-lookup"><span data-stu-id="97eb4-112">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="97eb4-113">List categories</span><span class="sxs-lookup"><span data-stu-id="97eb4-113">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="97eb4-114">[outlookCategory](outlookcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97eb4-114">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="97eb4-115">获取为用户定义的所有类别。</span><span class="sxs-lookup"><span data-stu-id="97eb4-115">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="97eb4-116">创建 outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="97eb4-116">Create outlookTaskFolder</span></span>](../api/outlookuser-post-taskfolders.md) |[<span data-ttu-id="97eb4-117">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="97eb4-117">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="97eb4-118">在用户邮箱的默认任务组（`My Tasks`）中创建一个任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="97eb4-118">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>|
|[<span data-ttu-id="97eb4-119">列出 taskFolders</span><span class="sxs-lookup"><span data-stu-id="97eb4-119">List taskFolders</span></span>](../api/outlookuser-list-taskfolders.md) |<span data-ttu-id="97eb4-120">[outlookTaskFolder](outlooktaskfolder.md)集合</span><span class="sxs-lookup"><span data-stu-id="97eb4-120">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="97eb4-121">获取用户邮箱中的所有 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="97eb4-121">Get all the Outlook task folders in the user's mailbox.</span></span>|
|[<span data-ttu-id="97eb4-122">创建 outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="97eb4-122">Create outlookTaskGroup</span></span>](../api/outlookuser-post-taskgroups.md) |[<span data-ttu-id="97eb4-123">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="97eb4-123">outlookTaskGroup</span></span>](outlooktaskgroup.md)| <span data-ttu-id="97eb4-124">在用户的邮箱中创建一个 Outlook 任务组。</span><span class="sxs-lookup"><span data-stu-id="97eb4-124">Create an Outlook task group in the user's mailbox.</span></span>|
|[<span data-ttu-id="97eb4-125">列出 taskGroups</span><span class="sxs-lookup"><span data-stu-id="97eb4-125">List taskGroups</span></span>](../api/outlookuser-list-taskgroups.md) |<span data-ttu-id="97eb4-126">[outlookTaskGroup](outlooktaskgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="97eb4-126">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="97eb4-127">获取用户邮箱中的所有 Outlook 任务组。</span><span class="sxs-lookup"><span data-stu-id="97eb4-127">Get all the Outlook task groups in the user's mailbox.</span></span>|
|[<span data-ttu-id="97eb4-128">创建 outlookTask</span><span class="sxs-lookup"><span data-stu-id="97eb4-128">Create outlookTask</span></span>](../api/outlookuser-post-tasks.md) |[<span data-ttu-id="97eb4-129">outlookTask</span><span class="sxs-lookup"><span data-stu-id="97eb4-129">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="97eb4-130">在用户邮箱中的默认任务组（`My Tasks`）和默认任务文件夹（`Tasks`）中创建一个 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="97eb4-130">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>|
|[<span data-ttu-id="97eb4-131">列出任务</span><span class="sxs-lookup"><span data-stu-id="97eb4-131">List tasks</span></span>](../api/outlookuser-list-tasks.md) |<span data-ttu-id="97eb4-132">[outlookTask](outlooktask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97eb4-132">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="97eb4-133">获取用户邮箱中的所有 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="97eb4-133">Get all the Outlook tasks in the user's mailbox.</span></span>|
|[<span data-ttu-id="97eb4-134">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="97eb4-134">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="97eb4-135">[localeInfo](localeinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97eb4-135">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="97eb4-136">获取用户支持的区域设置和语言列表，就像在用户的邮箱服务器上配置的那样。</span><span class="sxs-lookup"><span data-stu-id="97eb4-136">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="97eb4-137">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="97eb4-137">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="97eb4-138">[timeZoneInformation](timezoneinformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97eb4-138">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="97eb4-139">获取用户支持的时区列表，就像在用户的邮箱服务器上配置的那样。</span><span class="sxs-lookup"><span data-stu-id="97eb4-139">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="97eb4-140">属性</span><span class="sxs-lookup"><span data-stu-id="97eb4-140">Properties</span></span>
<span data-ttu-id="97eb4-141">无</span><span class="sxs-lookup"><span data-stu-id="97eb4-141">None</span></span>

## <a name="relationships"></a><span data-ttu-id="97eb4-142">关系</span><span class="sxs-lookup"><span data-stu-id="97eb4-142">Relationships</span></span>
| <span data-ttu-id="97eb4-143">关系</span><span class="sxs-lookup"><span data-stu-id="97eb4-143">Relationship</span></span> | <span data-ttu-id="97eb4-144">类型</span><span class="sxs-lookup"><span data-stu-id="97eb4-144">Type</span></span>   |<span data-ttu-id="97eb4-145">说明</span><span class="sxs-lookup"><span data-stu-id="97eb4-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97eb4-146">masterCategories</span><span class="sxs-lookup"><span data-stu-id="97eb4-146">masterCategories</span></span>|<span data-ttu-id="97eb4-147">[outlookCategory](../resources/outlookcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97eb4-147">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="97eb4-148">为用户定义的类别列表。</span><span class="sxs-lookup"><span data-stu-id="97eb4-148">A list of categories defined for the user.</span></span> | 
|<span data-ttu-id="97eb4-149">taskFolders</span><span class="sxs-lookup"><span data-stu-id="97eb4-149">taskFolders</span></span>|<span data-ttu-id="97eb4-150">[outlookTaskFolder](outlooktaskfolder.md)集合</span><span class="sxs-lookup"><span data-stu-id="97eb4-150">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="97eb4-151">用户的 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="97eb4-151">The user's Outlook task folders.</span></span> <span data-ttu-id="97eb4-152">只读。</span><span class="sxs-lookup"><span data-stu-id="97eb4-152">Read-only.</span></span> <span data-ttu-id="97eb4-153">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="97eb4-153">Nullable.</span></span>|
|<span data-ttu-id="97eb4-154">taskGroups</span><span class="sxs-lookup"><span data-stu-id="97eb4-154">taskGroups</span></span>|<span data-ttu-id="97eb4-155">[outlookTaskGroup](outlooktaskgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="97eb4-155">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="97eb4-156">用户的 Outlook 任务组。</span><span class="sxs-lookup"><span data-stu-id="97eb4-156">The user's Outlook task groups.</span></span> <span data-ttu-id="97eb4-157">只读。</span><span class="sxs-lookup"><span data-stu-id="97eb4-157">Read-only.</span></span> <span data-ttu-id="97eb4-158">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="97eb4-158">Nullable.</span></span>|
|<span data-ttu-id="97eb4-159">任务</span><span class="sxs-lookup"><span data-stu-id="97eb4-159">tasks</span></span>|<span data-ttu-id="97eb4-160">[outlookTask](outlooktask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97eb4-160">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="97eb4-161">用户的 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="97eb4-161">The user's Outlook tasks.</span></span> <span data-ttu-id="97eb4-162">只读。</span><span class="sxs-lookup"><span data-stu-id="97eb4-162">Read-only.</span></span> <span data-ttu-id="97eb4-163">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="97eb4-163">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97eb4-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97eb4-164">JSON representation</span></span>

<span data-ttu-id="97eb4-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97eb4-165">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.outlookUser"
}-->
```json
{  
    "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
