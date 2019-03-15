---
title: 启用的枚举类型
description: 介绍支持多个工作流的适用于 Intune 的 Microsoft Graph API 的支持枚举。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e781e1c58427ea166f77f3c250e572cbd3520210
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571233"
---
# <a name="enablement-enum-type"></a><span data-ttu-id="1dfbe-103">启用的枚举类型</span><span class="sxs-lookup"><span data-stu-id="1dfbe-103">enablement enum type</span></span>

> <span data-ttu-id="1dfbe-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1dfbe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1dfbe-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1dfbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dfbe-106">属性的可能值</span><span class="sxs-lookup"><span data-stu-id="1dfbe-106">Possible values of a property</span></span>

## <a name="members"></a><span data-ttu-id="1dfbe-107">成员</span><span class="sxs-lookup"><span data-stu-id="1dfbe-107">Members</span></span>
|<span data-ttu-id="1dfbe-108">成员</span><span class="sxs-lookup"><span data-stu-id="1dfbe-108">Member</span></span>|<span data-ttu-id="1dfbe-109">值</span><span class="sxs-lookup"><span data-stu-id="1dfbe-109">Value</span></span>|<span data-ttu-id="1dfbe-110">说明</span><span class="sxs-lookup"><span data-stu-id="1dfbe-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dfbe-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1dfbe-111">notConfigured</span></span>|<span data-ttu-id="1dfbe-112">0</span><span class="sxs-lookup"><span data-stu-id="1dfbe-112">0</span></span>|<span data-ttu-id="1dfbe-113">设备默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="1dfbe-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="1dfbe-114">enabled</span><span class="sxs-lookup"><span data-stu-id="1dfbe-114">enabled</span></span>|<span data-ttu-id="1dfbe-115">1</span><span class="sxs-lookup"><span data-stu-id="1dfbe-115">1</span></span>|<span data-ttu-id="1dfbe-116">启用设备上的设置。</span><span class="sxs-lookup"><span data-stu-id="1dfbe-116">Enables the setting on the device.</span></span>|
|<span data-ttu-id="1dfbe-117">禁用</span><span class="sxs-lookup"><span data-stu-id="1dfbe-117">disabled</span></span>|<span data-ttu-id="1dfbe-118">双面</span><span class="sxs-lookup"><span data-stu-id="1dfbe-118">2</span></span>|<span data-ttu-id="1dfbe-119">禁用设备上的设置。</span><span class="sxs-lookup"><span data-stu-id="1dfbe-119">Disables the setting on the device.</span></span>|
