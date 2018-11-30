---
title: win32LobAppRegistryDetectionType 枚举类型
description: 包含所有支持的注册表数据检测类型。
ms.openlocfilehash: cd0fc2f2941ae6cbab19222a414c5f52fe2a726c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042502"
---
# <a name="win32lobappregistrydetectiontype-enum-type"></a><span data-ttu-id="3b402-103">win32LobAppRegistryDetectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3b402-103">win32LobAppRegistryDetectionType enum type</span></span>

> <span data-ttu-id="3b402-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3b402-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b402-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3b402-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b402-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3b402-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b402-107">包含所有支持的注册表数据检测类型。</span><span class="sxs-lookup"><span data-stu-id="3b402-107">Contains all supported registry data detection type.</span></span>
## <a name="members"></a><span data-ttu-id="3b402-108">成员</span><span class="sxs-lookup"><span data-stu-id="3b402-108">Members</span></span>
|<span data-ttu-id="3b402-109">成员</span><span class="sxs-lookup"><span data-stu-id="3b402-109">Member</span></span>|<span data-ttu-id="3b402-110">值</span><span class="sxs-lookup"><span data-stu-id="3b402-110">Value</span></span>|<span data-ttu-id="3b402-111">说明</span><span class="sxs-lookup"><span data-stu-id="3b402-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b402-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="3b402-112">notConfigured</span></span>|<span data-ttu-id="3b402-113">0</span><span class="sxs-lookup"><span data-stu-id="3b402-113">0</span></span>|<span data-ttu-id="3b402-114">未配置。</span><span class="sxs-lookup"><span data-stu-id="3b402-114">Not configured.</span></span>|
|<span data-ttu-id="3b402-115">存在</span><span class="sxs-lookup"><span data-stu-id="3b402-115">exists</span></span>|<span data-ttu-id="3b402-116">1</span><span class="sxs-lookup"><span data-stu-id="3b402-116">1</span></span>|<span data-ttu-id="3b402-117">指定的注册表项或值存在。</span><span class="sxs-lookup"><span data-stu-id="3b402-117">The specified registry key or value exists.</span></span>|
|<span data-ttu-id="3b402-118">doesNotExist</span><span class="sxs-lookup"><span data-stu-id="3b402-118">doesNotExist</span></span>|<span data-ttu-id="3b402-119">2</span><span class="sxs-lookup"><span data-stu-id="3b402-119">2</span></span>|<span data-ttu-id="3b402-120">指定的注册表项的值不存在。</span><span class="sxs-lookup"><span data-stu-id="3b402-120">The specified registry key or value does not exist.</span></span>|
|<span data-ttu-id="3b402-121">string</span><span class="sxs-lookup"><span data-stu-id="3b402-121">string</span></span>|<span data-ttu-id="3b402-122">3</span><span class="sxs-lookup"><span data-stu-id="3b402-122">3</span></span>|<span data-ttu-id="3b402-123">字符串值类型。</span><span class="sxs-lookup"><span data-stu-id="3b402-123">String value type.</span></span>|
|<span data-ttu-id="3b402-124">integer</span><span class="sxs-lookup"><span data-stu-id="3b402-124">integer</span></span>|<span data-ttu-id="3b402-125">4</span><span class="sxs-lookup"><span data-stu-id="3b402-125">4</span></span>|<span data-ttu-id="3b402-126">整数值类型。</span><span class="sxs-lookup"><span data-stu-id="3b402-126">Integer value type.</span></span>|
|<span data-ttu-id="3b402-127">version</span><span class="sxs-lookup"><span data-stu-id="3b402-127">version</span></span>|<span data-ttu-id="3b402-128">5</span><span class="sxs-lookup"><span data-stu-id="3b402-128">5</span></span>|<span data-ttu-id="3b402-129">版本值类型。</span><span class="sxs-lookup"><span data-stu-id="3b402-129">Version value type.</span></span>|





