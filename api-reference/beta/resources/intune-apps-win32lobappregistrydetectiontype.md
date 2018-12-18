---
title: win32LobAppRegistryDetectionType 枚举类型
description: 包含所有支持的注册表数据检测类型。
author: tfitzmac
ms.openlocfilehash: d47d13c01d282d73d65f559e016bde5f74248158
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362487"
---
# <a name="win32lobappregistrydetectiontype-enum-type"></a><span data-ttu-id="169f4-103">win32LobAppRegistryDetectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="169f4-103">win32LobAppRegistryDetectionType enum type</span></span>

> <span data-ttu-id="169f4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="169f4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="169f4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="169f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="169f4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="169f4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="169f4-107">包含所有支持的注册表数据检测类型。</span><span class="sxs-lookup"><span data-stu-id="169f4-107">Contains all supported registry data detection type.</span></span>
## <a name="members"></a><span data-ttu-id="169f4-108">成员</span><span class="sxs-lookup"><span data-stu-id="169f4-108">Members</span></span>
|<span data-ttu-id="169f4-109">成员</span><span class="sxs-lookup"><span data-stu-id="169f4-109">Member</span></span>|<span data-ttu-id="169f4-110">值</span><span class="sxs-lookup"><span data-stu-id="169f4-110">Value</span></span>|<span data-ttu-id="169f4-111">说明</span><span class="sxs-lookup"><span data-stu-id="169f4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="169f4-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="169f4-112">notConfigured</span></span>|<span data-ttu-id="169f4-113">0</span><span class="sxs-lookup"><span data-stu-id="169f4-113">0</span></span>|<span data-ttu-id="169f4-114">未配置。</span><span class="sxs-lookup"><span data-stu-id="169f4-114">Not configured.</span></span>|
|<span data-ttu-id="169f4-115">存在</span><span class="sxs-lookup"><span data-stu-id="169f4-115">exists</span></span>|<span data-ttu-id="169f4-116">1</span><span class="sxs-lookup"><span data-stu-id="169f4-116">1</span></span>|<span data-ttu-id="169f4-117">指定的注册表项或值存在。</span><span class="sxs-lookup"><span data-stu-id="169f4-117">The specified registry key or value exists.</span></span>|
|<span data-ttu-id="169f4-118">doesNotExist</span><span class="sxs-lookup"><span data-stu-id="169f4-118">doesNotExist</span></span>|<span data-ttu-id="169f4-119">2</span><span class="sxs-lookup"><span data-stu-id="169f4-119">2</span></span>|<span data-ttu-id="169f4-120">指定的注册表项的值不存在。</span><span class="sxs-lookup"><span data-stu-id="169f4-120">The specified registry key or value does not exist.</span></span>|
|<span data-ttu-id="169f4-121">string</span><span class="sxs-lookup"><span data-stu-id="169f4-121">string</span></span>|<span data-ttu-id="169f4-122">3</span><span class="sxs-lookup"><span data-stu-id="169f4-122">3</span></span>|<span data-ttu-id="169f4-123">字符串值类型。</span><span class="sxs-lookup"><span data-stu-id="169f4-123">String value type.</span></span>|
|<span data-ttu-id="169f4-124">integer</span><span class="sxs-lookup"><span data-stu-id="169f4-124">integer</span></span>|<span data-ttu-id="169f4-125">4</span><span class="sxs-lookup"><span data-stu-id="169f4-125">4</span></span>|<span data-ttu-id="169f4-126">整数值类型。</span><span class="sxs-lookup"><span data-stu-id="169f4-126">Integer value type.</span></span>|
|<span data-ttu-id="169f4-127">version</span><span class="sxs-lookup"><span data-stu-id="169f4-127">version</span></span>|<span data-ttu-id="169f4-128">5</span><span class="sxs-lookup"><span data-stu-id="169f4-128">5</span></span>|<span data-ttu-id="169f4-129">版本值类型。</span><span class="sxs-lookup"><span data-stu-id="169f4-129">Version value type.</span></span>|





