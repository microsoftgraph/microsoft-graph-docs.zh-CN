---
title: macOSFileVaultRecoveryKeyTypes 枚举类型
description: MacOS FileVault 的恢复密钥类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 193bfc5769da2919f93df9beef38524a57bfece0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002544"
---
# <a name="macosfilevaultrecoverykeytypes-enum-type"></a><span data-ttu-id="996f9-103">macOSFileVaultRecoveryKeyTypes 枚举类型</span><span class="sxs-lookup"><span data-stu-id="996f9-103">macOSFileVaultRecoveryKeyTypes enum type</span></span>

> <span data-ttu-id="996f9-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="996f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="996f9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="996f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="996f9-106">MacOS FileVault 的恢复密钥类型</span><span class="sxs-lookup"><span data-stu-id="996f9-106">Recovery key types for macOS FileVault</span></span>

## <a name="members"></a><span data-ttu-id="996f9-107">成员</span><span class="sxs-lookup"><span data-stu-id="996f9-107">Members</span></span>
|<span data-ttu-id="996f9-108">成员</span><span class="sxs-lookup"><span data-stu-id="996f9-108">Member</span></span>|<span data-ttu-id="996f9-109">值</span><span class="sxs-lookup"><span data-stu-id="996f9-109">Value</span></span>|<span data-ttu-id="996f9-110">说明</span><span class="sxs-lookup"><span data-stu-id="996f9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="996f9-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="996f9-111">notConfigured</span></span>|<span data-ttu-id="996f9-112">0</span><span class="sxs-lookup"><span data-stu-id="996f9-112">0</span></span>|<span data-ttu-id="996f9-113">设备默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="996f9-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="996f9-114">institutionalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="996f9-114">institutionalRecoveryKey</span></span>|<span data-ttu-id="996f9-115">1</span><span class="sxs-lookup"><span data-stu-id="996f9-115">1</span></span>|<span data-ttu-id="996f9-116">机构恢复密钥类似于 "主" 恢复密钥, 可用于解锁已丢失密码的任何设备。</span><span class="sxs-lookup"><span data-stu-id="996f9-116">An institutional recovery key is like a “master” recovery key that can be used to unlock any device whose password has been lost.</span></span>|
|<span data-ttu-id="996f9-117">personalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="996f9-117">personalRecoveryKey</span></span>|<span data-ttu-id="996f9-118">双面</span><span class="sxs-lookup"><span data-stu-id="996f9-118">2</span></span>|<span data-ttu-id="996f9-119">个人恢复密钥是唯一的代码, 可用于解锁用户的设备, 即使设备的密码丢失也是如此。</span><span class="sxs-lookup"><span data-stu-id="996f9-119">A personal recovery key is a unique code that can be used to unlock the user’s device, even if the password to the device is lost.</span></span>|





