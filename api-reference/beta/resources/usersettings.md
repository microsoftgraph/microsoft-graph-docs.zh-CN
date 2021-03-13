---
title: userSettings 资源类型
description: '内容发现的当前用户设置。 '
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 12c75691b5b0515fbf8ef49b54ce1e4a0b806c2c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761770"
---
# <a name="usersettings-resource-type"></a><span data-ttu-id="98d5e-103">userSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="98d5e-103">userSettings resource type</span></span>

<span data-ttu-id="98d5e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98d5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98d5e-105">表示区域设置和语言、排班计划以及[](../resources/regionalandlanguagesettings.md)见解和内容发现的用户[首选项的设置](../resources/officegraphinsights.md)。 [](../resources/shiftpreferences.md)</span><span class="sxs-lookup"><span data-stu-id="98d5e-105">Settings that represent a user’s preferences for [regional locale and languages](../resources/regionalandlanguagesettings.md), for [shift scheduling](../resources/shiftpreferences.md), and for [insights and content discovery](../resources/officegraphinsights.md).</span></span>

<span data-ttu-id="98d5e-106">管理用户基于区域设置首选项：</span><span class="sxs-lookup"><span data-stu-id="98d5e-106">Manage user's locale-based preferences:</span></span> 
  - <span data-ttu-id="98d5e-107">确定用户首选使用哪些语言和区域格式查看应用程序。</span><span class="sxs-lookup"><span data-stu-id="98d5e-107">Determining what language and regional formatting a user prefers to view applications with.</span></span>
  - <span data-ttu-id="98d5e-108">更新用户的语言和区域格式首选项。</span><span class="sxs-lookup"><span data-stu-id="98d5e-108">Updating a user's language and regional formatting preferences.</span></span>

<span data-ttu-id="98d5e-109">管理用户的工作班次首选项：</span><span class="sxs-lookup"><span data-stu-id="98d5e-109">Manage user's work shift preferences:</span></span> 
  - <span data-ttu-id="98d5e-110">检查是否可以在日程安排中为用户分配班次。</span><span class="sxs-lookup"><span data-stu-id="98d5e-110">Checking whether a user can be assigned to shifts in a schedule.</span></span>
  - <span data-ttu-id="98d5e-111">更新用户的班次首选项。</span><span class="sxs-lookup"><span data-stu-id="98d5e-111">Updating a user's shift preferences.</span></span>
  
<span data-ttu-id="98d5e-112">允许发现内容和以文档为中心的见解：</span><span class="sxs-lookup"><span data-stu-id="98d5e-112">Enable discovery of content and document-centric insights:</span></span>
  - <span data-ttu-id="98d5e-113">检查用户及用户的组织是否对内容发现做贡献。</span><span class="sxs-lookup"><span data-stu-id="98d5e-113">Checking whether a user and the user's organization contribute to content discovery.</span></span>
  - <span data-ttu-id="98d5e-114">为特定用户禁用或启用内容发现。</span><span class="sxs-lookup"><span data-stu-id="98d5e-114">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="98d5e-115">这也会禁用 Office Delve 中的文档。</span><span class="sxs-lookup"><span data-stu-id="98d5e-115">This also disables documents in Office Delve.</span></span>

<span data-ttu-id="98d5e-116">若要了解如何获取或更新用户设置，请参阅[获取设置](../api/usersettings-get.md)和[更新设置](../api/usersettings-update.md)。</span><span class="sxs-lookup"><span data-stu-id="98d5e-116">To learn how to get or update user settings, see [Get settings](../api/usersettings-get.md) and [Update settings](../api/usersettings-update.md).</span></span>

> [!NOTE]
> <span data-ttu-id="98d5e-117">此终结点仅适用于用户。</span><span class="sxs-lookup"><span data-stu-id="98d5e-117">This endpoint works only with users.</span></span> <span data-ttu-id="98d5e-118">无法将此终结点用于联系人。</span><span class="sxs-lookup"><span data-stu-id="98d5e-118">You can't use this endpoint with contacts.</span></span>

## <a name="methods"></a><span data-ttu-id="98d5e-119">方法</span><span class="sxs-lookup"><span data-stu-id="98d5e-119">Methods</span></span>
| <span data-ttu-id="98d5e-120">方法</span><span class="sxs-lookup"><span data-stu-id="98d5e-120">Method</span></span>       | <span data-ttu-id="98d5e-121">返回类型</span><span class="sxs-lookup"><span data-stu-id="98d5e-121">Return Type</span></span>  |<span data-ttu-id="98d5e-122">说明</span><span class="sxs-lookup"><span data-stu-id="98d5e-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="98d5e-123">获取用户设置</span><span class="sxs-lookup"><span data-stu-id="98d5e-123">Get user settings</span></span>](../api/usersettings-get.md) |[<span data-ttu-id="98d5e-124">userSettings</span><span class="sxs-lookup"><span data-stu-id="98d5e-124">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="98d5e-125">获取用户和组织设置。</span><span class="sxs-lookup"><span data-stu-id="98d5e-125">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="98d5e-126">更新用户设置</span><span class="sxs-lookup"><span data-stu-id="98d5e-126">Update user settings</span></span>](../api/usersettings-update.md) |[<span data-ttu-id="98d5e-127">userSettings</span><span class="sxs-lookup"><span data-stu-id="98d5e-127">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="98d5e-128">更新用户当前的设置。</span><span class="sxs-lookup"><span data-stu-id="98d5e-128">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="98d5e-129">属性</span><span class="sxs-lookup"><span data-stu-id="98d5e-129">Properties</span></span>

| <span data-ttu-id="98d5e-130">属性</span><span class="sxs-lookup"><span data-stu-id="98d5e-130">Property</span></span>     | <span data-ttu-id="98d5e-131">类型</span><span class="sxs-lookup"><span data-stu-id="98d5e-131">Type</span></span>   |<span data-ttu-id="98d5e-132">说明</span><span class="sxs-lookup"><span data-stu-id="98d5e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98d5e-133">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="98d5e-133">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="98d5e-134">布尔值</span><span class="sxs-lookup"><span data-stu-id="98d5e-134">Boolean</span></span>|<span data-ttu-id="98d5e-135">如果设为 true，则会禁用至用户的[趋势](insights-trending.md) API 的委托访问。</span><span class="sxs-lookup"><span data-stu-id="98d5e-135">When set to true, the delegate access to the user's [trending](insights-trending.md) API is disabled.</span></span> <span data-ttu-id="98d5e-136">如果设为 true，则用户的 Office Delve 中的文档将禁用。</span><span class="sxs-lookup"><span data-stu-id="98d5e-136">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="98d5e-137">如果设为 true，则 Microsoft 365 中显示的内容相关性（如 SharePoint 家庭版中的建议网站以及 OneDrive for Business 中的发现视图）将受到影响。</span><span class="sxs-lookup"><span data-stu-id="98d5e-137">When set to true, the relevancy of the content displayed in Microsoft 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="98d5e-138">用户可以在 [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout) 中控制此设置。</span><span class="sxs-lookup"><span data-stu-id="98d5e-138">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="98d5e-139">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="98d5e-139">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="98d5e-140">布尔值</span><span class="sxs-lookup"><span data-stu-id="98d5e-140">Boolean</span></span>|<span data-ttu-id="98d5e-141">反映用于控制至[趋势](insights-trending.md) API 的委托访问的[组织级别设置](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)。</span><span class="sxs-lookup"><span data-stu-id="98d5e-141">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](insights-trending.md) API.</span></span> <span data-ttu-id="98d5e-142">如果设为 true，则组织没有 Office Delve 的访问权限。</span><span class="sxs-lookup"><span data-stu-id="98d5e-142">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="98d5e-143">对整个组织来说，Microsoft 365 中显示的内容相关性（如 SharePoint 家庭版中的建议网站以及 OneDrive for Business 中的发现视图）将受到影响。</span><span class="sxs-lookup"><span data-stu-id="98d5e-143">The relevancy of the content displayed in Microsoft 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="98d5e-144">此设置为只读，并且仅可由管理员在 [SharePoint 管理中心](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)更改。</span><span class="sxs-lookup"><span data-stu-id="98d5e-144">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="relationships"></a><span data-ttu-id="98d5e-145">关系</span><span class="sxs-lookup"><span data-stu-id="98d5e-145">Relationships</span></span>

| <span data-ttu-id="98d5e-146">关系</span><span class="sxs-lookup"><span data-stu-id="98d5e-146">Relationship</span></span> | <span data-ttu-id="98d5e-147">类型</span><span class="sxs-lookup"><span data-stu-id="98d5e-147">Type</span></span> | <span data-ttu-id="98d5e-148">说明</span><span class="sxs-lookup"><span data-stu-id="98d5e-148">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="98d5e-149">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="98d5e-149">shiftPreferences</span></span>|[<span data-ttu-id="98d5e-150">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="98d5e-150">shiftPreferences</span></span>](shiftpreferences.md)| <span data-ttu-id="98d5e-151">用户的班次首选项。</span><span class="sxs-lookup"><span data-stu-id="98d5e-151">The shift preferences for the user.</span></span> |
|<span data-ttu-id="98d5e-152">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="98d5e-152">regionalAndLanguageSettings</span></span>|[<span data-ttu-id="98d5e-153">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="98d5e-153">regionalAndLanguageSettings</span></span>](regionalandlanguagesettings.md)| <span data-ttu-id="98d5e-154">用户的语言、区域设置和日期/时间格式的首选项。</span><span class="sxs-lookup"><span data-stu-id="98d5e-154">The user's preferences for languages, regional locale and date/time formatting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="98d5e-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98d5e-155">JSON representation</span></span>

<span data-ttu-id="98d5e-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98d5e-156">Here is a JSON representation of the resource.</span></span>
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


