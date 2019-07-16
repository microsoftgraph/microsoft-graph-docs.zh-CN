---
title: fileVaultState 枚举类型
description: FileVault 状态
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f122d62f85f90825f5fe3129ec2a314d5886e6f2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725931"
---
# <a name="filevaultstate-enum-type"></a><span data-ttu-id="55f82-103">fileVaultState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="55f82-103">fileVaultState enum type</span></span>

> <span data-ttu-id="55f82-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="55f82-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55f82-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="55f82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55f82-106">FileVault 状态</span><span class="sxs-lookup"><span data-stu-id="55f82-106">FileVault State</span></span>

## <a name="members"></a><span data-ttu-id="55f82-107">成员</span><span class="sxs-lookup"><span data-stu-id="55f82-107">Members</span></span>
|<span data-ttu-id="55f82-108">成员</span><span class="sxs-lookup"><span data-stu-id="55f82-108">Member</span></span>|<span data-ttu-id="55f82-109">值</span><span class="sxs-lookup"><span data-stu-id="55f82-109">Value</span></span>|<span data-ttu-id="55f82-110">说明</span><span class="sxs-lookup"><span data-stu-id="55f82-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55f82-111">success</span><span class="sxs-lookup"><span data-stu-id="55f82-111">success</span></span>|<span data-ttu-id="55f82-112">0</span><span class="sxs-lookup"><span data-stu-id="55f82-112">0</span></span>|<span data-ttu-id="55f82-113">FileVault 状态成功</span><span class="sxs-lookup"><span data-stu-id="55f82-113">FileVault State Success</span></span>|
|<span data-ttu-id="55f82-114">driveEncryptedByUser</span><span class="sxs-lookup"><span data-stu-id="55f82-114">driveEncryptedByUser</span></span>|<span data-ttu-id="55f82-115">1</span><span class="sxs-lookup"><span data-stu-id="55f82-115">1</span></span>|<span data-ttu-id="55f82-116">FileVault 已由用户启用, 且不受策略管理</span><span class="sxs-lookup"><span data-stu-id="55f82-116">FileVault has been enabled by user and is not being managed by policy</span></span>|
|<span data-ttu-id="55f82-117">userDeferredEncryption</span><span class="sxs-lookup"><span data-stu-id="55f82-117">userDeferredEncryption</span></span>|<span data-ttu-id="55f82-118">双面</span><span class="sxs-lookup"><span data-stu-id="55f82-118">2</span></span>|<span data-ttu-id="55f82-119">FileVault 策略已成功安装, 但用户尚未开始加密</span><span class="sxs-lookup"><span data-stu-id="55f82-119">FileVault policy is successfully installed but user has not started encryption</span></span>|
|<span data-ttu-id="55f82-120">escrowNotEnabled</span><span class="sxs-lookup"><span data-stu-id="55f82-120">escrowNotEnabled</span></span>|<span data-ttu-id="55f82-121">4</span><span class="sxs-lookup"><span data-stu-id="55f82-121">4</span></span>|<span data-ttu-id="55f82-122">FileVault 未启用恢复密钥的保管功能</span><span class="sxs-lookup"><span data-stu-id="55f82-122">FileVault recovery key escrow is not enabled</span></span>|







