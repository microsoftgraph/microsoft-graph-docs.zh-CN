---
title: userSettings 资源类型
description: '内容发现的当前用户设置。 '
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: a16ab96bb04f6d7dfc4f9ceff29f49dc7d348d23
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108871"
---
# <a name="usersettings-resource-type"></a><span data-ttu-id="42787-103">userSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="42787-103">userSettings resource type</span></span>

<span data-ttu-id="42787-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42787-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42787-105">设置表示用户对区域设置和语言、排班、排[](../resources/regionalandlanguagesettings.md)班和项目Delve[首选项](../resources/officegraphinsights.md)的首选项[](../resources/shiftpreferences.md)。</span><span class="sxs-lookup"><span data-stu-id="42787-105">Settings that represent a user’s preferences for [regional locale and languages](../resources/regionalandlanguagesettings.md), for [shift scheduling](../resources/shiftpreferences.md), for Delve and for [item insights](../resources/officegraphinsights.md).</span></span>

<span data-ttu-id="42787-106">管理用户基于区域设置首选项：</span><span class="sxs-lookup"><span data-stu-id="42787-106">Manage user's locale-based preferences:</span></span> 
  - <span data-ttu-id="42787-107">确定用户首选使用哪些语言和区域格式查看应用程序。</span><span class="sxs-lookup"><span data-stu-id="42787-107">Determining what language and regional formatting a user prefers to view applications with.</span></span>
  - <span data-ttu-id="42787-108">更新用户的语言和区域格式首选项。</span><span class="sxs-lookup"><span data-stu-id="42787-108">Updating a user's language and regional formatting preferences.</span></span>

<span data-ttu-id="42787-109">管理用户的工作班次首选项：</span><span class="sxs-lookup"><span data-stu-id="42787-109">Manage user's work shift preferences:</span></span> 
  - <span data-ttu-id="42787-110">检查是否可以在日程安排中为用户分配班次。</span><span class="sxs-lookup"><span data-stu-id="42787-110">Checking whether a user can be assigned to shifts in a schedule.</span></span>
  - <span data-ttu-id="42787-111">更新用户的班次首选项。</span><span class="sxs-lookup"><span data-stu-id="42787-111">Updating a user's shift preferences.</span></span>
  
<span data-ttu-id="42787-112">管理Delve辅助功能：</span><span class="sxs-lookup"><span data-stu-id="42787-112">Manage Delve accessibility:</span></span>
  - <span data-ttu-id="42787-113">检查用户及其组织是否有权访问Office Delve。</span><span class="sxs-lookup"><span data-stu-id="42787-113">Checking whether a user and the user's organization have access to Office Delve.</span></span>
  - <span data-ttu-id="42787-114">为特定用户禁用或Office Delve文档。</span><span class="sxs-lookup"><span data-stu-id="42787-114">Disabling or enabling documents in Office Delve for specific users.</span></span> 

<span data-ttu-id="42787-115">配置 [itemInsights 的可见性](../resources/iteminsights.md) 和 [会议时间见解](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1)。</span><span class="sxs-lookup"><span data-stu-id="42787-115">Configure the visibility of [itemInsights](../resources/iteminsights.md) and [meeting hours insights](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1).</span></span> <span data-ttu-id="42787-116">ItemInsight 在用户和其他项目之间派生 (如文档中的文档) 网站Microsoft 365：</span><span class="sxs-lookup"><span data-stu-id="42787-116">ItemInsights are derived between users and other items (such as documents or sites) in Microsoft 365:</span></span>
  - <span data-ttu-id="42787-117">检查是否已启用用户的项目和会议时间见解。</span><span class="sxs-lookup"><span data-stu-id="42787-117">Checking whether a user's item and meeting hours insights are enabled.</span></span>
  - <span data-ttu-id="42787-118">为特定用户禁用或启用项和会议时间见解。</span><span class="sxs-lookup"><span data-stu-id="42787-118">Disabling or enabling item and meeting hours insights for specific user.</span></span>

<span data-ttu-id="42787-119">若要了解如何获取或更新用户设置，请参阅[获取设置](../api/usersettings-get.md)和[更新设置](../api/usersettings-update.md)。</span><span class="sxs-lookup"><span data-stu-id="42787-119">To learn how to get or update user settings, see [Get settings](../api/usersettings-get.md) and [Update settings](../api/usersettings-update.md).</span></span>

> [!NOTE]
> <span data-ttu-id="42787-120">此终结点仅适用于用户。</span><span class="sxs-lookup"><span data-stu-id="42787-120">This endpoint works only with users.</span></span> <span data-ttu-id="42787-121">无法将此终结点用于联系人。</span><span class="sxs-lookup"><span data-stu-id="42787-121">You can't use this endpoint with contacts.</span></span>

## <a name="methods"></a><span data-ttu-id="42787-122">方法</span><span class="sxs-lookup"><span data-stu-id="42787-122">Methods</span></span>
| <span data-ttu-id="42787-123">方法</span><span class="sxs-lookup"><span data-stu-id="42787-123">Method</span></span>       | <span data-ttu-id="42787-124">返回类型</span><span class="sxs-lookup"><span data-stu-id="42787-124">Return Type</span></span>  |<span data-ttu-id="42787-125">说明</span><span class="sxs-lookup"><span data-stu-id="42787-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="42787-126">获取用户设置</span><span class="sxs-lookup"><span data-stu-id="42787-126">Get user settings</span></span>](../api/usersettings-get.md) |[<span data-ttu-id="42787-127">userSettings</span><span class="sxs-lookup"><span data-stu-id="42787-127">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="42787-128">获取用户和组织设置。</span><span class="sxs-lookup"><span data-stu-id="42787-128">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="42787-129">更新用户设置</span><span class="sxs-lookup"><span data-stu-id="42787-129">Update user settings</span></span>](../api/usersettings-update.md) |[<span data-ttu-id="42787-130">userSettings</span><span class="sxs-lookup"><span data-stu-id="42787-130">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="42787-131">更新用户当前的设置。</span><span class="sxs-lookup"><span data-stu-id="42787-131">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="42787-132">属性</span><span class="sxs-lookup"><span data-stu-id="42787-132">Properties</span></span>

| <span data-ttu-id="42787-133">属性</span><span class="sxs-lookup"><span data-stu-id="42787-133">Property</span></span>     | <span data-ttu-id="42787-134">类型</span><span class="sxs-lookup"><span data-stu-id="42787-134">Type</span></span>   |<span data-ttu-id="42787-135">说明</span><span class="sxs-lookup"><span data-stu-id="42787-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42787-136">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="42787-136">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="42787-137">布尔值</span><span class="sxs-lookup"><span data-stu-id="42787-137">Boolean</span></span>|<span data-ttu-id="42787-138">如果设为 true，则用户的 Office Delve 中的文档将禁用。</span><span class="sxs-lookup"><span data-stu-id="42787-138">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="42787-139">用户可以在 [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout) 中控制此设置。</span><span class="sxs-lookup"><span data-stu-id="42787-139">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="42787-140">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="42787-140">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="42787-141">布尔值</span><span class="sxs-lookup"><span data-stu-id="42787-141">Boolean</span></span>|<span data-ttu-id="42787-142">反映Office Delve[级别设置](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)。</span><span class="sxs-lookup"><span data-stu-id="42787-142">Reflects the [Office Delve organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff).</span></span> <span data-ttu-id="42787-143">如果设为 true，则组织没有 Office Delve 的访问权限。</span><span class="sxs-lookup"><span data-stu-id="42787-143">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="42787-144">此设置为只读，并且仅可由管理员在 [SharePoint 管理中心](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)更改。</span><span class="sxs-lookup"><span data-stu-id="42787-144">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="relationships"></a><span data-ttu-id="42787-145">关系</span><span class="sxs-lookup"><span data-stu-id="42787-145">Relationships</span></span>

| <span data-ttu-id="42787-146">关系</span><span class="sxs-lookup"><span data-stu-id="42787-146">Relationship</span></span> | <span data-ttu-id="42787-147">类型</span><span class="sxs-lookup"><span data-stu-id="42787-147">Type</span></span> | <span data-ttu-id="42787-148">说明</span><span class="sxs-lookup"><span data-stu-id="42787-148">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="42787-149">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="42787-149">shiftPreferences</span></span>|[<span data-ttu-id="42787-150">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="42787-150">shiftPreferences</span></span>](shiftpreferences.md)| <span data-ttu-id="42787-151">用户的班次首选项。</span><span class="sxs-lookup"><span data-stu-id="42787-151">The shift preferences for the user.</span></span> |
|<span data-ttu-id="42787-152">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="42787-152">regionalAndLanguageSettings</span></span>|[<span data-ttu-id="42787-153">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="42787-153">regionalAndLanguageSettings</span></span>](regionalandlanguagesettings.md)| <span data-ttu-id="42787-154">用户的语言、区域设置和日期/时间格式的首选项。</span><span class="sxs-lookup"><span data-stu-id="42787-154">The user's preferences for languages, regional locale and date/time formatting.</span></span> |
|<span data-ttu-id="42787-155">itemInsights</span><span class="sxs-lookup"><span data-stu-id="42787-155">itemInsights</span></span>|[<span data-ttu-id="42787-156">userInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="42787-156">userInsightsSettings</span></span>](userinsightssettings.md)| <span data-ttu-id="42787-157">用户设置，用于查看会议时间见解，以及从用户与 Microsoft 365（如文档或网站）中派生的见解。</span><span class="sxs-lookup"><span data-stu-id="42787-157">The user's settings for the visibility of meeting hour insights, and insights derived between a user and other items in Microsoft 365, such as documents or sites.</span></span> <span data-ttu-id="42787-158">[通过此导航属性获取 userInsightsSettings。](../api/userinsightssettings-get.md)</span><span class="sxs-lookup"><span data-stu-id="42787-158">[Get userInsightsSettings](../api/userinsightssettings-get.md) through this navigation property.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="42787-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42787-159">JSON representation</span></span>

<span data-ttu-id="42787-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42787-160">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userSettings",
  "baseType": "microsoft.graph.entity"
}-->
```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```


