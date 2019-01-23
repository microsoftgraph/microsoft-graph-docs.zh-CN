---
title: androidDeviceOwnerAppAutoUpdatePolicyType 枚举类型
description: Android 设备所有者可能值的状态的设备的应用程序自动更新策略。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 68dec6bb21cf27a7b5b54f9fc8a839fba3dc6f00
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419070"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="4a9ff-103">androidDeviceOwnerAppAutoUpdatePolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4a9ff-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="4a9ff-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="4a9ff-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4a9ff-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4a9ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a9ff-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4a9ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a9ff-107">Android 设备所有者可能值的状态的设备的应用程序自动更新策略。</span><span class="sxs-lookup"><span data-stu-id="4a9ff-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="4a9ff-108">成员</span><span class="sxs-lookup"><span data-stu-id="4a9ff-108">Members</span></span>
|<span data-ttu-id="4a9ff-109">成员</span><span class="sxs-lookup"><span data-stu-id="4a9ff-109">Member</span></span>|<span data-ttu-id="4a9ff-110">值</span><span class="sxs-lookup"><span data-stu-id="4a9ff-110">Value</span></span>|<span data-ttu-id="4a9ff-111">说明</span><span class="sxs-lookup"><span data-stu-id="4a9ff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a9ff-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4a9ff-112">notConfigured</span></span>|<span data-ttu-id="4a9ff-113">0</span><span class="sxs-lookup"><span data-stu-id="4a9ff-113">0</span></span>|<span data-ttu-id="4a9ff-114">未配置;此值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="4a9ff-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="4a9ff-115">userChoice</span><span class="sxs-lookup"><span data-stu-id="4a9ff-115">userChoice</span></span>|<span data-ttu-id="4a9ff-116">1</span><span class="sxs-lookup"><span data-stu-id="4a9ff-116">1</span></span>|<span data-ttu-id="4a9ff-117">用户可以控制自动更新。</span><span class="sxs-lookup"><span data-stu-id="4a9ff-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="4a9ff-118">从不</span><span class="sxs-lookup"><span data-stu-id="4a9ff-118">never</span></span>|<span data-ttu-id="4a9ff-119">2</span><span class="sxs-lookup"><span data-stu-id="4a9ff-119">2</span></span>|<span data-ttu-id="4a9ff-120">应用程序永远不会自动更新。</span><span class="sxs-lookup"><span data-stu-id="4a9ff-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="4a9ff-121">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="4a9ff-121">wiFiOnly</span></span>|<span data-ttu-id="4a9ff-122">3</span><span class="sxs-lookup"><span data-stu-id="4a9ff-122">3</span></span>|<span data-ttu-id="4a9ff-123">应用程序仅自动更新通过 Wi-fi。</span><span class="sxs-lookup"><span data-stu-id="4a9ff-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="4a9ff-124">始终</span><span class="sxs-lookup"><span data-stu-id="4a9ff-124">always</span></span>|<span data-ttu-id="4a9ff-125">4</span><span class="sxs-lookup"><span data-stu-id="4a9ff-125">4</span></span>|<span data-ttu-id="4a9ff-126">应用程序在任何时候都自动更新。</span><span class="sxs-lookup"><span data-stu-id="4a9ff-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="4a9ff-127">可能话费数据。</span><span class="sxs-lookup"><span data-stu-id="4a9ff-127">Data charges may apply.</span></span>|




