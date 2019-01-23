---
title: androidDeviceOwnerSystemUpdateInstallType 枚举类型
description: Android 设备所有者的系统更新类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8d7caaa3c79062bba6b8aa06ea11389e1370fba5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419175"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="27ef2-103">androidDeviceOwnerSystemUpdateInstallType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="27ef2-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

> <span data-ttu-id="27ef2-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="27ef2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="27ef2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="27ef2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27ef2-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="27ef2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27ef2-107">Android 设备所有者的系统更新类型。</span><span class="sxs-lookup"><span data-stu-id="27ef2-107">System Update Types for Android Device Owner.</span></span>

## <a name="members"></a><span data-ttu-id="27ef2-108">成员</span><span class="sxs-lookup"><span data-stu-id="27ef2-108">Members</span></span>
|<span data-ttu-id="27ef2-109">成员</span><span class="sxs-lookup"><span data-stu-id="27ef2-109">Member</span></span>|<span data-ttu-id="27ef2-110">值</span><span class="sxs-lookup"><span data-stu-id="27ef2-110">Value</span></span>|<span data-ttu-id="27ef2-111">说明</span><span class="sxs-lookup"><span data-stu-id="27ef2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27ef2-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="27ef2-112">deviceDefault</span></span>|<span data-ttu-id="27ef2-113">0</span><span class="sxs-lookup"><span data-stu-id="27ef2-113">0</span></span>|<span data-ttu-id="27ef2-114">设备默认行为，通常会提示用户接受系统更新。</span><span class="sxs-lookup"><span data-stu-id="27ef2-114">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="27ef2-115">延迟</span><span class="sxs-lookup"><span data-stu-id="27ef2-115">postpone</span></span>|<span data-ttu-id="27ef2-116">1</span><span class="sxs-lookup"><span data-stu-id="27ef2-116">1</span></span>|<span data-ttu-id="27ef2-117">为 30 天推迟自动安装更新。</span><span class="sxs-lookup"><span data-stu-id="27ef2-117">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="27ef2-118">窗口</span><span class="sxs-lookup"><span data-stu-id="27ef2-118">windowed</span></span>|<span data-ttu-id="27ef2-119">2</span><span class="sxs-lookup"><span data-stu-id="27ef2-119">2</span></span>|<span data-ttu-id="27ef2-120">在日常维护时段内自动安装。</span><span class="sxs-lookup"><span data-stu-id="27ef2-120">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="27ef2-121">自动</span><span class="sxs-lookup"><span data-stu-id="27ef2-121">automatic</span></span>|<span data-ttu-id="27ef2-122">3</span><span class="sxs-lookup"><span data-stu-id="27ef2-122">3</span></span>|<span data-ttu-id="27ef2-123">自动尽快安装更新。</span><span class="sxs-lookup"><span data-stu-id="27ef2-123">Automatically install updates as soon as possible.</span></span>|




