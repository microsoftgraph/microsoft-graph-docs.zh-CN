---
title: androidDeviceOwnerAppAutoUpdatePolicyType 枚举类型
description: Android 设备所有者可能值的状态的设备的应用程序自动更新策略。
localization_priority: Normal
ms.openlocfilehash: 721d08220553bf6acfaac0f84bf0d71725c39ba6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834116"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="e923b-103">androidDeviceOwnerAppAutoUpdatePolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e923b-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="e923b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e923b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e923b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e923b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e923b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e923b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e923b-107">Android 设备所有者可能值的状态的设备的应用程序自动更新策略。</span><span class="sxs-lookup"><span data-stu-id="e923b-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>
## <a name="members"></a><span data-ttu-id="e923b-108">成员</span><span class="sxs-lookup"><span data-stu-id="e923b-108">Members</span></span>
|<span data-ttu-id="e923b-109">成员</span><span class="sxs-lookup"><span data-stu-id="e923b-109">Member</span></span>|<span data-ttu-id="e923b-110">值</span><span class="sxs-lookup"><span data-stu-id="e923b-110">Value</span></span>|<span data-ttu-id="e923b-111">Description</span><span class="sxs-lookup"><span data-stu-id="e923b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e923b-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e923b-112">notConfigured</span></span>|<span data-ttu-id="e923b-113">0</span><span class="sxs-lookup"><span data-stu-id="e923b-113">0</span></span>|<span data-ttu-id="e923b-114">未配置;此值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="e923b-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="e923b-115">userChoice</span><span class="sxs-lookup"><span data-stu-id="e923b-115">userChoice</span></span>|<span data-ttu-id="e923b-116">1</span><span class="sxs-lookup"><span data-stu-id="e923b-116">1</span></span>|<span data-ttu-id="e923b-117">用户可以控制自动更新。</span><span class="sxs-lookup"><span data-stu-id="e923b-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="e923b-118">从不</span><span class="sxs-lookup"><span data-stu-id="e923b-118">never</span></span>|<span data-ttu-id="e923b-119">2</span><span class="sxs-lookup"><span data-stu-id="e923b-119">2</span></span>|<span data-ttu-id="e923b-120">应用程序永远不会自动更新。</span><span class="sxs-lookup"><span data-stu-id="e923b-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="e923b-121">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="e923b-121">wiFiOnly</span></span>|<span data-ttu-id="e923b-122">3</span><span class="sxs-lookup"><span data-stu-id="e923b-122">3</span></span>|<span data-ttu-id="e923b-123">应用程序仅自动更新通过 Wi-fi。</span><span class="sxs-lookup"><span data-stu-id="e923b-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="e923b-124">始终</span><span class="sxs-lookup"><span data-stu-id="e923b-124">always</span></span>|<span data-ttu-id="e923b-125">4</span><span class="sxs-lookup"><span data-stu-id="e923b-125">4</span></span>|<span data-ttu-id="e923b-126">应用程序在任何时候都自动更新。</span><span class="sxs-lookup"><span data-stu-id="e923b-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="e923b-127">可能话费数据。</span><span class="sxs-lookup"><span data-stu-id="e923b-127">Data charges may apply.</span></span>|





