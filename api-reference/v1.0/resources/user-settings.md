---
title: 设置资源类型
description: '当前用户设置。 '
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 433824e715940f2309619a0467179ef99ee3daec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456926"
---
# <a name="settings-resource-type"></a><span data-ttu-id="ed7a5-103">设置资源类型</span><span class="sxs-lookup"><span data-stu-id="ed7a5-103">settings resource type</span></span>

<span data-ttu-id="ed7a5-104">当前用户设置。</span><span class="sxs-lookup"><span data-stu-id="ed7a5-104">The current user.</span></span> <span data-ttu-id="ed7a5-105">若要了解如何获取或更新用户设置，请参阅[获取设置](../api/user-get-settings.md)和[更新设置](../api/user-update-settings.md)。</span><span class="sxs-lookup"><span data-stu-id="ed7a5-105">To learn how to get or update user settings, see [Get settings](../api/user-get-settings.md) and [Update settings](../api/user-update-settings.md).</span></span>

<span data-ttu-id="ed7a5-106">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="ed7a5-106">This resource supports:</span></span>

- <span data-ttu-id="ed7a5-107">检查用户及用户的组织是否对内容发现做贡献。</span><span class="sxs-lookup"><span data-stu-id="ed7a5-107">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="ed7a5-108">为特定用户禁用或启用内容发现。</span><span class="sxs-lookup"><span data-stu-id="ed7a5-108">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="ed7a5-109">这也会禁用 Office Delve 中的文档。</span><span class="sxs-lookup"><span data-stu-id="ed7a5-109">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="ed7a5-110">方法</span><span class="sxs-lookup"><span data-stu-id="ed7a5-110">Methods</span></span>
| <span data-ttu-id="ed7a5-111">方法</span><span class="sxs-lookup"><span data-stu-id="ed7a5-111">Method</span></span>       | <span data-ttu-id="ed7a5-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="ed7a5-112">Return Type</span></span>  |<span data-ttu-id="ed7a5-113">说明</span><span class="sxs-lookup"><span data-stu-id="ed7a5-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed7a5-114">[获取用户设置](../api/user-get-settings.md)</span><span class="sxs-lookup"><span data-stu-id="ed7a5-114">[](../api/user-get-settings.md)Get user mailbox settings</span></span> |[<span data-ttu-id="ed7a5-115">settings</span><span class="sxs-lookup"><span data-stu-id="ed7a5-115">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="ed7a5-116">获取用户和组织设置。</span><span class="sxs-lookup"><span data-stu-id="ed7a5-116">Get the user and organization settings.</span></span> |
|<span data-ttu-id="ed7a5-117">[更新用户设置](../api/user-update-settings.md)</span><span class="sxs-lookup"><span data-stu-id="ed7a5-117">[](../api/user-update-settings.md)Update user mailbox settings</span></span> |[<span data-ttu-id="ed7a5-118">settings</span><span class="sxs-lookup"><span data-stu-id="ed7a5-118">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="ed7a5-119">更新用户当前的设置。</span><span class="sxs-lookup"><span data-stu-id="ed7a5-119">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="ed7a5-120">属性</span><span class="sxs-lookup"><span data-stu-id="ed7a5-120">Properties</span></span>

| <span data-ttu-id="ed7a5-121">属性</span><span class="sxs-lookup"><span data-stu-id="ed7a5-121">Property</span></span>     | <span data-ttu-id="ed7a5-122">类型</span><span class="sxs-lookup"><span data-stu-id="ed7a5-122">Type</span></span>   |<span data-ttu-id="ed7a5-123">说明</span><span class="sxs-lookup"><span data-stu-id="ed7a5-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed7a5-124">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="ed7a5-124">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="ed7a5-125">布尔值</span><span class="sxs-lookup"><span data-stu-id="ed7a5-125">Boolean</span></span>|<span data-ttu-id="ed7a5-126">如果设为 true，则会禁用至用户的[趋势](/graph/api/resources/insights-trending?view=graph-rest-beta) API 的委托访问。</span><span class="sxs-lookup"><span data-stu-id="ed7a5-126">When set to true, the delegate access to the user's [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API is disabled.</span></span> <span data-ttu-id="ed7a5-127">如果设为 true，则用户的 Office Delve 中的文档将禁用。</span><span class="sxs-lookup"><span data-stu-id="ed7a5-127">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="ed7a5-128">如果设为 true，则 Office 365 中显示的内容相关性（如 SharePoint 家庭版中的建议网站以及 OneDrive for Business 中的发现视图）将受到影响。</span><span class="sxs-lookup"><span data-stu-id="ed7a5-128">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="ed7a5-129">用户可以在 [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout) 中控制此设置。</span><span class="sxs-lookup"><span data-stu-id="ed7a5-129">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="ed7a5-130">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="ed7a5-130">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="ed7a5-131">布尔值</span><span class="sxs-lookup"><span data-stu-id="ed7a5-131">Boolean</span></span>|<span data-ttu-id="ed7a5-132">反映用于控制至[趋势](/graph/api/resources/insights-trending?view=graph-rest-beta) API 的委托访问的[组织级别设置](https://support.office.com/zh-CN/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)。</span><span class="sxs-lookup"><span data-stu-id="ed7a5-132">Reflects the [organization level setting](https://support.office.com/zh-CN/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API.</span></span> <span data-ttu-id="ed7a5-133">如果设为 true，则组织没有 Office Delve 的访问权限。</span><span class="sxs-lookup"><span data-stu-id="ed7a5-133">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="ed7a5-134">对整个组织来说，Office 365 中显示的内容相关性（如 SharePoint 家庭版中的建议网站以及 OneDrive for Business 中的发现视图）将受到影响。</span><span class="sxs-lookup"><span data-stu-id="ed7a5-134">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="ed7a5-135">此设置为只读，并且仅可由管理员在 [SharePoint 管理中心](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)更改。</span><span class="sxs-lookup"><span data-stu-id="ed7a5-135">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ed7a5-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed7a5-136">JSON representation</span></span>

<span data-ttu-id="ed7a5-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed7a5-137">Here is a JSON representation of the resource.</span></span>

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
