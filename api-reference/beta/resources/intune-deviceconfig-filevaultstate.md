---
title: fileVaultState 枚举类型
description: FileVault 状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4d2e038d5f75f25bb534bfc5923b946d0a0dfd16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994139"
---
# <a name="filevaultstate-enum-type"></a><span data-ttu-id="5ad99-103">fileVaultState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5ad99-103">fileVaultState enum type</span></span>

<span data-ttu-id="5ad99-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ad99-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ad99-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5ad99-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ad99-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5ad99-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ad99-107">FileVault 状态</span><span class="sxs-lookup"><span data-stu-id="5ad99-107">FileVault State</span></span>

## <a name="members"></a><span data-ttu-id="5ad99-108">成员</span><span class="sxs-lookup"><span data-stu-id="5ad99-108">Members</span></span>
|<span data-ttu-id="5ad99-109">成员</span><span class="sxs-lookup"><span data-stu-id="5ad99-109">Member</span></span>|<span data-ttu-id="5ad99-110">值</span><span class="sxs-lookup"><span data-stu-id="5ad99-110">Value</span></span>|<span data-ttu-id="5ad99-111">说明</span><span class="sxs-lookup"><span data-stu-id="5ad99-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ad99-112">success</span><span class="sxs-lookup"><span data-stu-id="5ad99-112">success</span></span>|<span data-ttu-id="5ad99-113">0</span><span class="sxs-lookup"><span data-stu-id="5ad99-113">0</span></span>|<span data-ttu-id="5ad99-114">FileVault 状态成功</span><span class="sxs-lookup"><span data-stu-id="5ad99-114">FileVault State Success</span></span>|
|<span data-ttu-id="5ad99-115">driveEncryptedByUser</span><span class="sxs-lookup"><span data-stu-id="5ad99-115">driveEncryptedByUser</span></span>|<span data-ttu-id="5ad99-116">1 </span><span class="sxs-lookup"><span data-stu-id="5ad99-116">1</span></span>|<span data-ttu-id="5ad99-117">FileVault 已由用户启用，且不受策略管理</span><span class="sxs-lookup"><span data-stu-id="5ad99-117">FileVault has been enabled by user and is not being managed by policy</span></span>|
|<span data-ttu-id="5ad99-118">userDeferredEncryption</span><span class="sxs-lookup"><span data-stu-id="5ad99-118">userDeferredEncryption</span></span>|<span data-ttu-id="5ad99-119">2 </span><span class="sxs-lookup"><span data-stu-id="5ad99-119">2</span></span>|<span data-ttu-id="5ad99-120">FileVault 策略已成功安装，但用户尚未开始加密</span><span class="sxs-lookup"><span data-stu-id="5ad99-120">FileVault policy is successfully installed but user has not started encryption</span></span>|
|<span data-ttu-id="5ad99-121">escrowNotEnabled</span><span class="sxs-lookup"><span data-stu-id="5ad99-121">escrowNotEnabled</span></span>|<span data-ttu-id="5ad99-122">4 </span><span class="sxs-lookup"><span data-stu-id="5ad99-122">4</span></span>|<span data-ttu-id="5ad99-123">FileVault 未启用恢复密钥的保管功能</span><span class="sxs-lookup"><span data-stu-id="5ad99-123">FileVault recovery key escrow is not enabled</span></span>|






