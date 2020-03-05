---
title: fileVaultState 枚举类型
description: FileVault 状态
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8f2fa72d2db91ba000209332aec3d59579cba822
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530000"
---
# <a name="filevaultstate-enum-type"></a><span data-ttu-id="2a083-103">fileVaultState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2a083-103">fileVaultState enum type</span></span>

<span data-ttu-id="2a083-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2a083-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a083-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2a083-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a083-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2a083-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a083-107">FileVault 状态</span><span class="sxs-lookup"><span data-stu-id="2a083-107">FileVault State</span></span>

## <a name="members"></a><span data-ttu-id="2a083-108">成员</span><span class="sxs-lookup"><span data-stu-id="2a083-108">Members</span></span>
|<span data-ttu-id="2a083-109">成员</span><span class="sxs-lookup"><span data-stu-id="2a083-109">Member</span></span>|<span data-ttu-id="2a083-110">值</span><span class="sxs-lookup"><span data-stu-id="2a083-110">Value</span></span>|<span data-ttu-id="2a083-111">说明</span><span class="sxs-lookup"><span data-stu-id="2a083-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a083-112">success</span><span class="sxs-lookup"><span data-stu-id="2a083-112">success</span></span>|<span data-ttu-id="2a083-113">0</span><span class="sxs-lookup"><span data-stu-id="2a083-113">0</span></span>|<span data-ttu-id="2a083-114">FileVault 状态成功</span><span class="sxs-lookup"><span data-stu-id="2a083-114">FileVault State Success</span></span>|
|<span data-ttu-id="2a083-115">driveEncryptedByUser</span><span class="sxs-lookup"><span data-stu-id="2a083-115">driveEncryptedByUser</span></span>|<span data-ttu-id="2a083-116">1 </span><span class="sxs-lookup"><span data-stu-id="2a083-116">1</span></span>|<span data-ttu-id="2a083-117">FileVault 已由用户启用，且不受策略管理</span><span class="sxs-lookup"><span data-stu-id="2a083-117">FileVault has been enabled by user and is not being managed by policy</span></span>|
|<span data-ttu-id="2a083-118">userDeferredEncryption</span><span class="sxs-lookup"><span data-stu-id="2a083-118">userDeferredEncryption</span></span>|<span data-ttu-id="2a083-119">2 </span><span class="sxs-lookup"><span data-stu-id="2a083-119">2</span></span>|<span data-ttu-id="2a083-120">FileVault 策略已成功安装，但用户尚未开始加密</span><span class="sxs-lookup"><span data-stu-id="2a083-120">FileVault policy is successfully installed but user has not started encryption</span></span>|
|<span data-ttu-id="2a083-121">escrowNotEnabled</span><span class="sxs-lookup"><span data-stu-id="2a083-121">escrowNotEnabled</span></span>|<span data-ttu-id="2a083-122">4 </span><span class="sxs-lookup"><span data-stu-id="2a083-122">4</span></span>|<span data-ttu-id="2a083-123">FileVault 未启用恢复密钥的保管功能</span><span class="sxs-lookup"><span data-stu-id="2a083-123">FileVault recovery key escrow is not enabled</span></span>|



