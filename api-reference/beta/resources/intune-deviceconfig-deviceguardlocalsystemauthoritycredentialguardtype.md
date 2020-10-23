---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型
description: Credential Guard 设置的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 481bcb0bfb1380017a2b9261f6896f69e78b40b6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724591"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="fc8c6-103">deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fc8c6-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

<span data-ttu-id="fc8c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc8c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc8c6-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fc8c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc8c6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc8c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc8c6-107">Credential Guard 设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="fc8c6-107">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="fc8c6-108">成员</span><span class="sxs-lookup"><span data-stu-id="fc8c6-108">Members</span></span>
|<span data-ttu-id="fc8c6-109">成员</span><span class="sxs-lookup"><span data-stu-id="fc8c6-109">Member</span></span>|<span data-ttu-id="fc8c6-110">值</span><span class="sxs-lookup"><span data-stu-id="fc8c6-110">Value</span></span>|<span data-ttu-id="fc8c6-111">说明</span><span class="sxs-lookup"><span data-stu-id="fc8c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc8c6-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="fc8c6-112">notConfigured</span></span>|<span data-ttu-id="fc8c6-113">0</span><span class="sxs-lookup"><span data-stu-id="fc8c6-113">0</span></span>|<span data-ttu-id="fc8c6-114">如果之前未进行配置，则远程关闭 Credential Guard （不启用 UEFI 锁定）。</span><span class="sxs-lookup"><span data-stu-id="fc8c6-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="fc8c6-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="fc8c6-115">enableWithUEFILock</span></span>|<span data-ttu-id="fc8c6-116">1</span><span class="sxs-lookup"><span data-stu-id="fc8c6-116">1</span></span>|<span data-ttu-id="fc8c6-117">启用 Credential Guard 和 UEFI 锁定。</span><span class="sxs-lookup"><span data-stu-id="fc8c6-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="fc8c6-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="fc8c6-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="fc8c6-119">双面</span><span class="sxs-lookup"><span data-stu-id="fc8c6-119">2</span></span>|<span data-ttu-id="fc8c6-120">打开不含 UEFI 锁定的 Credential Guard。</span><span class="sxs-lookup"><span data-stu-id="fc8c6-120">Turns on Credential Guard without UEFI lock.</span></span>|
|<span data-ttu-id="fc8c6-121">disable</span><span class="sxs-lookup"><span data-stu-id="fc8c6-121">disable</span></span>|<span data-ttu-id="fc8c6-122">第三章</span><span class="sxs-lookup"><span data-stu-id="fc8c6-122">3</span></span>|<span data-ttu-id="fc8c6-123">禁用 Credential Guard。</span><span class="sxs-lookup"><span data-stu-id="fc8c6-123">Disables Credential Guard.</span></span> <span data-ttu-id="fc8c6-124">这是默认的 OS 值。</span><span class="sxs-lookup"><span data-stu-id="fc8c6-124">This is the default OS value.</span></span>|





