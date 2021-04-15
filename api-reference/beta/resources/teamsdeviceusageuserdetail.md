---
title: teamsDeviceUsageUserDetail 资源类型
description: 表示有关用户 Microsoft Teams 设备使用情况的详细信息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 294ffee8a1a5db208508cce230377285d6834b07
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766054"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="fc442-103">teamsDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="fc442-103">teamsDeviceUsageUserDetail resource type</span></span>

<span data-ttu-id="fc442-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc442-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc442-105">表示有关用户 Microsoft Teams 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="fc442-105">Represents details about Microsoft Teams device usage by user.</span></span>

## <a name="properties"></a><span data-ttu-id="fc442-106">属性</span><span class="sxs-lookup"><span data-stu-id="fc442-106">Properties</span></span>

| <span data-ttu-id="fc442-107">属性</span><span class="sxs-lookup"><span data-stu-id="fc442-107">Property</span></span>          | <span data-ttu-id="fc442-108">类型</span><span class="sxs-lookup"><span data-stu-id="fc442-108">Type</span></span>    | <span data-ttu-id="fc442-109">说明</span><span class="sxs-lookup"><span data-stu-id="fc442-109">Description</span></span>                                                  |
| :---------------- | :------ | ------------------------------------------------------------ |
| <span data-ttu-id="fc442-110">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fc442-110">reportRefreshDate</span></span> | <span data-ttu-id="fc442-111">日期</span><span class="sxs-lookup"><span data-stu-id="fc442-111">Date</span></span>    | <span data-ttu-id="fc442-112">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="fc442-112">The latest date of the content.</span></span>                              |
| <span data-ttu-id="fc442-113">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fc442-113">userPrincipalName</span></span> | <span data-ttu-id="fc442-114">String</span><span class="sxs-lookup"><span data-stu-id="fc442-114">String</span></span>  | <span data-ttu-id="fc442-115">用户的用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="fc442-115">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="fc442-116">UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。</span><span class="sxs-lookup"><span data-stu-id="fc442-116">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="fc442-117">按照惯例，此名称应映射到用户的电子邮件名称。</span><span class="sxs-lookup"><span data-stu-id="fc442-117">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="fc442-118">常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。</span><span class="sxs-lookup"><span data-stu-id="fc442-118">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="fc442-119">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="fc442-119">This property is required when a user is created.</span></span> |
| <span data-ttu-id="fc442-120">isLicensed</span><span class="sxs-lookup"><span data-stu-id="fc442-120">isLicensed</span></span>        | <span data-ttu-id="fc442-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc442-121">Boolean</span></span> | <span data-ttu-id="fc442-122">是否已为用户分配 Teams 许可证。</span><span class="sxs-lookup"><span data-stu-id="fc442-122">Whether the user has been assigned a Teams license.</span></span>          |
| <span data-ttu-id="fc442-123">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="fc442-123">lastActivityDate</span></span>  | <span data-ttu-id="fc442-124">日期</span><span class="sxs-lookup"><span data-stu-id="fc442-124">Date</span></span>    | <span data-ttu-id="fc442-125">用户上次参与 Microsoft Teams 活动的日期。</span><span class="sxs-lookup"><span data-stu-id="fc442-125">The last date that the user participated in a Microsoft Teams activity.</span></span> |
| <span data-ttu-id="fc442-126">isDeleted</span><span class="sxs-lookup"><span data-stu-id="fc442-126">isDeleted</span></span>         | <span data-ttu-id="fc442-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc442-127">Boolean</span></span> | <span data-ttu-id="fc442-128">此用户是已删除还是软删除。</span><span class="sxs-lookup"><span data-stu-id="fc442-128">Whether this user has been deleted or soft deleted.</span></span>          |
| <span data-ttu-id="fc442-129">deletedDate</span><span class="sxs-lookup"><span data-stu-id="fc442-129">deletedDate</span></span>       | <span data-ttu-id="fc442-130">日期</span><span class="sxs-lookup"><span data-stu-id="fc442-130">Date</span></span>    | <span data-ttu-id="fc442-131">删除操作发生的日期。</span><span class="sxs-lookup"><span data-stu-id="fc442-131">The date when the delete operation happened.</span></span> <span data-ttu-id="fc442-132">如果用户尚未删除，则默认值为"null"。</span><span class="sxs-lookup"><span data-stu-id="fc442-132">Default value is "null" when the user has not been deleted.</span></span> |
| <span data-ttu-id="fc442-133">usedWeb</span><span class="sxs-lookup"><span data-stu-id="fc442-133">usedWeb</span></span>           | <span data-ttu-id="fc442-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc442-134">Boolean</span></span> | <span data-ttu-id="fc442-135">用户是否在设备的 Teams Web 客户端中处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="fc442-135">Whether the user was active in the Teams web client on devices.</span></span> |
| <span data-ttu-id="fc442-136">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="fc442-136">usedWindowsPhone</span></span>  | <span data-ttu-id="fc442-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc442-137">Boolean</span></span> | <span data-ttu-id="fc442-138">用户是否在适用于 Windows Phone 的 Teams 移动客户端上处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="fc442-138">Whether the user was active on the Teams mobile client for Windows phone.</span></span> |
| <span data-ttu-id="fc442-139">usediOS</span><span class="sxs-lookup"><span data-stu-id="fc442-139">usediOS</span></span>           | <span data-ttu-id="fc442-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc442-140">Boolean</span></span> | <span data-ttu-id="fc442-141">用户是否在适用于 iOS 的 Teams 移动客户端上处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="fc442-141">Whether the user was active on the Teams mobile client for iOS.</span></span> |
| <span data-ttu-id="fc442-142">usedMac</span><span class="sxs-lookup"><span data-stu-id="fc442-142">usedMac</span></span>           | <span data-ttu-id="fc442-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc442-143">Boolean</span></span> | <span data-ttu-id="fc442-144">用户是否在 macOS 计算机的 Teams 桌面客户端中处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="fc442-144">Whether the user was active in the Teams desktop client on a macOS computer.</span></span> |
| <span data-ttu-id="fc442-145">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="fc442-145">usedAndroidPhone</span></span>  | <span data-ttu-id="fc442-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc442-146">Boolean</span></span> | <span data-ttu-id="fc442-147">用户是否在适用于 Android 的 Teams 移动客户端上处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="fc442-147">Whether the user was active on the Teams mobile client for Android.</span></span> |
| <span data-ttu-id="fc442-148">usedWindows</span><span class="sxs-lookup"><span data-stu-id="fc442-148">usedWindows</span></span>       | <span data-ttu-id="fc442-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc442-149">Boolean</span></span> | <span data-ttu-id="fc442-150">用户是否在基于 Windows 的计算机的 Teams 桌面客户端中处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="fc442-150">Whether the user was active in the Teams desktop client on a Windows-based computer.</span></span> |
| <span data-ttu-id="fc442-151">usedChromeOS</span><span class="sxs-lookup"><span data-stu-id="fc442-151">usedChromeOS</span></span>      | <span data-ttu-id="fc442-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc442-152">Boolean</span></span> | <span data-ttu-id="fc442-153">用户是否在 ChromeOS 计算机的 Teams 桌面客户端中处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="fc442-153">Whether the user was active in the Teams desktop client on a ChromeOS computer.</span></span> |
| <span data-ttu-id="fc442-154">used 过</span><span class="sxs-lookup"><span data-stu-id="fc442-154">usedLinux</span></span>         | <span data-ttu-id="fc442-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc442-155">Boolean</span></span> | <span data-ttu-id="fc442-156">用户在 Linux 计算机的 Teams 桌面客户端中是否处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="fc442-156">Whether the user was active in the Teams desktop client on a Linux computer.</span></span> |
| <span data-ttu-id="fc442-157">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="fc442-157">reportPeriod</span></span>      | <span data-ttu-id="fc442-158">String</span><span class="sxs-lookup"><span data-stu-id="fc442-158">String</span></span>  | <span data-ttu-id="fc442-159">报告涵盖的天数。</span><span class="sxs-lookup"><span data-stu-id="fc442-159">The number of days the report covers.</span></span>                        |

## <a name="json-representation"></a><span data-ttu-id="fc442-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fc442-160">JSON representation</span></span>

<span data-ttu-id="fc442-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc442-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isLicensed": true, 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usediOS": true, 
  "usedMac": true, 
  "usedAndroidPhone": true, 
  "usedWindows": true, 
  "usedChromeOS": true, 
  "usedLinux": true, 
  "reportPeriod": "String"
}
```


