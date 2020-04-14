---
title: fileVaultState 枚举类型
description: FileVault 状态
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2d7f69413ac7fd4be1e857951b2a70aac0fe7bc3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444314"
---
# <a name="filevaultstate-enum-type"></a><span data-ttu-id="11112-103">fileVaultState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="11112-103">fileVaultState enum type</span></span>

<span data-ttu-id="11112-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11112-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11112-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="11112-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11112-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="11112-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11112-107">FileVault 状态</span><span class="sxs-lookup"><span data-stu-id="11112-107">FileVault State</span></span>

## <a name="members"></a><span data-ttu-id="11112-108">成员</span><span class="sxs-lookup"><span data-stu-id="11112-108">Members</span></span>
|<span data-ttu-id="11112-109">成员</span><span class="sxs-lookup"><span data-stu-id="11112-109">Member</span></span>|<span data-ttu-id="11112-110">值</span><span class="sxs-lookup"><span data-stu-id="11112-110">Value</span></span>|<span data-ttu-id="11112-111">说明</span><span class="sxs-lookup"><span data-stu-id="11112-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11112-112">success</span><span class="sxs-lookup"><span data-stu-id="11112-112">success</span></span>|<span data-ttu-id="11112-113">0</span><span class="sxs-lookup"><span data-stu-id="11112-113">0</span></span>|<span data-ttu-id="11112-114">FileVault 状态成功</span><span class="sxs-lookup"><span data-stu-id="11112-114">FileVault State Success</span></span>|
|<span data-ttu-id="11112-115">driveEncryptedByUser</span><span class="sxs-lookup"><span data-stu-id="11112-115">driveEncryptedByUser</span></span>|<span data-ttu-id="11112-116">1</span><span class="sxs-lookup"><span data-stu-id="11112-116">1</span></span>|<span data-ttu-id="11112-117">FileVault 已由用户启用，且不受策略管理</span><span class="sxs-lookup"><span data-stu-id="11112-117">FileVault has been enabled by user and is not being managed by policy</span></span>|
|<span data-ttu-id="11112-118">userDeferredEncryption</span><span class="sxs-lookup"><span data-stu-id="11112-118">userDeferredEncryption</span></span>|<span data-ttu-id="11112-119">双面</span><span class="sxs-lookup"><span data-stu-id="11112-119">2</span></span>|<span data-ttu-id="11112-120">FileVault 策略已成功安装，但用户尚未开始加密</span><span class="sxs-lookup"><span data-stu-id="11112-120">FileVault policy is successfully installed but user has not started encryption</span></span>|
|<span data-ttu-id="11112-121">escrowNotEnabled</span><span class="sxs-lookup"><span data-stu-id="11112-121">escrowNotEnabled</span></span>|<span data-ttu-id="11112-122">4 </span><span class="sxs-lookup"><span data-stu-id="11112-122">4</span></span>|<span data-ttu-id="11112-123">FileVault 未启用恢复密钥的保管功能</span><span class="sxs-lookup"><span data-stu-id="11112-123">FileVault recovery key escrow is not enabled</span></span>|



