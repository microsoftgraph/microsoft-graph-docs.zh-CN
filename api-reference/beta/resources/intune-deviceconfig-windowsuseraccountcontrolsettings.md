---
title: windowsUserAccountControlSettings 枚举类型
description: 对于 Windows 用户帐户控制设置的可能值。
author: tfitzmac
ms.openlocfilehash: dcec2ca6e5b6401b5277e513867c0646bff79c21
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320298"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="202bd-103">windowsUserAccountControlSettings 枚举类型</span><span class="sxs-lookup"><span data-stu-id="202bd-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="202bd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="202bd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="202bd-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="202bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="202bd-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="202bd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="202bd-107">对于 Windows 用户帐户控制设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="202bd-107">Possible values for Windows user account control settings.</span></span>
## <a name="members"></a><span data-ttu-id="202bd-108">成员</span><span class="sxs-lookup"><span data-stu-id="202bd-108">Members</span></span>
|<span data-ttu-id="202bd-109">成员</span><span class="sxs-lookup"><span data-stu-id="202bd-109">Member</span></span>|<span data-ttu-id="202bd-110">值</span><span class="sxs-lookup"><span data-stu-id="202bd-110">Value</span></span>|<span data-ttu-id="202bd-111">说明</span><span class="sxs-lookup"><span data-stu-id="202bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="202bd-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="202bd-112">userDefined</span></span>|<span data-ttu-id="202bd-113">0</span><span class="sxs-lookup"><span data-stu-id="202bd-113">0</span></span>|<span data-ttu-id="202bd-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="202bd-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="202bd-115">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="202bd-115">alwaysNotify</span></span>|<span data-ttu-id="202bd-116">1</span><span class="sxs-lookup"><span data-stu-id="202bd-116">1</span></span>|<span data-ttu-id="202bd-117">始终通知。</span><span class="sxs-lookup"><span data-stu-id="202bd-117">Always notify.</span></span>|
|<span data-ttu-id="202bd-118">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="202bd-118">notifyOnAppChanges</span></span>|<span data-ttu-id="202bd-119">2</span><span class="sxs-lookup"><span data-stu-id="202bd-119">2</span></span>|<span data-ttu-id="202bd-120">通知应用程序的更改。</span><span class="sxs-lookup"><span data-stu-id="202bd-120">Notify on app changes.</span></span>|
|<span data-ttu-id="202bd-121">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="202bd-121">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="202bd-122">3</span><span class="sxs-lookup"><span data-stu-id="202bd-122">3</span></span>|<span data-ttu-id="202bd-123">不变暗桌面通知应用程序的更改。</span><span class="sxs-lookup"><span data-stu-id="202bd-123">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="202bd-124">neverNotify</span><span class="sxs-lookup"><span data-stu-id="202bd-124">neverNotify</span></span>|<span data-ttu-id="202bd-125">4</span><span class="sxs-lookup"><span data-stu-id="202bd-125">4</span></span>|<span data-ttu-id="202bd-126">从不通知。</span><span class="sxs-lookup"><span data-stu-id="202bd-126">Never notify.</span></span>|





