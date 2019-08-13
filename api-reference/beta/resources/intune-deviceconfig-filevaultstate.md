---
title: fileVaultState 枚举类型
description: FileVault 状态
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 54e8076dc4b4f6ab20f7790d2a650de6c07aa702
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325566"
---
# <a name="filevaultstate-enum-type"></a><span data-ttu-id="842bd-103">fileVaultState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="842bd-103">fileVaultState enum type</span></span>

> <span data-ttu-id="842bd-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="842bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="842bd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="842bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="842bd-106">FileVault 状态</span><span class="sxs-lookup"><span data-stu-id="842bd-106">FileVault State</span></span>

## <a name="members"></a><span data-ttu-id="842bd-107">成员</span><span class="sxs-lookup"><span data-stu-id="842bd-107">Members</span></span>
|<span data-ttu-id="842bd-108">成员</span><span class="sxs-lookup"><span data-stu-id="842bd-108">Member</span></span>|<span data-ttu-id="842bd-109">值</span><span class="sxs-lookup"><span data-stu-id="842bd-109">Value</span></span>|<span data-ttu-id="842bd-110">说明</span><span class="sxs-lookup"><span data-stu-id="842bd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="842bd-111">success</span><span class="sxs-lookup"><span data-stu-id="842bd-111">success</span></span>|<span data-ttu-id="842bd-112">0</span><span class="sxs-lookup"><span data-stu-id="842bd-112">0</span></span>|<span data-ttu-id="842bd-113">FileVault 状态成功</span><span class="sxs-lookup"><span data-stu-id="842bd-113">FileVault State Success</span></span>|
|<span data-ttu-id="842bd-114">driveEncryptedByUser</span><span class="sxs-lookup"><span data-stu-id="842bd-114">driveEncryptedByUser</span></span>|<span data-ttu-id="842bd-115">1</span><span class="sxs-lookup"><span data-stu-id="842bd-115">1</span></span>|<span data-ttu-id="842bd-116">FileVault 已由用户启用, 且不受策略管理</span><span class="sxs-lookup"><span data-stu-id="842bd-116">FileVault has been enabled by user and is not being managed by policy</span></span>|
|<span data-ttu-id="842bd-117">userDeferredEncryption</span><span class="sxs-lookup"><span data-stu-id="842bd-117">userDeferredEncryption</span></span>|<span data-ttu-id="842bd-118">双面</span><span class="sxs-lookup"><span data-stu-id="842bd-118">2</span></span>|<span data-ttu-id="842bd-119">FileVault 策略已成功安装, 但用户尚未开始加密</span><span class="sxs-lookup"><span data-stu-id="842bd-119">FileVault policy is successfully installed but user has not started encryption</span></span>|
|<span data-ttu-id="842bd-120">escrowNotEnabled</span><span class="sxs-lookup"><span data-stu-id="842bd-120">escrowNotEnabled</span></span>|<span data-ttu-id="842bd-121">4</span><span class="sxs-lookup"><span data-stu-id="842bd-121">4</span></span>|<span data-ttu-id="842bd-122">FileVault 未启用恢复密钥的保管功能</span><span class="sxs-lookup"><span data-stu-id="842bd-122">FileVault recovery key escrow is not enabled</span></span>|



