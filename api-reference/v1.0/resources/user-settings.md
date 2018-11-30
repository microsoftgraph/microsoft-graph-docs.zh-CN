---
title: 设置资源类型
description: '当前用户设置。 '
ms.openlocfilehash: 291ec0b8d11a94d082534f5a890b556df89d665e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010154"
---
# <a name="settings-resource-type"></a><span data-ttu-id="5647f-103">设置资源类型</span><span class="sxs-lookup"><span data-stu-id="5647f-103">settings resource type</span></span>

<span data-ttu-id="5647f-104">当前用户设置。</span><span class="sxs-lookup"><span data-stu-id="5647f-104">The current user settings.</span></span> <span data-ttu-id="5647f-105">若要了解如何获取或更新用户设置，请参阅[获取设置](../api/user-get-settings.md)并[更新设置](../api/user-update-settings.md)。</span><span class="sxs-lookup"><span data-stu-id="5647f-105">To learn how to get or update user settings, see [Get settings](../api/user-get-settings.md) and [Update settings](../api/user-update-settings.md).</span></span>

<span data-ttu-id="5647f-106">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="5647f-106">This resource supports:</span></span>

- <span data-ttu-id="5647f-107">检查用户和用户的组织是否为内容发现参与。</span><span class="sxs-lookup"><span data-stu-id="5647f-107">Checking whether a user and the user's organization contribute to content discovery.</span></span>
- <span data-ttu-id="5647f-108">如果禁用或启用特定用户的内容发现。</span><span class="sxs-lookup"><span data-stu-id="5647f-108">Disabling or enabling content discovery for specific users.</span></span> <span data-ttu-id="5647f-109">这还将禁用 Office 深入中的文档。</span><span class="sxs-lookup"><span data-stu-id="5647f-109">This also disables documents in Office Delve.</span></span>

## <a name="methods"></a><span data-ttu-id="5647f-110">方法</span><span class="sxs-lookup"><span data-stu-id="5647f-110">Methods</span></span>
| <span data-ttu-id="5647f-111">方法</span><span class="sxs-lookup"><span data-stu-id="5647f-111">Method</span></span>       | <span data-ttu-id="5647f-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="5647f-112">Return Type</span></span>  |<span data-ttu-id="5647f-113">说明</span><span class="sxs-lookup"><span data-stu-id="5647f-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5647f-114">获取用户设置</span><span class="sxs-lookup"><span data-stu-id="5647f-114">Get user settings</span></span>](../api/user-get-settings.md) |[<span data-ttu-id="5647f-115">设置</span><span class="sxs-lookup"><span data-stu-id="5647f-115">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="5647f-116">获取用户和组织设置。</span><span class="sxs-lookup"><span data-stu-id="5647f-116">Get the user and organization settings.</span></span> |
|[<span data-ttu-id="5647f-117">更新用户设置</span><span class="sxs-lookup"><span data-stu-id="5647f-117">Update user settings</span></span>](../api/user-update-settings.md) |[<span data-ttu-id="5647f-118">设置</span><span class="sxs-lookup"><span data-stu-id="5647f-118">settings</span></span>](../resources/user-settings.md)| <span data-ttu-id="5647f-119">更新用户的当前设置。</span><span class="sxs-lookup"><span data-stu-id="5647f-119">Update the user current settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="5647f-120">属性</span><span class="sxs-lookup"><span data-stu-id="5647f-120">Properties</span></span>

| <span data-ttu-id="5647f-121">属性</span><span class="sxs-lookup"><span data-stu-id="5647f-121">Property</span></span>     | <span data-ttu-id="5647f-122">类型</span><span class="sxs-lookup"><span data-stu-id="5647f-122">Type</span></span>   |<span data-ttu-id="5647f-123">说明</span><span class="sxs-lookup"><span data-stu-id="5647f-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5647f-124">contributionToContentDiscoveryDisabled</span><span class="sxs-lookup"><span data-stu-id="5647f-124">contributionToContentDiscoveryDisabled</span></span>|<span data-ttu-id="5647f-125">布尔</span><span class="sxs-lookup"><span data-stu-id="5647f-125">Boolean</span></span>|<span data-ttu-id="5647f-126">设置为 true，代理访问权限的用户时禁用[趋势](/graph/api/resources/insights-trending?view=graph-rest-beta)API。</span><span class="sxs-lookup"><span data-stu-id="5647f-126">When set to true, the delegate access to the user's [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API is disabled.</span></span> <span data-ttu-id="5647f-127">当设置为在用户的 Office 深入为 true，则文档将被禁用。</span><span class="sxs-lookup"><span data-stu-id="5647f-127">When set to true, documents in the user's Office Delve are disabled.</span></span> <span data-ttu-id="5647f-128">当设置为 true，Office 365，例如在建议的网站中 SharePoint 主页中显示的内容的相关性和受影响的 OneDrive for Business 中的发现视图。</span><span class="sxs-lookup"><span data-stu-id="5647f-128">When set to true, the relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected.</span></span> <span data-ttu-id="5647f-129">用户可以控制在[Office 深入](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)此设置。</span><span class="sxs-lookup"><span data-stu-id="5647f-129">Users can control this setting in [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).</span></span> |
|<span data-ttu-id="5647f-130">contributionToContentDiscoveryAsOrganizationDisabled</span><span class="sxs-lookup"><span data-stu-id="5647f-130">contributionToContentDiscoveryAsOrganizationDisabled</span></span>|<span data-ttu-id="5647f-131">布尔</span><span class="sxs-lookup"><span data-stu-id="5647f-131">Boolean</span></span>|<span data-ttu-id="5647f-132">反映[组织级别设置](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff)控制对[趋势](/graph/api/resources/insights-trending?view=graph-rest-beta)API 的代理访问。</span><span class="sxs-lookup"><span data-stu-id="5647f-132">Reflects the [organization level setting](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlling delegate access to the [trending](/graph/api/resources/insights-trending?view=graph-rest-beta) API.</span></span> <span data-ttu-id="5647f-133">当设置为 true，组织不具有对 Office 深入的访问。</span><span class="sxs-lookup"><span data-stu-id="5647f-133">When set to true, the organization doesn't have access to Office Delve.</span></span> <span data-ttu-id="5647f-134">为整个组织受影响的 Office 365，例如在建议的网站中 SharePoint 主页和 OneDrive for Business 中的发现视图中显示的内容相关性。</span><span class="sxs-lookup"><span data-stu-id="5647f-134">The relevancy of the content displayed in Office 365, for example in Suggested sites in SharePoint Home and the Discover view in OneDrive for Business is affected for the whole organization.</span></span> <span data-ttu-id="5647f-135">此设置是只读的并且只能通过[SharePoint 管理中心](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)中的管理员来更改。</span><span class="sxs-lookup"><span data-stu-id="5647f-135">This setting is read-only and can only be changed by administrators in the [SharePoint admin center](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5647f-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5647f-136">JSON representation</span></span>

<span data-ttu-id="5647f-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5647f-137">Here is a JSON representation of the resource.</span></span>

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```