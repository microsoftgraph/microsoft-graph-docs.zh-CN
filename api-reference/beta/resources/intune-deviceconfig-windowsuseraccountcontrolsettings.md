---
title: windowsUserAccountControlSettings 枚举类型
description: 对于 Windows 用户帐户控制设置的可能值。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c2803e2d15b907fc2a05303be8a0b4e4db4ce66f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861451"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="cca18-103">windowsUserAccountControlSettings 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cca18-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="cca18-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cca18-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cca18-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cca18-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cca18-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cca18-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cca18-107">对于 Windows 用户帐户控制设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="cca18-107">Possible values for Windows user account control settings.</span></span>
## <a name="members"></a><span data-ttu-id="cca18-108">成员</span><span class="sxs-lookup"><span data-stu-id="cca18-108">Members</span></span>
|<span data-ttu-id="cca18-109">成员</span><span class="sxs-lookup"><span data-stu-id="cca18-109">Member</span></span>|<span data-ttu-id="cca18-110">值</span><span class="sxs-lookup"><span data-stu-id="cca18-110">Value</span></span>|<span data-ttu-id="cca18-111">Description</span><span class="sxs-lookup"><span data-stu-id="cca18-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cca18-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="cca18-112">userDefined</span></span>|<span data-ttu-id="cca18-113">0</span><span class="sxs-lookup"><span data-stu-id="cca18-113">0</span></span>|<span data-ttu-id="cca18-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="cca18-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="cca18-115">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="cca18-115">alwaysNotify</span></span>|<span data-ttu-id="cca18-116">1</span><span class="sxs-lookup"><span data-stu-id="cca18-116">1</span></span>|<span data-ttu-id="cca18-117">始终通知。</span><span class="sxs-lookup"><span data-stu-id="cca18-117">Always notify.</span></span>|
|<span data-ttu-id="cca18-118">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="cca18-118">notifyOnAppChanges</span></span>|<span data-ttu-id="cca18-119">2</span><span class="sxs-lookup"><span data-stu-id="cca18-119">2</span></span>|<span data-ttu-id="cca18-120">通知应用程序的更改。</span><span class="sxs-lookup"><span data-stu-id="cca18-120">Notify on app changes.</span></span>|
|<span data-ttu-id="cca18-121">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="cca18-121">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="cca18-122">3</span><span class="sxs-lookup"><span data-stu-id="cca18-122">3</span></span>|<span data-ttu-id="cca18-123">不变暗桌面通知应用程序的更改。</span><span class="sxs-lookup"><span data-stu-id="cca18-123">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="cca18-124">neverNotify</span><span class="sxs-lookup"><span data-stu-id="cca18-124">neverNotify</span></span>|<span data-ttu-id="cca18-125">4</span><span class="sxs-lookup"><span data-stu-id="cca18-125">4</span></span>|<span data-ttu-id="cca18-126">从不通知。</span><span class="sxs-lookup"><span data-stu-id="cca18-126">Never notify.</span></span>|





