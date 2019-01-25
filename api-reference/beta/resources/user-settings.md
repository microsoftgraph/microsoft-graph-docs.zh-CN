---
title: 设置资源类型
description: '当前用户设置。 '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 208d232af609f92d5924267ae26831b9929e357a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521094"
---
# <a name="settings-resource-type"></a><span data-ttu-id="8c44e-103">设置资源类型</span><span class="sxs-lookup"><span data-stu-id="8c44e-103">settings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c44e-104">当前用户设置。</span><span class="sxs-lookup"><span data-stu-id="8c44e-104">The current user settings.</span></span> <span data-ttu-id="8c44e-105">若要了解如何获取或更新用户设置，请参阅[获取设置](../api/user-get-settings.md)并[更新设置](../api/user-update-settings.md)。</span><span class="sxs-lookup"><span data-stu-id="8c44e-105">To learn how to get or update user settings, see [Get settings](../api/user-get-settings.md) and [Update settings](../api/user-update-settings.md).</span></span>

<span data-ttu-id="8c44e-106">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="8c44e-106">This resource supports:</span></span>

- <span data-ttu-id="8c44e-107">检查用户和用户的组织是否为内容发现参与。</span><span class="sxs-lookup"><span data-stu-id="8c44e-107">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="8c44e-108">如果禁用或启用特定用户的内容发现。</span><span class="sxs-lookup"><span data-stu-id="8c44e-108">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="8c44e-109">这还将禁用 Office 深入中的文档。</span><span class="sxs-lookup"><span data-stu-id="8c44e-109">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="8c44e-110">方法</span><span class="sxs-lookup"><span data-stu-id="8c44e-110">Methods</span></span>
| <span data-ttu-id="8c44e-111">方法</span><span class="sxs-lookup"><span data-stu-id="8c44e-111">Method</span></span>       | <span data-ttu-id="8c44e-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="8c44e-112">Return Type</span></span>  |<span data-ttu-id="8c44e-113">说明</span><span class="sxs-lookup"><span data-stu-id="8c44e-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c44e-114">获取用户设置</span><span class="sxs-lookup"><span data-stu-id="8c44e-114">[Get user settings](../api/user-get-settings.md)</span></span> |[<span data-ttu-id="8c44e-115">Settings</span><span class="sxs-lookup"><span data-stu-id="8c44e-115">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="8c44e-116">获取用户和组织设置。</span><span class="sxs-lookup"><span data-stu-id="8c44e-116">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="8c44e-117">更新用户设置</span><span class="sxs-lookup"><span data-stu-id="8c44e-117">Update user settings</span></span>](../api/user-update-settings.md) |[<span data-ttu-id="8c44e-118">Settings</span><span class="sxs-lookup"><span data-stu-id="8c44e-118">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="8c44e-119">更新用户的当前设置。</span><span class="sxs-lookup"><span data-stu-id="8c44e-119">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="8c44e-120">属性</span><span class="sxs-lookup"><span data-stu-id="8c44e-120">Properties</span></span>

| <span data-ttu-id="8c44e-121">属性</span><span class="sxs-lookup"><span data-stu-id="8c44e-121">Property</span></span>     | <span data-ttu-id="8c44e-122">类型</span><span class="sxs-lookup"><span data-stu-id="8c44e-122">Type</span></span>   |<span data-ttu-id="8c44e-123">说明</span><span class="sxs-lookup"><span data-stu-id="8c44e-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c44e-124">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="8c44e-124">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="8c44e-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c44e-125">Boolean</span></span>|<span data-ttu-id="8c44e-126">设置为 true，代理访问权限的用户时禁用[趋势](insights-trending.md)API。</span><span class="sxs-lookup"><span data-stu-id="8c44e-126">When set to true, the delegate access to the user's [trending](insights-trending.md) API is disabled.</span></span> <span data-ttu-id="8c44e-127">当设置为在用户的 Office 深入为 true，则文档将被禁用。</span><span class="sxs-lookup"><span data-stu-id="8c44e-127">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="8c44e-128">当设置为 true，Office 365，例如在建议的网站中 SharePoint 主页中显示的内容的相关性和受影响的 OneDrive for Business 中的发现视图。</span><span class="sxs-lookup"><span data-stu-id="8c44e-128">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="8c44e-129">用户可以控制在[Office 深入](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)此设置。</span><span class="sxs-lookup"><span data-stu-id="8c44e-129">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="8c44e-130">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="8c44e-130">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="8c44e-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c44e-131">Boolean</span></span>|<span data-ttu-id="8c44e-132">反映[组织级别设置](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)控制对[趋势](insights-trending.md)API 的代理访问。</span><span class="sxs-lookup"><span data-stu-id="8c44e-132">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](insights-trending.md) API.</span></span> <span data-ttu-id="8c44e-133">当设置为 true，组织不具有对 Office 深入的访问。</span><span class="sxs-lookup"><span data-stu-id="8c44e-133">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="8c44e-134">为整个组织受影响的 Office 365，例如在建议的网站中 SharePoint 主页和 OneDrive for Business 中的发现视图中显示的内容相关性。</span><span class="sxs-lookup"><span data-stu-id="8c44e-134">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="8c44e-135">此设置是只读的并且只能通过[SharePoint 管理中心](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)中的管理员来更改。</span><span class="sxs-lookup"><span data-stu-id="8c44e-135">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8c44e-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c44e-136">JSON representation</span></span>

<span data-ttu-id="8c44e-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c44e-137">Here is a JSON representation of the resource.</span></span>

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
