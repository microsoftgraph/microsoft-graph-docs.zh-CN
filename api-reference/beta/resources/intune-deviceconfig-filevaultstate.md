---
title: fileVaultState 枚举类型
description: FileVault 状态
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1efe284a4d6bad3685c6fbf9c4003153a3aca913
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791763"
---
# <a name="filevaultstate-enum-type"></a><span data-ttu-id="b5d43-103">fileVaultState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b5d43-103">fileVaultState enum type</span></span>

> <span data-ttu-id="b5d43-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b5d43-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5d43-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b5d43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5d43-106">FileVault 状态</span><span class="sxs-lookup"><span data-stu-id="b5d43-106">FileVault State</span></span>

## <a name="members"></a><span data-ttu-id="b5d43-107">成员</span><span class="sxs-lookup"><span data-stu-id="b5d43-107">Members</span></span>
|<span data-ttu-id="b5d43-108">成员</span><span class="sxs-lookup"><span data-stu-id="b5d43-108">Member</span></span>|<span data-ttu-id="b5d43-109">值</span><span class="sxs-lookup"><span data-stu-id="b5d43-109">Value</span></span>|<span data-ttu-id="b5d43-110">说明</span><span class="sxs-lookup"><span data-stu-id="b5d43-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5d43-111">success</span><span class="sxs-lookup"><span data-stu-id="b5d43-111">success</span></span>|<span data-ttu-id="b5d43-112">0</span><span class="sxs-lookup"><span data-stu-id="b5d43-112">0</span></span>|<span data-ttu-id="b5d43-113">FileVault 状态成功</span><span class="sxs-lookup"><span data-stu-id="b5d43-113">FileVault State Success</span></span>|
|<span data-ttu-id="b5d43-114">driveEncryptedByUser</span><span class="sxs-lookup"><span data-stu-id="b5d43-114">driveEncryptedByUser</span></span>|<span data-ttu-id="b5d43-115">1</span><span class="sxs-lookup"><span data-stu-id="b5d43-115">1</span></span>|<span data-ttu-id="b5d43-116">FileVault 已由用户启用，且不受策略管理</span><span class="sxs-lookup"><span data-stu-id="b5d43-116">FileVault has been enabled by user and is not being managed by policy</span></span>|
|<span data-ttu-id="b5d43-117">userDeferredEncryption</span><span class="sxs-lookup"><span data-stu-id="b5d43-117">userDeferredEncryption</span></span>|<span data-ttu-id="b5d43-118">双面</span><span class="sxs-lookup"><span data-stu-id="b5d43-118">2</span></span>|<span data-ttu-id="b5d43-119">FileVault 策略已成功安装，但用户尚未开始加密</span><span class="sxs-lookup"><span data-stu-id="b5d43-119">FileVault policy is successfully installed but user has not started encryption</span></span>|
|<span data-ttu-id="b5d43-120">escrowNotEnabled</span><span class="sxs-lookup"><span data-stu-id="b5d43-120">escrowNotEnabled</span></span>|<span data-ttu-id="b5d43-121">4 </span><span class="sxs-lookup"><span data-stu-id="b5d43-121">4</span></span>|<span data-ttu-id="b5d43-122">FileVault 未启用恢复密钥的保管功能</span><span class="sxs-lookup"><span data-stu-id="b5d43-122">FileVault recovery key escrow is not enabled</span></span>|



