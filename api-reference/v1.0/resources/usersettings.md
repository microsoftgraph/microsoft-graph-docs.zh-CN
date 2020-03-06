---
title: userSettings 资源类型
description: '内容发现的当前用户设置。 '
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 862316ba98cab7ccbbaa1c6f7cc909924e400d59
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533419"
---
# <a name="usersettings-resource-type"></a><span data-ttu-id="26226-103">userSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="26226-103">userSettings resource type</span></span>

<span data-ttu-id="26226-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26226-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="26226-105">内容发现的当前用户设置。</span><span class="sxs-lookup"><span data-stu-id="26226-105">The current user settings for content discovery.</span></span>
<span data-ttu-id="26226-106">若要了解如何获取或更新用户设置，请参阅[获取设置](../api/usersettings-get.md)和[更新设置](../api/usersettings-update.md)。</span><span class="sxs-lookup"><span data-stu-id="26226-106">To learn how to get or update user settings, see [Get settings](../api/usersettings-get.md) and [Update settings](../api/usersettings-update.md).</span></span>

<span data-ttu-id="26226-107">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="26226-107">This resource supports:</span></span>

- <span data-ttu-id="26226-108">检查用户及用户的组织是否对内容发现做贡献。</span><span class="sxs-lookup"><span data-stu-id="26226-108">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="26226-109">为特定用户禁用或启用内容发现。</span><span class="sxs-lookup"><span data-stu-id="26226-109">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="26226-110">这也会禁用 Office Delve 中的文档。</span><span class="sxs-lookup"><span data-stu-id="26226-110">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="26226-111">方法</span><span class="sxs-lookup"><span data-stu-id="26226-111">Methods</span></span>
| <span data-ttu-id="26226-112">方法</span><span class="sxs-lookup"><span data-stu-id="26226-112">Method</span></span>       | <span data-ttu-id="26226-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="26226-113">Return Type</span></span>  |<span data-ttu-id="26226-114">说明</span><span class="sxs-lookup"><span data-stu-id="26226-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="26226-115">获取用户设置</span><span class="sxs-lookup"><span data-stu-id="26226-115">Get user settings</span></span>](../api/usersettings-get.md) |[<span data-ttu-id="26226-116">userSettings</span><span class="sxs-lookup"><span data-stu-id="26226-116">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="26226-117">获取用户和组织设置。</span><span class="sxs-lookup"><span data-stu-id="26226-117">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="26226-118">更新用户设置</span><span class="sxs-lookup"><span data-stu-id="26226-118">Update user settings</span></span>](../api/usersettings-update.md) |[<span data-ttu-id="26226-119">userSettings</span><span class="sxs-lookup"><span data-stu-id="26226-119">userSettings</span></span>](../resources/usersettings.md)| <span data-ttu-id="26226-120">更新用户当前的设置。</span><span class="sxs-lookup"><span data-stu-id="26226-120">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="26226-121">属性</span><span class="sxs-lookup"><span data-stu-id="26226-121">Properties</span></span>

| <span data-ttu-id="26226-122">属性</span><span class="sxs-lookup"><span data-stu-id="26226-122">Property</span></span>     | <span data-ttu-id="26226-123">类型</span><span class="sxs-lookup"><span data-stu-id="26226-123">Type</span></span>   |<span data-ttu-id="26226-124">说明</span><span class="sxs-lookup"><span data-stu-id="26226-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26226-125">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="26226-125">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="26226-126">布尔值</span><span class="sxs-lookup"><span data-stu-id="26226-126">Boolean</span></span>|<span data-ttu-id="26226-127">如果设为 true，则会禁用至用户的[趋势](/graph/api/resources/insights-trending?view=graph-rest-beta) API 的委托访问。</span><span class="sxs-lookup"><span data-stu-id="26226-127">When set to true, the delegate access to the user's [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API is disabled.</span></span> <span data-ttu-id="26226-128">如果设为 true，则用户的 Office Delve 中的文档将禁用。</span><span class="sxs-lookup"><span data-stu-id="26226-128">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="26226-129">如果设为 true，则 Office 365 中显示的内容相关性（如 SharePoint 家庭版中的建议网站以及 OneDrive for Business 中的发现视图）将受到影响。</span><span class="sxs-lookup"><span data-stu-id="26226-129">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="26226-130">用户可以在 [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout) 中控制此设置。</span><span class="sxs-lookup"><span data-stu-id="26226-130">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="26226-131">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="26226-131">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="26226-132">布尔值</span><span class="sxs-lookup"><span data-stu-id="26226-132">Boolean</span></span>|<span data-ttu-id="26226-133">反映用于控制至[趋势](/graph/api/resources/insights-trending?view=graph-rest-beta) API 的委托访问的[组织级别设置](https://support.office.com/zh-CN/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)。</span><span class="sxs-lookup"><span data-stu-id="26226-133">Reflects the [organization level setting](https://support.office.com/zh-CN/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API.</span></span> <span data-ttu-id="26226-134">如果设为 true，则组织没有 Office Delve 的访问权限。</span><span class="sxs-lookup"><span data-stu-id="26226-134">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="26226-135">对整个组织来说，Office 365 中显示的内容相关性（如 SharePoint 家庭版中的建议网站以及 OneDrive for Business 中的发现视图）将受到影响。</span><span class="sxs-lookup"><span data-stu-id="26226-135">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="26226-136">此设置为只读，并且仅可由管理员在 [SharePoint 管理中心](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)更改。</span><span class="sxs-lookup"><span data-stu-id="26226-136">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="26226-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26226-137">JSON representation</span></span>

<span data-ttu-id="26226-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26226-138">Here is a JSON representation of the resource.</span></span>

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
