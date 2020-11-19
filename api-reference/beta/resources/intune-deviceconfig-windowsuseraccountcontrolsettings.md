---
title: windowsUserAccountControlSettings 枚举类型
description: Windows 用户帐户控制设置的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9cfb9120b55fc2ef208f8e0d16fecde216f55d6d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49272302"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="6bfd6-103">windowsUserAccountControlSettings 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6bfd6-103">windowsUserAccountControlSettings enum type</span></span>

<span data-ttu-id="6bfd6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bfd6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6bfd6-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6bfd6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bfd6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6bfd6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bfd6-107">Windows 用户帐户控制设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="6bfd6-107">Possible values for Windows user account control settings.</span></span>

## <a name="members"></a><span data-ttu-id="6bfd6-108">成员</span><span class="sxs-lookup"><span data-stu-id="6bfd6-108">Members</span></span>
|<span data-ttu-id="6bfd6-109">成员</span><span class="sxs-lookup"><span data-stu-id="6bfd6-109">Member</span></span>|<span data-ttu-id="6bfd6-110">值</span><span class="sxs-lookup"><span data-stu-id="6bfd6-110">Value</span></span>|<span data-ttu-id="6bfd6-111">说明</span><span class="sxs-lookup"><span data-stu-id="6bfd6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bfd6-112">定制</span><span class="sxs-lookup"><span data-stu-id="6bfd6-112">userDefined</span></span>|<span data-ttu-id="6bfd6-113">0</span><span class="sxs-lookup"><span data-stu-id="6bfd6-113">0</span></span>|<span data-ttu-id="6bfd6-114">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="6bfd6-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="6bfd6-115">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="6bfd6-115">alwaysNotify</span></span>|<span data-ttu-id="6bfd6-116">1</span><span class="sxs-lookup"><span data-stu-id="6bfd6-116">1</span></span>|<span data-ttu-id="6bfd6-117">总是通知。</span><span class="sxs-lookup"><span data-stu-id="6bfd6-117">Always notify.</span></span>|
|<span data-ttu-id="6bfd6-118">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="6bfd6-118">notifyOnAppChanges</span></span>|<span data-ttu-id="6bfd6-119">双面</span><span class="sxs-lookup"><span data-stu-id="6bfd6-119">2</span></span>|<span data-ttu-id="6bfd6-120">通知应用更改。</span><span class="sxs-lookup"><span data-stu-id="6bfd6-120">Notify on app changes.</span></span>|
|<span data-ttu-id="6bfd6-121">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="6bfd6-121">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="6bfd6-122">第三章</span><span class="sxs-lookup"><span data-stu-id="6bfd6-122">3</span></span>|<span data-ttu-id="6bfd6-123">在应用程序发生更改时通知桌面不变暗。</span><span class="sxs-lookup"><span data-stu-id="6bfd6-123">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="6bfd6-124">neverNotify</span><span class="sxs-lookup"><span data-stu-id="6bfd6-124">neverNotify</span></span>|<span data-ttu-id="6bfd6-125">4 </span><span class="sxs-lookup"><span data-stu-id="6bfd6-125">4</span></span>|<span data-ttu-id="6bfd6-126">从不通知。</span><span class="sxs-lookup"><span data-stu-id="6bfd6-126">Never notify.</span></span>|




