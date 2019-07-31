---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 21769c01603bfb18445fdb073fdd22a4bdbceb23
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001885"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="83bb8-103">appLockerApplicationControlType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="83bb8-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="83bb8-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="83bb8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83bb8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="83bb8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83bb8-106">AppLocker 应用程序控件类型的可能值</span><span class="sxs-lookup"><span data-stu-id="83bb8-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="83bb8-107">成员</span><span class="sxs-lookup"><span data-stu-id="83bb8-107">Members</span></span>
|<span data-ttu-id="83bb8-108">成员</span><span class="sxs-lookup"><span data-stu-id="83bb8-108">Member</span></span>|<span data-ttu-id="83bb8-109">值</span><span class="sxs-lookup"><span data-stu-id="83bb8-109">Value</span></span>|<span data-ttu-id="83bb8-110">说明</span><span class="sxs-lookup"><span data-stu-id="83bb8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83bb8-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="83bb8-111">notConfigured</span></span>|<span data-ttu-id="83bb8-112">0</span><span class="sxs-lookup"><span data-stu-id="83bb8-112">0</span></span>|<span data-ttu-id="83bb8-113">设备默认值, 未选择应用程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="83bb8-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="83bb8-114">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="83bb8-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="83bb8-115">1</span><span class="sxs-lookup"><span data-stu-id="83bb8-115">1</span></span>|<span data-ttu-id="83bb8-116">强制实施 Windows 组件和应用商店应用。</span><span class="sxs-lookup"><span data-stu-id="83bb8-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="83bb8-117">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="83bb8-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="83bb8-118">双面</span><span class="sxs-lookup"><span data-stu-id="83bb8-118">2</span></span>|<span data-ttu-id="83bb8-119">审核 Windows 组件和存储应用程序。</span><span class="sxs-lookup"><span data-stu-id="83bb8-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="83bb8-120">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="83bb8-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="83bb8-121">第三章</span><span class="sxs-lookup"><span data-stu-id="83bb8-121">3</span></span>|<span data-ttu-id="83bb8-122">强制实施 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="83bb8-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="83bb8-123">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="83bb8-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="83bb8-124">4</span><span class="sxs-lookup"><span data-stu-id="83bb8-124">4</span></span>|<span data-ttu-id="83bb8-125">审核 Windows 组件、存储应用和智能保险箱。</span><span class="sxs-lookup"><span data-stu-id="83bb8-125">Audit Windows components, store apps and smart locker.</span></span>|





