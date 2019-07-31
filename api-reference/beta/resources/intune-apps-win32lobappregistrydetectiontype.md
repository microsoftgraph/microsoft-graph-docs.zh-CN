---
title: win32LobAppRegistryDetectionType 枚举类型
description: 包含所有受支持的注册表数据检测类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 45f961236363f25205763a3d9765453fc8760ad5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012231"
---
# <a name="win32lobappregistrydetectiontype-enum-type"></a><span data-ttu-id="55d03-103">win32LobAppRegistryDetectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="55d03-103">win32LobAppRegistryDetectionType enum type</span></span>

> <span data-ttu-id="55d03-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="55d03-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55d03-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="55d03-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55d03-106">包含所有受支持的注册表数据检测类型。</span><span class="sxs-lookup"><span data-stu-id="55d03-106">Contains all supported registry data detection type.</span></span>

## <a name="members"></a><span data-ttu-id="55d03-107">成员</span><span class="sxs-lookup"><span data-stu-id="55d03-107">Members</span></span>
|<span data-ttu-id="55d03-108">成员</span><span class="sxs-lookup"><span data-stu-id="55d03-108">Member</span></span>|<span data-ttu-id="55d03-109">值</span><span class="sxs-lookup"><span data-stu-id="55d03-109">Value</span></span>|<span data-ttu-id="55d03-110">说明</span><span class="sxs-lookup"><span data-stu-id="55d03-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55d03-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="55d03-111">notConfigured</span></span>|<span data-ttu-id="55d03-112">0</span><span class="sxs-lookup"><span data-stu-id="55d03-112">0</span></span>|<span data-ttu-id="55d03-113">未配置。</span><span class="sxs-lookup"><span data-stu-id="55d03-113">Not configured.</span></span>|
|<span data-ttu-id="55d03-114">存在</span><span class="sxs-lookup"><span data-stu-id="55d03-114">exists</span></span>|<span data-ttu-id="55d03-115">1</span><span class="sxs-lookup"><span data-stu-id="55d03-115">1</span></span>|<span data-ttu-id="55d03-116">指定的注册表项或值存在。</span><span class="sxs-lookup"><span data-stu-id="55d03-116">The specified registry key or value exists.</span></span>|
|<span data-ttu-id="55d03-117">doesNotExist</span><span class="sxs-lookup"><span data-stu-id="55d03-117">doesNotExist</span></span>|<span data-ttu-id="55d03-118">双面</span><span class="sxs-lookup"><span data-stu-id="55d03-118">2</span></span>|<span data-ttu-id="55d03-119">指定的注册表项或值不存在。</span><span class="sxs-lookup"><span data-stu-id="55d03-119">The specified registry key or value does not exist.</span></span>|
|<span data-ttu-id="55d03-120">string</span><span class="sxs-lookup"><span data-stu-id="55d03-120">string</span></span>|<span data-ttu-id="55d03-121">第三章</span><span class="sxs-lookup"><span data-stu-id="55d03-121">3</span></span>|<span data-ttu-id="55d03-122">字符串值类型。</span><span class="sxs-lookup"><span data-stu-id="55d03-122">String value type.</span></span>|
|<span data-ttu-id="55d03-123">integer</span><span class="sxs-lookup"><span data-stu-id="55d03-123">integer</span></span>|<span data-ttu-id="55d03-124">4</span><span class="sxs-lookup"><span data-stu-id="55d03-124">4</span></span>|<span data-ttu-id="55d03-125">整型值类型。</span><span class="sxs-lookup"><span data-stu-id="55d03-125">Integer value type.</span></span>|
|<span data-ttu-id="55d03-126">version</span><span class="sxs-lookup"><span data-stu-id="55d03-126">version</span></span>|<span data-ttu-id="55d03-127">5</span><span class="sxs-lookup"><span data-stu-id="55d03-127">5</span></span>|<span data-ttu-id="55d03-128">版本值类型。</span><span class="sxs-lookup"><span data-stu-id="55d03-128">Version value type.</span></span>|





