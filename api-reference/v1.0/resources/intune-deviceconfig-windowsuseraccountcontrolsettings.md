---
title: windowsUserAccountControlSettings 枚举类型
description: 对于 Windows 用户帐户控制设置的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0475d8fb013cbb07f8d69a659f8ecde2eb580e43
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972472"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="6b382-103">windowsUserAccountControlSettings 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6b382-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="6b382-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6b382-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b382-105">对于 Windows 用户帐户控制设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="6b382-105">Possible values for Windows user account control settings.</span></span>
## <a name="members"></a><span data-ttu-id="6b382-106">成员</span><span class="sxs-lookup"><span data-stu-id="6b382-106">Members</span></span>
|<span data-ttu-id="6b382-107">成员</span><span class="sxs-lookup"><span data-stu-id="6b382-107">Member</span></span>|<span data-ttu-id="6b382-108">值</span><span class="sxs-lookup"><span data-stu-id="6b382-108">Value</span></span>|<span data-ttu-id="6b382-109">说明</span><span class="sxs-lookup"><span data-stu-id="6b382-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b382-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="6b382-110">userDefined</span></span>|<span data-ttu-id="6b382-111">0</span><span class="sxs-lookup"><span data-stu-id="6b382-111">0</span></span>|<span data-ttu-id="6b382-112">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="6b382-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="6b382-113">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="6b382-113">alwaysNotify</span></span>|<span data-ttu-id="6b382-114">1</span><span class="sxs-lookup"><span data-stu-id="6b382-114">1</span></span>|<span data-ttu-id="6b382-115">始终通知。</span><span class="sxs-lookup"><span data-stu-id="6b382-115">Always notify.</span></span>|
|<span data-ttu-id="6b382-116">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="6b382-116">notifyOnAppChanges</span></span>|<span data-ttu-id="6b382-117">2</span><span class="sxs-lookup"><span data-stu-id="6b382-117">2</span></span>|<span data-ttu-id="6b382-118">通知应用程序的更改。</span><span class="sxs-lookup"><span data-stu-id="6b382-118">Notify on app changes.</span></span>|
|<span data-ttu-id="6b382-119">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="6b382-119">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="6b382-120">3</span><span class="sxs-lookup"><span data-stu-id="6b382-120">3</span></span>|<span data-ttu-id="6b382-121">不变暗桌面通知应用程序的更改。</span><span class="sxs-lookup"><span data-stu-id="6b382-121">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="6b382-122">neverNotify</span><span class="sxs-lookup"><span data-stu-id="6b382-122">neverNotify</span></span>|<span data-ttu-id="6b382-123">4</span><span class="sxs-lookup"><span data-stu-id="6b382-123">4</span></span>|<span data-ttu-id="6b382-124">从不通知。</span><span class="sxs-lookup"><span data-stu-id="6b382-124">Never notify.</span></span>|



