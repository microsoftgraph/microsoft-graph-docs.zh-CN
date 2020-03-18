---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型
description: Credential Guard 设置的可能值。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c9532485213c97ac500057842cdcc3e5cbb6719b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42792043"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="51029-103">deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="51029-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="51029-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="51029-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51029-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51029-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51029-106">Credential Guard 设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="51029-106">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="51029-107">成员</span><span class="sxs-lookup"><span data-stu-id="51029-107">Members</span></span>
|<span data-ttu-id="51029-108">成员</span><span class="sxs-lookup"><span data-stu-id="51029-108">Member</span></span>|<span data-ttu-id="51029-109">值</span><span class="sxs-lookup"><span data-stu-id="51029-109">Value</span></span>|<span data-ttu-id="51029-110">说明</span><span class="sxs-lookup"><span data-stu-id="51029-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51029-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="51029-111">notConfigured</span></span>|<span data-ttu-id="51029-112">0</span><span class="sxs-lookup"><span data-stu-id="51029-112">0</span></span>|<span data-ttu-id="51029-113">如果之前未进行配置，则远程关闭 Credential Guard （不启用 UEFI 锁定）。</span><span class="sxs-lookup"><span data-stu-id="51029-113">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="51029-114">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="51029-114">enableWithUEFILock</span></span>|<span data-ttu-id="51029-115">1</span><span class="sxs-lookup"><span data-stu-id="51029-115">1</span></span>|<span data-ttu-id="51029-116">启用 Credential Guard 和 UEFI 锁定。</span><span class="sxs-lookup"><span data-stu-id="51029-116">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="51029-117">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="51029-117">enableWithoutUEFILock</span></span>|<span data-ttu-id="51029-118">双面</span><span class="sxs-lookup"><span data-stu-id="51029-118">2</span></span>|<span data-ttu-id="51029-119">打开不含 UEFI 锁定的 Credential Guard。</span><span class="sxs-lookup"><span data-stu-id="51029-119">Turns on Credential Guard without UEFI lock.</span></span>|



