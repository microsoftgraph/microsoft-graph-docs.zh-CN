---
title: fileVaultState 枚举类型
description: FileVault 状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a9aa7c0b11a155597911f64882f5b6d424a2b129
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294520"
---
# <a name="filevaultstate-enum-type"></a><span data-ttu-id="ca47a-103">fileVaultState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ca47a-103">fileVaultState enum type</span></span>

<span data-ttu-id="ca47a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca47a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca47a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ca47a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca47a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca47a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca47a-107">FileVault 状态</span><span class="sxs-lookup"><span data-stu-id="ca47a-107">FileVault State</span></span>

## <a name="members"></a><span data-ttu-id="ca47a-108">成员</span><span class="sxs-lookup"><span data-stu-id="ca47a-108">Members</span></span>
|<span data-ttu-id="ca47a-109">成员</span><span class="sxs-lookup"><span data-stu-id="ca47a-109">Member</span></span>|<span data-ttu-id="ca47a-110">值</span><span class="sxs-lookup"><span data-stu-id="ca47a-110">Value</span></span>|<span data-ttu-id="ca47a-111">Description</span><span class="sxs-lookup"><span data-stu-id="ca47a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca47a-112">success</span><span class="sxs-lookup"><span data-stu-id="ca47a-112">success</span></span>|<span data-ttu-id="ca47a-113">0</span><span class="sxs-lookup"><span data-stu-id="ca47a-113">0</span></span>|<span data-ttu-id="ca47a-114">FileVault 状态成功</span><span class="sxs-lookup"><span data-stu-id="ca47a-114">FileVault State Success</span></span>|
|<span data-ttu-id="ca47a-115">driveEncryptedByUser</span><span class="sxs-lookup"><span data-stu-id="ca47a-115">driveEncryptedByUser</span></span>|<span data-ttu-id="ca47a-116">1</span><span class="sxs-lookup"><span data-stu-id="ca47a-116">1</span></span>|<span data-ttu-id="ca47a-117">FileVault 已由用户启用，且不受策略管理</span><span class="sxs-lookup"><span data-stu-id="ca47a-117">FileVault has been enabled by user and is not being managed by policy</span></span>|
|<span data-ttu-id="ca47a-118">userDeferredEncryption</span><span class="sxs-lookup"><span data-stu-id="ca47a-118">userDeferredEncryption</span></span>|<span data-ttu-id="ca47a-119">双面</span><span class="sxs-lookup"><span data-stu-id="ca47a-119">2</span></span>|<span data-ttu-id="ca47a-120">FileVault 策略已成功安装，但用户尚未开始加密</span><span class="sxs-lookup"><span data-stu-id="ca47a-120">FileVault policy is successfully installed but user has not started encryption</span></span>|
|<span data-ttu-id="ca47a-121">escrowNotEnabled</span><span class="sxs-lookup"><span data-stu-id="ca47a-121">escrowNotEnabled</span></span>|<span data-ttu-id="ca47a-122">4 </span><span class="sxs-lookup"><span data-stu-id="ca47a-122">4</span></span>|<span data-ttu-id="ca47a-123">FileVault 未启用恢复密钥的保管功能</span><span class="sxs-lookup"><span data-stu-id="ca47a-123">FileVault recovery key escrow is not enabled</span></span>|




