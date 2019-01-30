---
title: outlookUser 资源类型
description: 表示用户可用的 Outlook 服务。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a649de502728bbc51ac53e072c08d95291d20853
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643543"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="28ec6-103">outlookUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="28ec6-103">outlookUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28ec6-104">表示用户可用的 Outlook 服务。</span><span class="sxs-lookup"><span data-stu-id="28ec6-104">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="28ec6-105">方法</span><span class="sxs-lookup"><span data-stu-id="28ec6-105">Methods</span></span>

| <span data-ttu-id="28ec6-106">方法</span><span class="sxs-lookup"><span data-stu-id="28ec6-106">Method</span></span>           | <span data-ttu-id="28ec6-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="28ec6-107">Return Type</span></span>    |<span data-ttu-id="28ec6-108">说明</span><span class="sxs-lookup"><span data-stu-id="28ec6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="28ec6-109">Create category</span><span class="sxs-lookup"><span data-stu-id="28ec6-109">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="28ec6-110">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="28ec6-110">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="28ec6-111">在用户主类别列表中创建 **outlookCategory** 对象。</span><span class="sxs-lookup"><span data-stu-id="28ec6-111">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="28ec6-112">List categories</span><span class="sxs-lookup"><span data-stu-id="28ec6-112">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="28ec6-113">[outlookCategory](outlookcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="28ec6-113">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="28ec6-114">获取为用户定义的所有类别。</span><span class="sxs-lookup"><span data-stu-id="28ec6-114">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="28ec6-115">创建 outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="28ec6-115">Create outlookTaskFolder</span></span>](../api/outlookuser-post-taskfolders.md) |[<span data-ttu-id="28ec6-116">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="28ec6-116">outlookTaskFolder</span></span>](outlooktaskfolder.md)| <span data-ttu-id="28ec6-117">创建任务文件夹中的默认任务组 (`My Tasks`) 的用户的邮箱。</span><span class="sxs-lookup"><span data-stu-id="28ec6-117">Create a task folder in the default task group (`My Tasks`) of the user's mailbox.</span></span>|
|[<span data-ttu-id="28ec6-118">列表 taskFolders</span><span class="sxs-lookup"><span data-stu-id="28ec6-118">List taskFolders</span></span>](../api/outlookuser-list-taskfolders.md) |<span data-ttu-id="28ec6-119">[outlookTaskFolder](outlooktaskfolder.md)集合</span><span class="sxs-lookup"><span data-stu-id="28ec6-119">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="28ec6-120">获取用户的邮箱中的所有 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="28ec6-120">Get all the Outlook task folders in the user's mailbox.</span></span>|
|[<span data-ttu-id="28ec6-121">创建 outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="28ec6-121">Create outlookTaskGroup</span></span>](../api/outlookuser-post-taskgroups.md) |[<span data-ttu-id="28ec6-122">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="28ec6-122">outlookTaskGroup</span></span>](outlooktaskgroup.md)| <span data-ttu-id="28ec6-123">在用户邮箱中创建 Outlook 任务组。</span><span class="sxs-lookup"><span data-stu-id="28ec6-123">Create an Outlook task group in the user's mailbox.</span></span>|
|[<span data-ttu-id="28ec6-124">列表 taskGroups</span><span class="sxs-lookup"><span data-stu-id="28ec6-124">List taskGroups</span></span>](../api/outlookuser-list-taskgroups.md) |<span data-ttu-id="28ec6-125">[outlookTaskGroup](outlooktaskgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="28ec6-125">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="28ec6-126">获取用户的邮箱中的所有 Outlook 任务组。</span><span class="sxs-lookup"><span data-stu-id="28ec6-126">Get all the Outlook task groups in the user's mailbox.</span></span>|
|[<span data-ttu-id="28ec6-127">创建 outlookTask</span><span class="sxs-lookup"><span data-stu-id="28ec6-127">Create outlookTask</span></span>](../api/outlookuser-post-tasks.md) |[<span data-ttu-id="28ec6-128">outlookTask</span><span class="sxs-lookup"><span data-stu-id="28ec6-128">outlookTask</span></span>](outlooktask.md)| <span data-ttu-id="28ec6-129">创建 Outlook 任务中的默认任务组 (`My Tasks`) 和默认任务文件夹 (`Tasks`) 用户的邮箱中。</span><span class="sxs-lookup"><span data-stu-id="28ec6-129">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>|
|[<span data-ttu-id="28ec6-130">List tasks</span><span class="sxs-lookup"><span data-stu-id="28ec6-130">List tasks</span></span>](../api/outlookuser-list-tasks.md) |<span data-ttu-id="28ec6-131">[outlookTask](outlooktask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="28ec6-131">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="28ec6-132">获取用户的邮箱中的所有 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="28ec6-132">Get all the Outlook tasks in the user's mailbox.</span></span>|
|[<span data-ttu-id="28ec6-133">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="28ec6-133">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="28ec6-134">[localeInfo](localeinfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="28ec6-134">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="28ec6-135">获取用户支持的区域设置和语言列表，就像在用户的邮箱服务器上配置的那样。</span><span class="sxs-lookup"><span data-stu-id="28ec6-135">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="28ec6-136">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="28ec6-136">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="28ec6-137">[timeZoneInformation](timezoneinformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="28ec6-137">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="28ec6-138">获取用户支持的时区列表，就像在用户的邮箱服务器上配置的那样。</span><span class="sxs-lookup"><span data-stu-id="28ec6-138">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="28ec6-139">属性</span><span class="sxs-lookup"><span data-stu-id="28ec6-139">Properties</span></span>
<span data-ttu-id="28ec6-140">无</span><span class="sxs-lookup"><span data-stu-id="28ec6-140">None</span></span>

## <a name="relationships"></a><span data-ttu-id="28ec6-141">关系</span><span class="sxs-lookup"><span data-stu-id="28ec6-141">Relationships</span></span>
| <span data-ttu-id="28ec6-142">关系</span><span class="sxs-lookup"><span data-stu-id="28ec6-142">Relationship</span></span> | <span data-ttu-id="28ec6-143">类型</span><span class="sxs-lookup"><span data-stu-id="28ec6-143">Type</span></span>   |<span data-ttu-id="28ec6-144">说明</span><span class="sxs-lookup"><span data-stu-id="28ec6-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28ec6-145">masterCategories</span><span class="sxs-lookup"><span data-stu-id="28ec6-145">masterCategories</span></span>|<span data-ttu-id="28ec6-146">[outlookCategory](../resources/outlookcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="28ec6-146">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="28ec6-147">为用户定义的类别列表。</span><span class="sxs-lookup"><span data-stu-id="28ec6-147">A list of categories defined for the user.</span></span> | 
|<span data-ttu-id="28ec6-148">taskFolders</span><span class="sxs-lookup"><span data-stu-id="28ec6-148">taskFolders</span></span>|<span data-ttu-id="28ec6-149">[outlookTaskFolder](outlooktaskfolder.md)集合</span><span class="sxs-lookup"><span data-stu-id="28ec6-149">[outlookTaskFolder](outlooktaskfolder.md) collection</span></span>| <span data-ttu-id="28ec6-150">用户的 Outlook 任务文件夹。</span><span class="sxs-lookup"><span data-stu-id="28ec6-150">The user's Outlook task folders.</span></span> <span data-ttu-id="28ec6-151">只读。</span><span class="sxs-lookup"><span data-stu-id="28ec6-151">Read-only.</span></span> <span data-ttu-id="28ec6-152">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="28ec6-152">Nullable.</span></span>|
|<span data-ttu-id="28ec6-153">taskGroups</span><span class="sxs-lookup"><span data-stu-id="28ec6-153">taskGroups</span></span>|<span data-ttu-id="28ec6-154">[outlookTaskGroup](outlooktaskgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="28ec6-154">[outlookTaskGroup](outlooktaskgroup.md) collection</span></span>| <span data-ttu-id="28ec6-155">用户的 Outlook 任务组。</span><span class="sxs-lookup"><span data-stu-id="28ec6-155">The user's Outlook task groups.</span></span> <span data-ttu-id="28ec6-156">只读。</span><span class="sxs-lookup"><span data-stu-id="28ec6-156">Read-only.</span></span> <span data-ttu-id="28ec6-157">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="28ec6-157">Nullable.</span></span>|
|<span data-ttu-id="28ec6-158">tasks</span><span class="sxs-lookup"><span data-stu-id="28ec6-158">tasks</span></span>|<span data-ttu-id="28ec6-159">[outlookTask](outlooktask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="28ec6-159">[outlookTask](outlooktask.md) collection</span></span>| <span data-ttu-id="28ec6-160">用户的 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="28ec6-160">The user's Outlook tasks.</span></span> <span data-ttu-id="28ec6-161">只读。</span><span class="sxs-lookup"><span data-stu-id="28ec6-161">Read-only.</span></span> <span data-ttu-id="28ec6-162">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="28ec6-162">Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlookuser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
