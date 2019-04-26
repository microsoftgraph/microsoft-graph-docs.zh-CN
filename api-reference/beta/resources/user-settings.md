---
title: 设置资源类型
description: '当前用户设置。 '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 208d232af609f92d5924267ae26831b9929e357a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554259"
---
# <a name="settings-resource-type"></a><span data-ttu-id="55edf-103">设置资源类型</span><span class="sxs-lookup"><span data-stu-id="55edf-103">settings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55edf-104">当前用户设置。</span><span class="sxs-lookup"><span data-stu-id="55edf-104">The current user settings.</span></span> <span data-ttu-id="55edf-105">若要了解如何获取或更新用户设置, 请参阅[获取设置](../api/user-get-settings.md)和[更新设置](../api/user-update-settings.md)。</span><span class="sxs-lookup"><span data-stu-id="55edf-105">To learn how to get or update user settings, see [Get settings](../api/user-get-settings.md) and [Update settings](../api/user-update-settings.md).</span></span>

<span data-ttu-id="55edf-106">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="55edf-106">This resource supports:</span></span>

- <span data-ttu-id="55edf-107">检查用户和用户的组织是否参与内容发现。</span><span class="sxs-lookup"><span data-stu-id="55edf-107">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="55edf-108">为特定用户禁用或启用内容发现。</span><span class="sxs-lookup"><span data-stu-id="55edf-108">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="55edf-109">这也会禁用 Office Delve 中的文档。</span><span class="sxs-lookup"><span data-stu-id="55edf-109">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="55edf-110">方法</span><span class="sxs-lookup"><span data-stu-id="55edf-110">Methods</span></span>
| <span data-ttu-id="55edf-111">方法</span><span class="sxs-lookup"><span data-stu-id="55edf-111">Method</span></span>       | <span data-ttu-id="55edf-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="55edf-112">Return Type</span></span>  |<span data-ttu-id="55edf-113">说明</span><span class="sxs-lookup"><span data-stu-id="55edf-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="55edf-114">获取用户设置</span><span class="sxs-lookup"><span data-stu-id="55edf-114">Get user settings</span></span>](../api/user-get-settings.md) |[<span data-ttu-id="55edf-115">settings</span><span class="sxs-lookup"><span data-stu-id="55edf-115">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="55edf-116">获取用户和组织设置。</span><span class="sxs-lookup"><span data-stu-id="55edf-116">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="55edf-117">更新用户设置</span><span class="sxs-lookup"><span data-stu-id="55edf-117">Update user settings</span></span>](../api/user-update-settings.md) |[<span data-ttu-id="55edf-118">settings</span><span class="sxs-lookup"><span data-stu-id="55edf-118">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="55edf-119">更新用户的当前设置。</span><span class="sxs-lookup"><span data-stu-id="55edf-119">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="55edf-120">属性</span><span class="sxs-lookup"><span data-stu-id="55edf-120">Properties</span></span>

| <span data-ttu-id="55edf-121">属性</span><span class="sxs-lookup"><span data-stu-id="55edf-121">Property</span></span>     | <span data-ttu-id="55edf-122">类型</span><span class="sxs-lookup"><span data-stu-id="55edf-122">Type</span></span>   |<span data-ttu-id="55edf-123">说明</span><span class="sxs-lookup"><span data-stu-id="55edf-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55edf-124">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="55edf-124">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="55edf-125">布尔值</span><span class="sxs-lookup"><span data-stu-id="55edf-125">Boolean</span></span>|<span data-ttu-id="55edf-126">当设置为 true 时, 将禁用对用户的[趋势](insights-trending.md)API 的代理访问。</span><span class="sxs-lookup"><span data-stu-id="55edf-126">When set to true, the delegate access to the user's [trending](insights-trending.md) API is disabled.</span></span> <span data-ttu-id="55edf-127">当设置为 true 时, 将禁用用户的 Office Delve 中的文档。</span><span class="sxs-lookup"><span data-stu-id="55edf-127">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="55edf-128">如果设置为 true, 则在 Office 365 中显示的内容的关联性 (例如, SharePoint 主页中的建议网站和 OneDrive for business 中的发现视图) 将受到影响。</span><span class="sxs-lookup"><span data-stu-id="55edf-128">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="55edf-129">用户可在[Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)中控制此设置。</span><span class="sxs-lookup"><span data-stu-id="55edf-129">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="55edf-130">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="55edf-130">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="55edf-131">布尔值</span><span class="sxs-lookup"><span data-stu-id="55edf-131">Boolean</span></span>|<span data-ttu-id="55edf-132">反映了控制对[趋势](insights-trending.md)API 的代理访问的[组织级别设置](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)。</span><span class="sxs-lookup"><span data-stu-id="55edf-132">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](insights-trending.md) API.</span></span> <span data-ttu-id="55edf-133">如果设置为 true, 则组织不具有对 Office Delve 的访问权限。</span><span class="sxs-lookup"><span data-stu-id="55edf-133">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="55edf-134">Office 365 中显示的内容的相关性 (例如, SharePoint 主页中的建议网站和 OneDrive for business 中的发现视图) 对整个组织受到影响。</span><span class="sxs-lookup"><span data-stu-id="55edf-134">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="55edf-135">此设置是只读的, 并且只能由[SharePoint 管理中心](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)中的管理员更改。</span><span class="sxs-lookup"><span data-stu-id="55edf-135">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55edf-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55edf-136">JSON representation</span></span>

<span data-ttu-id="55edf-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55edf-137">Here is a JSON representation of the resource.</span></span>

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/user-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
