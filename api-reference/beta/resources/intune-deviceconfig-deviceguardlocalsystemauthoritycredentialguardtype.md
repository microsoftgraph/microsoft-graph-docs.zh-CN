---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型
description: Credential Guard 设置的可能值。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4d063858501bb8741000234bde8ade8d33550c9f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43359739"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="1f382-103">deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1f382-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

<span data-ttu-id="1f382-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f382-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f382-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1f382-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f382-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1f382-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f382-107">Credential Guard 设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="1f382-107">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="1f382-108">成员</span><span class="sxs-lookup"><span data-stu-id="1f382-108">Members</span></span>
|<span data-ttu-id="1f382-109">成员</span><span class="sxs-lookup"><span data-stu-id="1f382-109">Member</span></span>|<span data-ttu-id="1f382-110">值</span><span class="sxs-lookup"><span data-stu-id="1f382-110">Value</span></span>|<span data-ttu-id="1f382-111">说明</span><span class="sxs-lookup"><span data-stu-id="1f382-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f382-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1f382-112">notConfigured</span></span>|<span data-ttu-id="1f382-113">0</span><span class="sxs-lookup"><span data-stu-id="1f382-113">0</span></span>|<span data-ttu-id="1f382-114">如果之前未进行配置，则远程关闭 Credential Guard （不启用 UEFI 锁定）。</span><span class="sxs-lookup"><span data-stu-id="1f382-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="1f382-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="1f382-115">enableWithUEFILock</span></span>|<span data-ttu-id="1f382-116">1</span><span class="sxs-lookup"><span data-stu-id="1f382-116">1</span></span>|<span data-ttu-id="1f382-117">启用 Credential Guard 和 UEFI 锁定。</span><span class="sxs-lookup"><span data-stu-id="1f382-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="1f382-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="1f382-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="1f382-119">双面</span><span class="sxs-lookup"><span data-stu-id="1f382-119">2</span></span>|<span data-ttu-id="1f382-120">打开不含 UEFI 锁定的 Credential Guard。</span><span class="sxs-lookup"><span data-stu-id="1f382-120">Turns on Credential Guard without UEFI lock.</span></span>|



