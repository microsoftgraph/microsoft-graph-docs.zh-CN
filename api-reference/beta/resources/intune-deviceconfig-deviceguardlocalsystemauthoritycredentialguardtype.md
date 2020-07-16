---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型
description: Credential Guard 设置的可能值。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4b02402ff6c6c0373396bd6fca0cad6ded5cb36d
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123769"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="a2ea3-103">deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a2ea3-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

<span data-ttu-id="a2ea3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2ea3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2ea3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a2ea3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2ea3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a2ea3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2ea3-107">Credential Guard 设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="a2ea3-107">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="a2ea3-108">成员</span><span class="sxs-lookup"><span data-stu-id="a2ea3-108">Members</span></span>
|<span data-ttu-id="a2ea3-109">成员</span><span class="sxs-lookup"><span data-stu-id="a2ea3-109">Member</span></span>|<span data-ttu-id="a2ea3-110">值</span><span class="sxs-lookup"><span data-stu-id="a2ea3-110">Value</span></span>|<span data-ttu-id="a2ea3-111">说明</span><span class="sxs-lookup"><span data-stu-id="a2ea3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2ea3-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a2ea3-112">notConfigured</span></span>|<span data-ttu-id="a2ea3-113">0</span><span class="sxs-lookup"><span data-stu-id="a2ea3-113">0</span></span>|<span data-ttu-id="a2ea3-114">如果之前未进行配置，则远程关闭 Credential Guard （不启用 UEFI 锁定）。</span><span class="sxs-lookup"><span data-stu-id="a2ea3-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="a2ea3-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="a2ea3-115">enableWithUEFILock</span></span>|<span data-ttu-id="a2ea3-116">1 </span><span class="sxs-lookup"><span data-stu-id="a2ea3-116">1</span></span>|<span data-ttu-id="a2ea3-117">启用 Credential Guard 和 UEFI 锁定。</span><span class="sxs-lookup"><span data-stu-id="a2ea3-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="a2ea3-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="a2ea3-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="a2ea3-119">2 </span><span class="sxs-lookup"><span data-stu-id="a2ea3-119">2</span></span>|<span data-ttu-id="a2ea3-120">打开不含 UEFI 锁定的 Credential Guard。</span><span class="sxs-lookup"><span data-stu-id="a2ea3-120">Turns on Credential Guard without UEFI lock.</span></span>|
|<span data-ttu-id="a2ea3-121">disable</span><span class="sxs-lookup"><span data-stu-id="a2ea3-121">disable</span></span>|<span data-ttu-id="a2ea3-122">3 </span><span class="sxs-lookup"><span data-stu-id="a2ea3-122">3</span></span>|<span data-ttu-id="a2ea3-123">禁用 Credential Guard。</span><span class="sxs-lookup"><span data-stu-id="a2ea3-123">Disables Credential Guard.</span></span> <span data-ttu-id="a2ea3-124">这是默认的 OS 值。</span><span class="sxs-lookup"><span data-stu-id="a2ea3-124">This is the default OS value.</span></span>|



