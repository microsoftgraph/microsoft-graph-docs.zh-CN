---
title: androidDeviceOwnerSystemUpdateInstallType 枚举类型
description: Android 设备所有者的系统更新类型。
author: tfitzmac
ms.openlocfilehash: e2dc66851e0fa98d52a3fec30385e0fd27e6f6ca
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323196"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="ef93a-103">androidDeviceOwnerSystemUpdateInstallType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ef93a-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

> <span data-ttu-id="ef93a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ef93a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef93a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ef93a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef93a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ef93a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef93a-107">Android 设备所有者的系统更新类型。</span><span class="sxs-lookup"><span data-stu-id="ef93a-107">System Update Types for Android Device Owner.</span></span>
## <a name="members"></a><span data-ttu-id="ef93a-108">成员</span><span class="sxs-lookup"><span data-stu-id="ef93a-108">Members</span></span>
|<span data-ttu-id="ef93a-109">成员</span><span class="sxs-lookup"><span data-stu-id="ef93a-109">Member</span></span>|<span data-ttu-id="ef93a-110">值</span><span class="sxs-lookup"><span data-stu-id="ef93a-110">Value</span></span>|<span data-ttu-id="ef93a-111">说明</span><span class="sxs-lookup"><span data-stu-id="ef93a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef93a-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="ef93a-112">deviceDefault</span></span>|<span data-ttu-id="ef93a-113">0</span><span class="sxs-lookup"><span data-stu-id="ef93a-113">0</span></span>|<span data-ttu-id="ef93a-114">设备默认行为，通常会提示用户接受系统更新。</span><span class="sxs-lookup"><span data-stu-id="ef93a-114">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="ef93a-115">延迟</span><span class="sxs-lookup"><span data-stu-id="ef93a-115">postpone</span></span>|<span data-ttu-id="ef93a-116">1</span><span class="sxs-lookup"><span data-stu-id="ef93a-116">1</span></span>|<span data-ttu-id="ef93a-117">为 30 天推迟自动安装更新。</span><span class="sxs-lookup"><span data-stu-id="ef93a-117">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="ef93a-118">窗口</span><span class="sxs-lookup"><span data-stu-id="ef93a-118">windowed</span></span>|<span data-ttu-id="ef93a-119">2</span><span class="sxs-lookup"><span data-stu-id="ef93a-119">2</span></span>|<span data-ttu-id="ef93a-120">在日常维护时段内自动安装。</span><span class="sxs-lookup"><span data-stu-id="ef93a-120">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="ef93a-121">automatic</span><span class="sxs-lookup"><span data-stu-id="ef93a-121">automatic</span></span>|<span data-ttu-id="ef93a-122">3</span><span class="sxs-lookup"><span data-stu-id="ef93a-122">3</span></span>|<span data-ttu-id="ef93a-123">自动尽快安装更新。</span><span class="sxs-lookup"><span data-stu-id="ef93a-123">Automatically install updates as soon as possible.</span></span>|





