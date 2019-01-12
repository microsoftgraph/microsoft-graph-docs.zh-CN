---
title: androidDeviceOwnerAppAutoUpdatePolicyType 枚举类型
description: Android 设备所有者可能值的状态的设备的应用程序自动更新策略。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: f784e951df2a9d1ee56825649da3899b0792c3a6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973606"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="2aa35-103">androidDeviceOwnerAppAutoUpdatePolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2aa35-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="2aa35-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2aa35-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2aa35-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2aa35-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2aa35-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2aa35-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2aa35-107">Android 设备所有者可能值的状态的设备的应用程序自动更新策略。</span><span class="sxs-lookup"><span data-stu-id="2aa35-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>
## <a name="members"></a><span data-ttu-id="2aa35-108">成员</span><span class="sxs-lookup"><span data-stu-id="2aa35-108">Members</span></span>
|<span data-ttu-id="2aa35-109">成员</span><span class="sxs-lookup"><span data-stu-id="2aa35-109">Member</span></span>|<span data-ttu-id="2aa35-110">值</span><span class="sxs-lookup"><span data-stu-id="2aa35-110">Value</span></span>|<span data-ttu-id="2aa35-111">说明</span><span class="sxs-lookup"><span data-stu-id="2aa35-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2aa35-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="2aa35-112">notConfigured</span></span>|<span data-ttu-id="2aa35-113">0</span><span class="sxs-lookup"><span data-stu-id="2aa35-113">0</span></span>|<span data-ttu-id="2aa35-114">未配置;此值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="2aa35-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="2aa35-115">userChoice</span><span class="sxs-lookup"><span data-stu-id="2aa35-115">userChoice</span></span>|<span data-ttu-id="2aa35-116">1</span><span class="sxs-lookup"><span data-stu-id="2aa35-116">1</span></span>|<span data-ttu-id="2aa35-117">用户可以控制自动更新。</span><span class="sxs-lookup"><span data-stu-id="2aa35-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="2aa35-118">从不</span><span class="sxs-lookup"><span data-stu-id="2aa35-118">never</span></span>|<span data-ttu-id="2aa35-119">2</span><span class="sxs-lookup"><span data-stu-id="2aa35-119">2</span></span>|<span data-ttu-id="2aa35-120">应用程序永远不会自动更新。</span><span class="sxs-lookup"><span data-stu-id="2aa35-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="2aa35-121">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="2aa35-121">wiFiOnly</span></span>|<span data-ttu-id="2aa35-122">3</span><span class="sxs-lookup"><span data-stu-id="2aa35-122">3</span></span>|<span data-ttu-id="2aa35-123">应用程序仅自动更新通过 Wi-fi。</span><span class="sxs-lookup"><span data-stu-id="2aa35-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="2aa35-124">始终</span><span class="sxs-lookup"><span data-stu-id="2aa35-124">always</span></span>|<span data-ttu-id="2aa35-125">4</span><span class="sxs-lookup"><span data-stu-id="2aa35-125">4</span></span>|<span data-ttu-id="2aa35-126">应用程序在任何时候都自动更新。</span><span class="sxs-lookup"><span data-stu-id="2aa35-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="2aa35-127">可能话费数据。</span><span class="sxs-lookup"><span data-stu-id="2aa35-127">Data charges may apply.</span></span>|





