---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型
description: Credential Guard 设置的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 97f04bbf16d93602be466e4dc5fe4986cc26319e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530140"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="6a00e-103">deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6a00e-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

<span data-ttu-id="6a00e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6a00e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a00e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6a00e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a00e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6a00e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a00e-107">Credential Guard 设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="6a00e-107">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="6a00e-108">成员</span><span class="sxs-lookup"><span data-stu-id="6a00e-108">Members</span></span>
|<span data-ttu-id="6a00e-109">成员</span><span class="sxs-lookup"><span data-stu-id="6a00e-109">Member</span></span>|<span data-ttu-id="6a00e-110">值</span><span class="sxs-lookup"><span data-stu-id="6a00e-110">Value</span></span>|<span data-ttu-id="6a00e-111">说明</span><span class="sxs-lookup"><span data-stu-id="6a00e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a00e-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6a00e-112">notConfigured</span></span>|<span data-ttu-id="6a00e-113">0</span><span class="sxs-lookup"><span data-stu-id="6a00e-113">0</span></span>|<span data-ttu-id="6a00e-114">如果之前未进行配置，则远程关闭 Credential Guard （不启用 UEFI 锁定）。</span><span class="sxs-lookup"><span data-stu-id="6a00e-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="6a00e-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="6a00e-115">enableWithUEFILock</span></span>|<span data-ttu-id="6a00e-116">1 </span><span class="sxs-lookup"><span data-stu-id="6a00e-116">1</span></span>|<span data-ttu-id="6a00e-117">启用 Credential Guard 和 UEFI 锁定。</span><span class="sxs-lookup"><span data-stu-id="6a00e-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="6a00e-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="6a00e-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="6a00e-119">2 </span><span class="sxs-lookup"><span data-stu-id="6a00e-119">2</span></span>|<span data-ttu-id="6a00e-120">打开不含 UEFI 锁定的 Credential Guard。</span><span class="sxs-lookup"><span data-stu-id="6a00e-120">Turns on Credential Guard without UEFI lock.</span></span>|



