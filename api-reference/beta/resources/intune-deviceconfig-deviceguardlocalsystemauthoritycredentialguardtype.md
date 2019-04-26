---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型
description: Credential Guard 设置的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f22336a37c3d10d4e86b3db2af41e8103dcfe33
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567226"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="72210-103">deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="72210-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="72210-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="72210-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72210-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="72210-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72210-106">Credential Guard 设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="72210-106">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="72210-107">成员</span><span class="sxs-lookup"><span data-stu-id="72210-107">Members</span></span>
|<span data-ttu-id="72210-108">成员</span><span class="sxs-lookup"><span data-stu-id="72210-108">Member</span></span>|<span data-ttu-id="72210-109">值</span><span class="sxs-lookup"><span data-stu-id="72210-109">Value</span></span>|<span data-ttu-id="72210-110">说明</span><span class="sxs-lookup"><span data-stu-id="72210-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72210-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="72210-111">notConfigured</span></span>|<span data-ttu-id="72210-112">0</span><span class="sxs-lookup"><span data-stu-id="72210-112">0</span></span>|<span data-ttu-id="72210-113">如果之前未进行配置, 则远程关闭 Credential Guard (不启用 UEFI 锁定)。</span><span class="sxs-lookup"><span data-stu-id="72210-113">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="72210-114">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="72210-114">enableWithUEFILock</span></span>|<span data-ttu-id="72210-115">1</span><span class="sxs-lookup"><span data-stu-id="72210-115">1</span></span>|<span data-ttu-id="72210-116">启用 Credential Guard 和 UEFI 锁定。</span><span class="sxs-lookup"><span data-stu-id="72210-116">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="72210-117">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="72210-117">enableWithoutUEFILock</span></span>|<span data-ttu-id="72210-118">2 </span><span class="sxs-lookup"><span data-stu-id="72210-118">2</span></span>|<span data-ttu-id="72210-119">打开不含 UEFI 锁定的 Credential Guard。</span><span class="sxs-lookup"><span data-stu-id="72210-119">Turns on Credential Guard without UEFI lock.</span></span>|





