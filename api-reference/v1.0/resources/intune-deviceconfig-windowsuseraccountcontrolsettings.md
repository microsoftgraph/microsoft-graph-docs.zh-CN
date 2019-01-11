---
title: windowsUserAccountControlSettings 枚举类型
description: 对于 Windows 用户帐户控制设置的可能值。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 02ea15b10b0eb6a789456d9f91e63ca3249a0933
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810659"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="585da-103">windowsUserAccountControlSettings 枚举类型</span><span class="sxs-lookup"><span data-stu-id="585da-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="585da-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="585da-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="585da-105">对于 Windows 用户帐户控制设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="585da-105">Possible values for Windows user account control settings.</span></span>
## <a name="members"></a><span data-ttu-id="585da-106">成员</span><span class="sxs-lookup"><span data-stu-id="585da-106">Members</span></span>
|<span data-ttu-id="585da-107">成员</span><span class="sxs-lookup"><span data-stu-id="585da-107">Member</span></span>|<span data-ttu-id="585da-108">值</span><span class="sxs-lookup"><span data-stu-id="585da-108">Value</span></span>|<span data-ttu-id="585da-109">Description</span><span class="sxs-lookup"><span data-stu-id="585da-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="585da-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="585da-110">userDefined</span></span>|<span data-ttu-id="585da-111">0</span><span class="sxs-lookup"><span data-stu-id="585da-111">0</span></span>|<span data-ttu-id="585da-112">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="585da-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="585da-113">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="585da-113">alwaysNotify</span></span>|<span data-ttu-id="585da-114">1</span><span class="sxs-lookup"><span data-stu-id="585da-114">1</span></span>|<span data-ttu-id="585da-115">始终通知。</span><span class="sxs-lookup"><span data-stu-id="585da-115">Always notify.</span></span>|
|<span data-ttu-id="585da-116">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="585da-116">notifyOnAppChanges</span></span>|<span data-ttu-id="585da-117">2</span><span class="sxs-lookup"><span data-stu-id="585da-117">2</span></span>|<span data-ttu-id="585da-118">通知应用程序的更改。</span><span class="sxs-lookup"><span data-stu-id="585da-118">Notify on app changes.</span></span>|
|<span data-ttu-id="585da-119">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="585da-119">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="585da-120">3</span><span class="sxs-lookup"><span data-stu-id="585da-120">3</span></span>|<span data-ttu-id="585da-121">不变暗桌面通知应用程序的更改。</span><span class="sxs-lookup"><span data-stu-id="585da-121">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="585da-122">neverNotify</span><span class="sxs-lookup"><span data-stu-id="585da-122">neverNotify</span></span>|<span data-ttu-id="585da-123">4</span><span class="sxs-lookup"><span data-stu-id="585da-123">4</span></span>|<span data-ttu-id="585da-124">从不通知。</span><span class="sxs-lookup"><span data-stu-id="585da-124">Never notify.</span></span>|



