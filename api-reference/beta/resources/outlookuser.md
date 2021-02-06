---
title: outlookUser 资源类型
description: 表示用户可用的 Outlook 服务。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 15afe75d10bad489b913eaf7215cbc8327e02317
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130667"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="97b2c-103">outlookUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="97b2c-103">outlookUser resource type</span></span>

<span data-ttu-id="97b2c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97b2c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="97b2c-105">表示用户可用的 Outlook 服务。</span><span class="sxs-lookup"><span data-stu-id="97b2c-105">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="97b2c-106">方法</span><span class="sxs-lookup"><span data-stu-id="97b2c-106">Methods</span></span>

| <span data-ttu-id="97b2c-107">方法</span><span class="sxs-lookup"><span data-stu-id="97b2c-107">Method</span></span>           | <span data-ttu-id="97b2c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="97b2c-108">Return Type</span></span>    |<span data-ttu-id="97b2c-109">说明</span><span class="sxs-lookup"><span data-stu-id="97b2c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="97b2c-110">Create category</span><span class="sxs-lookup"><span data-stu-id="97b2c-110">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="97b2c-111">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="97b2c-111">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="97b2c-112">在用户主类别列表中创建 **outlookCategory** 对象。</span><span class="sxs-lookup"><span data-stu-id="97b2c-112">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="97b2c-113">List categories</span><span class="sxs-lookup"><span data-stu-id="97b2c-113">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="97b2c-114">[outlookCategory](outlookcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97b2c-114">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="97b2c-115">获取为用户定义的所有类别。</span><span class="sxs-lookup"><span data-stu-id="97b2c-115">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="97b2c-116">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="97b2c-116">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="97b2c-117">[localeInfo](localeinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97b2c-117">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="97b2c-118">获取用户支持的区域设置和语言列表，就像在用户的邮箱服务器上配置的那样。</span><span class="sxs-lookup"><span data-stu-id="97b2c-118">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="97b2c-119">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="97b2c-119">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="97b2c-120">[timeZoneInformation](timezoneinformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97b2c-120">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="97b2c-121">获取用户支持的时区列表，就像在用户的邮箱服务器上配置的那样。</span><span class="sxs-lookup"><span data-stu-id="97b2c-121">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |
|<span data-ttu-id="97b2c-122">[创建已弃 (outlookTaskFolder](../api/outlookuser-post-taskfolders.md)) </span><span class="sxs-lookup"><span data-stu-id="97b2c-122">[Create outlookTaskFolder](../api/outlookuser-post-taskfolders.md) (deprecated)</span></span> |[<span data-ttu-id="97b2c-123">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="97b2c-123">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="97b2c-124">在用户邮箱的默认任务组 () `My Tasks` 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="97b2c-124">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>|
|<span data-ttu-id="97b2c-125">[列出已 (taskFolders](../api/outlookuser-list-taskfolders.md)) </span><span class="sxs-lookup"><span data-stu-id="97b2c-125">[List taskFolders](../api/outlookuser-list-taskfolders.md) (deprecated)</span></span> |<span data-ttu-id="97b2c-126">[outlookTaskFolder](outlooktaskfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97b2c-126">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="97b2c-127">获取用户邮箱中所有 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="97b2c-127">Get all the Outlook task folders in the user's mailbox.</span></span>|
|<span data-ttu-id="97b2c-128">[创建已弃 (outlookTaskGroup](../api/outlookuser-post-taskgroups.md)) </span><span class="sxs-lookup"><span data-stu-id="97b2c-128">[Create outlookTaskGroup](../api/outlookuser-post-taskgroups.md) (deprecated)</span></span> |[<span data-ttu-id="97b2c-129">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="97b2c-129">outlookTaskGroup</span></span>](outlooktaskgroup.md)| <span data-ttu-id="97b2c-130">在用户邮箱中创建 Outlook 任务组。</span><span class="sxs-lookup"><span data-stu-id="97b2c-130">Create an Outlook task group in the user's mailbox.</span></span>|
|<span data-ttu-id="97b2c-131">[列出已 (](../api/outlookuser-list-taskgroups.md) 任务组) </span><span class="sxs-lookup"><span data-stu-id="97b2c-131">[List taskGroups](../api/outlookuser-list-taskgroups.md) (deprecated)</span></span> |<span data-ttu-id="97b2c-132">[outlookTaskGroup](outlooktaskgroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97b2c-132">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="97b2c-133">获取用户邮箱中所有的 Outlook 任务组。</span><span class="sxs-lookup"><span data-stu-id="97b2c-133">Get all the Outlook task groups in the user's mailbox.</span></span>|
|<span data-ttu-id="97b2c-134">[创建 outlookTask](../api/outlookuser-post-tasks.md)（已弃用）</span><span class="sxs-lookup"><span data-stu-id="97b2c-134">[Create outlookTask](../api/outlookuser-post-tasks.md) (deprecated)</span></span> |[<span data-ttu-id="97b2c-135">outlookTask</span><span class="sxs-lookup"><span data-stu-id="97b2c-135">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="97b2c-136">在默认任务组 () 创建 Outlook 任务， () `My Tasks` `Tasks` 用户邮箱中的默认任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="97b2c-136">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>|
|<span data-ttu-id="97b2c-137">[列出任务](../api/outlookuser-list-tasks.md)（已弃用）</span><span class="sxs-lookup"><span data-stu-id="97b2c-137">[List tasks](../api/outlookuser-list-tasks.md) (deprecated)</span></span> |<span data-ttu-id="97b2c-138">[outlookTask](outlooktask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97b2c-138">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="97b2c-139">获取用户邮箱中的所有 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="97b2c-139">Get all the Outlook tasks in the user's mailbox.</span></span>|



## <a name="properties"></a><span data-ttu-id="97b2c-140">属性</span><span class="sxs-lookup"><span data-stu-id="97b2c-140">Properties</span></span>
<span data-ttu-id="97b2c-141">无</span><span class="sxs-lookup"><span data-stu-id="97b2c-141">None</span></span>

## <a name="relationships"></a><span data-ttu-id="97b2c-142">关系</span><span class="sxs-lookup"><span data-stu-id="97b2c-142">Relationships</span></span>
| <span data-ttu-id="97b2c-143">关系</span><span class="sxs-lookup"><span data-stu-id="97b2c-143">Relationship</span></span> | <span data-ttu-id="97b2c-144">类型</span><span class="sxs-lookup"><span data-stu-id="97b2c-144">Type</span></span>   |<span data-ttu-id="97b2c-145">说明</span><span class="sxs-lookup"><span data-stu-id="97b2c-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97b2c-146">masterCategories</span><span class="sxs-lookup"><span data-stu-id="97b2c-146">masterCategories</span></span>|<span data-ttu-id="97b2c-147">[outlookCategory](../resources/outlookcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97b2c-147">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="97b2c-148">为用户定义的类别列表。</span><span class="sxs-lookup"><span data-stu-id="97b2c-148">A list of categories defined for the user.</span></span> | 
|<span data-ttu-id="97b2c-149">taskFolders (弃用) </span><span class="sxs-lookup"><span data-stu-id="97b2c-149">taskFolders (deprecated)</span></span>|<span data-ttu-id="97b2c-150">[outlookTaskFolder](outlooktaskfolder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97b2c-150">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="97b2c-151">用户的 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="97b2c-151">The user's Outlook task folders.</span></span> <span data-ttu-id="97b2c-152">只读。</span><span class="sxs-lookup"><span data-stu-id="97b2c-152">Read-only.</span></span> <span data-ttu-id="97b2c-153">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="97b2c-153">Nullable.</span></span>|
|<span data-ttu-id="97b2c-154">taskGroups (弃用) </span><span class="sxs-lookup"><span data-stu-id="97b2c-154">taskGroups (deprecated)</span></span>|<span data-ttu-id="97b2c-155">[outlookTaskGroup](outlooktaskgroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97b2c-155">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="97b2c-156">用户的 Outlook 任务组。</span><span class="sxs-lookup"><span data-stu-id="97b2c-156">The user's Outlook task groups.</span></span> <span data-ttu-id="97b2c-157">只读。</span><span class="sxs-lookup"><span data-stu-id="97b2c-157">Read-only.</span></span> <span data-ttu-id="97b2c-158">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="97b2c-158">Nullable.</span></span>|
|<span data-ttu-id="97b2c-159">任务 (已弃) </span><span class="sxs-lookup"><span data-stu-id="97b2c-159">tasks (deprecated)</span></span>|<span data-ttu-id="97b2c-160">[outlookTask](outlooktask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="97b2c-160">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="97b2c-161">用户的 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="97b2c-161">The user's Outlook tasks.</span></span> <span data-ttu-id="97b2c-162">只读。</span><span class="sxs-lookup"><span data-stu-id="97b2c-162">Read-only.</span></span> <span data-ttu-id="97b2c-163">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="97b2c-163">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97b2c-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97b2c-164">JSON representation</span></span>

<span data-ttu-id="97b2c-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97b2c-165">Here is a JSON representation of the resource</span></span>

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


