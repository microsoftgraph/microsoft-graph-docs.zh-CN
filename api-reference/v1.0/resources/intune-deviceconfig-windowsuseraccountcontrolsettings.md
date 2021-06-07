---
title: windowsUserAccountControlSettings 枚举类型
description: 用户帐户控制Windows的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3b1ebdab6ccfdb84593385beea45d0b62696033f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755782"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="8f3b3-103">windowsUserAccountControlSettings 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8f3b3-103">windowsUserAccountControlSettings enum type</span></span>

<span data-ttu-id="8f3b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f3b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f3b3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8f3b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f3b3-106">用户帐户控制Windows的可能值。</span><span class="sxs-lookup"><span data-stu-id="8f3b3-106">Possible values for Windows user account control settings.</span></span>

## <a name="members"></a><span data-ttu-id="8f3b3-107">成员</span><span class="sxs-lookup"><span data-stu-id="8f3b3-107">Members</span></span>
|<span data-ttu-id="8f3b3-108">成员</span><span class="sxs-lookup"><span data-stu-id="8f3b3-108">Member</span></span>|<span data-ttu-id="8f3b3-109">值</span><span class="sxs-lookup"><span data-stu-id="8f3b3-109">Value</span></span>|<span data-ttu-id="8f3b3-110">Description</span><span class="sxs-lookup"><span data-stu-id="8f3b3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f3b3-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="8f3b3-111">userDefined</span></span>|<span data-ttu-id="8f3b3-112">0</span><span class="sxs-lookup"><span data-stu-id="8f3b3-112">0</span></span>|<span data-ttu-id="8f3b3-113">用户定义，默认值，无意图。</span><span class="sxs-lookup"><span data-stu-id="8f3b3-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="8f3b3-114">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="8f3b3-114">alwaysNotify</span></span>|<span data-ttu-id="8f3b3-115">1</span><span class="sxs-lookup"><span data-stu-id="8f3b3-115">1</span></span>|<span data-ttu-id="8f3b3-116">始终通知。</span><span class="sxs-lookup"><span data-stu-id="8f3b3-116">Always notify.</span></span>|
|<span data-ttu-id="8f3b3-117">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="8f3b3-117">notifyOnAppChanges</span></span>|<span data-ttu-id="8f3b3-118">2</span><span class="sxs-lookup"><span data-stu-id="8f3b3-118">2</span></span>|<span data-ttu-id="8f3b3-119">通知应用更改。</span><span class="sxs-lookup"><span data-stu-id="8f3b3-119">Notify on app changes.</span></span>|
|<span data-ttu-id="8f3b3-120">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="8f3b3-120">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="8f3b3-121">3</span><span class="sxs-lookup"><span data-stu-id="8f3b3-121">3</span></span>|<span data-ttu-id="8f3b3-122">通知应用更改时，桌面不会变暗。</span><span class="sxs-lookup"><span data-stu-id="8f3b3-122">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="8f3b3-123">neverNotify</span><span class="sxs-lookup"><span data-stu-id="8f3b3-123">neverNotify</span></span>|<span data-ttu-id="8f3b3-124">4 </span><span class="sxs-lookup"><span data-stu-id="8f3b3-124">4</span></span>|<span data-ttu-id="8f3b3-125">从不通知。</span><span class="sxs-lookup"><span data-stu-id="8f3b3-125">Never notify.</span></span>|




