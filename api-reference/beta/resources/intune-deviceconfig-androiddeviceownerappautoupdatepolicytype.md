---
title: androidDeviceOwnerAppAutoUpdatePolicyType 枚举类型
description: Android 设备所有者可能值的状态的设备的应用程序自动更新策略。
ms.openlocfilehash: 0287a26b4974bc0b376341ca91791d1fa768a9e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041481"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="45522-103">androidDeviceOwnerAppAutoUpdatePolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="45522-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="45522-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="45522-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45522-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="45522-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45522-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="45522-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45522-107">Android 设备所有者可能值的状态的设备的应用程序自动更新策略。</span><span class="sxs-lookup"><span data-stu-id="45522-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>
## <a name="members"></a><span data-ttu-id="45522-108">成员</span><span class="sxs-lookup"><span data-stu-id="45522-108">Members</span></span>
|<span data-ttu-id="45522-109">成员</span><span class="sxs-lookup"><span data-stu-id="45522-109">Member</span></span>|<span data-ttu-id="45522-110">值</span><span class="sxs-lookup"><span data-stu-id="45522-110">Value</span></span>|<span data-ttu-id="45522-111">说明</span><span class="sxs-lookup"><span data-stu-id="45522-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45522-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="45522-112">notConfigured</span></span>|<span data-ttu-id="45522-113">0</span><span class="sxs-lookup"><span data-stu-id="45522-113">0</span></span>|<span data-ttu-id="45522-114">未配置;此值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="45522-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="45522-115">userChoice</span><span class="sxs-lookup"><span data-stu-id="45522-115">userChoice</span></span>|<span data-ttu-id="45522-116">1</span><span class="sxs-lookup"><span data-stu-id="45522-116">1</span></span>|<span data-ttu-id="45522-117">用户可以控制自动更新。</span><span class="sxs-lookup"><span data-stu-id="45522-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="45522-118">从不</span><span class="sxs-lookup"><span data-stu-id="45522-118">never</span></span>|<span data-ttu-id="45522-119">2</span><span class="sxs-lookup"><span data-stu-id="45522-119">2</span></span>|<span data-ttu-id="45522-120">应用程序永远不会自动更新。</span><span class="sxs-lookup"><span data-stu-id="45522-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="45522-121">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="45522-121">wiFiOnly</span></span>|<span data-ttu-id="45522-122">3</span><span class="sxs-lookup"><span data-stu-id="45522-122">3</span></span>|<span data-ttu-id="45522-123">应用程序仅自动更新通过 Wi-fi。</span><span class="sxs-lookup"><span data-stu-id="45522-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="45522-124">始终</span><span class="sxs-lookup"><span data-stu-id="45522-124">always</span></span>|<span data-ttu-id="45522-125">4</span><span class="sxs-lookup"><span data-stu-id="45522-125">4</span></span>|<span data-ttu-id="45522-126">应用程序在任何时候都自动更新。</span><span class="sxs-lookup"><span data-stu-id="45522-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="45522-127">可能话费数据。</span><span class="sxs-lookup"><span data-stu-id="45522-127">Data charges may apply.</span></span>|





