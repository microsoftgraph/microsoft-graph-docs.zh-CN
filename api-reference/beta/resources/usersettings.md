---
title: userSettings 资源类型
description: '内容发现的当前用户设置。 '
author: krbain
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 81391c38f2577fd3f60c57fa40f9671ae710c2a2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057771"
---
# <a name="usersettings-resource-type"></a><span data-ttu-id="c1f16-103">userSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="c1f16-103">userSettings resource type</span></span>

<span data-ttu-id="c1f16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1f16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1f16-105">代表用户对 [区域区域设置和语言](../resources/regionalandlanguagesettings.md)的首选项、用于 [倒班计划](../resources/shiftpreferences.md)以及用于 [真知灼见和内容发现](../resources/officegraphinsights.md)的设置。</span><span class="sxs-lookup"><span data-stu-id="c1f16-105">Settings that represent a user’s preferences for [regional locale and languages](../resources/regionalandlanguagesettings.md), for [shift scheduling](../resources/shiftpreferences.md), and for [insights and content discovery](../resources/officegraphinsights.md).</span></span>

<span data-ttu-id="c1f16-106">管理用户的基于区域设置的首选项：</span><span class="sxs-lookup"><span data-stu-id="c1f16-106">Manage user's locale-based preferences:</span></span> 
  - <span data-ttu-id="c1f16-107">确定用户在查看应用程序时首选的语言和区域格式。</span><span class="sxs-lookup"><span data-stu-id="c1f16-107">Determining what language and regional formatting a user prefers to view applications with.</span></span>
  - <span data-ttu-id="c1f16-108">更新用户的语言和区域格式设置首选项。</span><span class="sxs-lookup"><span data-stu-id="c1f16-108">Updating a user's language and regional formatting preferences.</span></span>

<span data-ttu-id="c1f16-109">管理用户的工作班次首选项：</span><span class="sxs-lookup"><span data-stu-id="c1f16-109">Manage user's work shift preferences:</span></span> 
  - <span data-ttu-id="c1f16-110">检查是否可将用户分配给计划中的班次。</span><span class="sxs-lookup"><span data-stu-id="c1f16-110">Checking whether a user can be assigned to shifts in a schedule.</span></span>
  - <span data-ttu-id="c1f16-111">更新用户的 shift 首选项。</span><span class="sxs-lookup"><span data-stu-id="c1f16-111">Updating a user's shift preferences.</span></span>
  
<span data-ttu-id="c1f16-112">启用内容发现和以文档为中心的见解：</span><span class="sxs-lookup"><span data-stu-id="c1f16-112">Enable discovery of content and document-centric insights:</span></span>
  - <span data-ttu-id="c1f16-113">检查用户及用户的组织是否对内容发现做贡献。</span><span class="sxs-lookup"><span data-stu-id="c1f16-113">Checking whether a user and the user's organization contribute to content discovery.</span></span>
  - <span data-ttu-id="c1f16-114">为特定用户禁用或启用内容发现。</span><span class="sxs-lookup"><span data-stu-id="c1f16-114">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="c1f16-115">这也会禁用 Office Delve 中的文档。</span><span class="sxs-lookup"><span data-stu-id="c1f16-115">This also disables documents in Office Delve.</span></span>

<span data-ttu-id="c1f16-116">若要了解如何获取或更新用户设置，请参阅[获取设置](../api/usersettings-get.md)和[更新设置](../api/usersettings-update.md)。</span><span class="sxs-lookup"><span data-stu-id="c1f16-116">To learn how to get or update user settings, see [Get settings](../api/usersettings-get.md) and [Update settings](../api/usersettings-update.md).</span></span>

> [!NOTE]
> <span data-ttu-id="c1f16-117">此终结点仅适用于用户。</span><span class="sxs-lookup"><span data-stu-id="c1f16-117">This endpoint works only with users.</span></span> <span data-ttu-id="c1f16-118">无法将此终结点用于联系人。</span><span class="sxs-lookup"><span data-stu-id="c1f16-118">You can't use this endpoint with contacts.</span></span>

## <a name="methods"></a><span data-ttu-id="c1f16-119">方法</span><span class="sxs-lookup"><span data-stu-id="c1f16-119">Methods</span></span>
| <span data-ttu-id="c1f16-120">方法</span><span class="sxs-lookup"><span data-stu-id="c1f16-120">Method</span></span>       | <span data-ttu-id="c1f16-121">返回类型</span><span class="sxs-lookup"><span data-stu-id="c1f16-121">Return Type</span></span>  |<span data-ttu-id="c1f16-122">说明</span><span class="sxs-lookup"><span data-stu-id="c1f16-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c1f16-123">获取用户设置</span><span class="sxs-lookup"><span data-stu-id="c1f16-123">Get user settings</span></span>](../api/usersettings-get.md) |[<span data-ttu-id="c1f16-124">userSettings</span><span class="sxs-lookup"><span data-stu-id="c1f16-124">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="c1f16-125">获取用户和组织设置。</span><span class="sxs-lookup"><span data-stu-id="c1f16-125">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="c1f16-126">更新用户设置</span><span class="sxs-lookup"><span data-stu-id="c1f16-126">Update user settings</span></span>](../api/usersettings-update.md) |[<span data-ttu-id="c1f16-127">userSettings</span><span class="sxs-lookup"><span data-stu-id="c1f16-127">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="c1f16-128">更新用户当前的设置。</span><span class="sxs-lookup"><span data-stu-id="c1f16-128">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="c1f16-129">属性</span><span class="sxs-lookup"><span data-stu-id="c1f16-129">Properties</span></span>

| <span data-ttu-id="c1f16-130">属性</span><span class="sxs-lookup"><span data-stu-id="c1f16-130">Property</span></span>     | <span data-ttu-id="c1f16-131">类型</span><span class="sxs-lookup"><span data-stu-id="c1f16-131">Type</span></span>   |<span data-ttu-id="c1f16-132">说明</span><span class="sxs-lookup"><span data-stu-id="c1f16-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1f16-133">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="c1f16-133">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="c1f16-134">布尔值</span><span class="sxs-lookup"><span data-stu-id="c1f16-134">Boolean</span></span>|<span data-ttu-id="c1f16-135">如果设为 true，则会禁用至用户的[趋势](insights-trending.md) API 的委托访问。</span><span class="sxs-lookup"><span data-stu-id="c1f16-135">When set to true, the delegate access to the user's [trending](insights-trending.md) API is disabled.</span></span> <span data-ttu-id="c1f16-136">如果设为 true，则用户的 Office Delve 中的文档将禁用。</span><span class="sxs-lookup"><span data-stu-id="c1f16-136">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="c1f16-137">如果设置为 true，则在 Microsoft 365 中显示的内容的关联性（例如，SharePoint 主页中的建议网站和 OneDrive for Business 中的发现视图）将受到影响。</span><span class="sxs-lookup"><span data-stu-id="c1f16-137">When set to true, the relevancy of the content displayed in Microsoft 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="c1f16-138">用户可以在 [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout) 中控制此设置。</span><span class="sxs-lookup"><span data-stu-id="c1f16-138">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="c1f16-139">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="c1f16-139">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="c1f16-140">布尔值</span><span class="sxs-lookup"><span data-stu-id="c1f16-140">Boolean</span></span>|<span data-ttu-id="c1f16-141">反映用于控制至[趋势](insights-trending.md) API 的委托访问的[组织级别设置](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)。</span><span class="sxs-lookup"><span data-stu-id="c1f16-141">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](insights-trending.md) API.</span></span> <span data-ttu-id="c1f16-142">如果设为 true，则组织没有 Office Delve 的访问权限。</span><span class="sxs-lookup"><span data-stu-id="c1f16-142">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="c1f16-143">Microsoft 365 中显示的内容的相关性（例如，SharePoint 主页中的建议网站和 OneDrive for Business 中的发现视图）对整个组织受到影响。</span><span class="sxs-lookup"><span data-stu-id="c1f16-143">The relevancy of the content displayed in Microsoft 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="c1f16-144">此设置为只读，并且仅可由管理员在 [SharePoint 管理中心](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)更改。</span><span class="sxs-lookup"><span data-stu-id="c1f16-144">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1f16-145">关系</span><span class="sxs-lookup"><span data-stu-id="c1f16-145">Relationships</span></span>

| <span data-ttu-id="c1f16-146">关系</span><span class="sxs-lookup"><span data-stu-id="c1f16-146">Relationship</span></span> | <span data-ttu-id="c1f16-147">类型</span><span class="sxs-lookup"><span data-stu-id="c1f16-147">Type</span></span> | <span data-ttu-id="c1f16-148">说明</span><span class="sxs-lookup"><span data-stu-id="c1f16-148">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c1f16-149">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="c1f16-149">shiftPreferences</span></span>|[<span data-ttu-id="c1f16-150">shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="c1f16-150">shiftPreferences</span></span>](shiftpreferences.md)| <span data-ttu-id="c1f16-151">用户的 shift 首选项。</span><span class="sxs-lookup"><span data-stu-id="c1f16-151">The shift preferences for the user.</span></span> |
|<span data-ttu-id="c1f16-152">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="c1f16-152">regionalAndLanguageSettings</span></span>|[<span data-ttu-id="c1f16-153">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="c1f16-153">regionalAndLanguageSettings</span></span>](regionalandlanguagesettings.md)| <span data-ttu-id="c1f16-154">用户的语言首选项、区域区域设置和日期/时间格式。</span><span class="sxs-lookup"><span data-stu-id="c1f16-154">The user's preferences for languages, regional locale and date/time formatting.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c1f16-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c1f16-155">JSON representation</span></span>

<span data-ttu-id="c1f16-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1f16-156">Here is a JSON representation of the resource.</span></span>
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


