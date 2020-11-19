---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型
description: Credential Guard 设置的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8467f60fba373265695a44533a25461e8d890824
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49216127"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="f7d82-103">deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f7d82-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

<span data-ttu-id="f7d82-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7d82-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7d82-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f7d82-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7d82-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7d82-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7d82-107">Credential Guard 设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="f7d82-107">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="f7d82-108">成员</span><span class="sxs-lookup"><span data-stu-id="f7d82-108">Members</span></span>
|<span data-ttu-id="f7d82-109">成员</span><span class="sxs-lookup"><span data-stu-id="f7d82-109">Member</span></span>|<span data-ttu-id="f7d82-110">值</span><span class="sxs-lookup"><span data-stu-id="f7d82-110">Value</span></span>|<span data-ttu-id="f7d82-111">说明</span><span class="sxs-lookup"><span data-stu-id="f7d82-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7d82-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f7d82-112">notConfigured</span></span>|<span data-ttu-id="f7d82-113">0</span><span class="sxs-lookup"><span data-stu-id="f7d82-113">0</span></span>|<span data-ttu-id="f7d82-114">如果之前未进行配置，则远程关闭 Credential Guard （不启用 UEFI 锁定）。</span><span class="sxs-lookup"><span data-stu-id="f7d82-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="f7d82-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="f7d82-115">enableWithUEFILock</span></span>|<span data-ttu-id="f7d82-116">1</span><span class="sxs-lookup"><span data-stu-id="f7d82-116">1</span></span>|<span data-ttu-id="f7d82-117">启用 Credential Guard 和 UEFI 锁定。</span><span class="sxs-lookup"><span data-stu-id="f7d82-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="f7d82-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="f7d82-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="f7d82-119">双面</span><span class="sxs-lookup"><span data-stu-id="f7d82-119">2</span></span>|<span data-ttu-id="f7d82-120">打开不含 UEFI 锁定的 Credential Guard。</span><span class="sxs-lookup"><span data-stu-id="f7d82-120">Turns on Credential Guard without UEFI lock.</span></span>|
|<span data-ttu-id="f7d82-121">disable</span><span class="sxs-lookup"><span data-stu-id="f7d82-121">disable</span></span>|<span data-ttu-id="f7d82-122">第三章</span><span class="sxs-lookup"><span data-stu-id="f7d82-122">3</span></span>|<span data-ttu-id="f7d82-123">禁用 Credential Guard。</span><span class="sxs-lookup"><span data-stu-id="f7d82-123">Disables Credential Guard.</span></span> <span data-ttu-id="f7d82-124">这是默认的 OS 值。</span><span class="sxs-lookup"><span data-stu-id="f7d82-124">This is the default OS value.</span></span>|




