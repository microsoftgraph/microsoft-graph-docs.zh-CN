---
title: windowsUserAccountControlSettings 枚举类型
description: 对于 Windows 用户帐户控制设置的可能值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ff348fd33e6bbc8370378783cf0a517a205ea101
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399813"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="63625-103">windowsUserAccountControlSettings 枚举类型</span><span class="sxs-lookup"><span data-stu-id="63625-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="63625-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="63625-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="63625-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="63625-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63625-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="63625-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63625-107">对于 Windows 用户帐户控制设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="63625-107">Possible values for Windows user account control settings.</span></span>

## <a name="members"></a><span data-ttu-id="63625-108">成员</span><span class="sxs-lookup"><span data-stu-id="63625-108">Members</span></span>
|<span data-ttu-id="63625-109">成员</span><span class="sxs-lookup"><span data-stu-id="63625-109">Member</span></span>|<span data-ttu-id="63625-110">值</span><span class="sxs-lookup"><span data-stu-id="63625-110">Value</span></span>|<span data-ttu-id="63625-111">说明</span><span class="sxs-lookup"><span data-stu-id="63625-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63625-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="63625-112">userDefined</span></span>|<span data-ttu-id="63625-113">0</span><span class="sxs-lookup"><span data-stu-id="63625-113">0</span></span>|<span data-ttu-id="63625-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="63625-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="63625-115">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="63625-115">alwaysNotify</span></span>|<span data-ttu-id="63625-116">1</span><span class="sxs-lookup"><span data-stu-id="63625-116">1</span></span>|<span data-ttu-id="63625-117">始终通知。</span><span class="sxs-lookup"><span data-stu-id="63625-117">Always notify.</span></span>|
|<span data-ttu-id="63625-118">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="63625-118">notifyOnAppChanges</span></span>|<span data-ttu-id="63625-119">2</span><span class="sxs-lookup"><span data-stu-id="63625-119">2</span></span>|<span data-ttu-id="63625-120">通知应用程序的更改。</span><span class="sxs-lookup"><span data-stu-id="63625-120">Notify on app changes.</span></span>|
|<span data-ttu-id="63625-121">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="63625-121">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="63625-122">3</span><span class="sxs-lookup"><span data-stu-id="63625-122">3</span></span>|<span data-ttu-id="63625-123">不变暗桌面通知应用程序的更改。</span><span class="sxs-lookup"><span data-stu-id="63625-123">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="63625-124">neverNotify</span><span class="sxs-lookup"><span data-stu-id="63625-124">neverNotify</span></span>|<span data-ttu-id="63625-125">4</span><span class="sxs-lookup"><span data-stu-id="63625-125">4</span></span>|<span data-ttu-id="63625-126">从不通知。</span><span class="sxs-lookup"><span data-stu-id="63625-126">Never notify.</span></span>|




