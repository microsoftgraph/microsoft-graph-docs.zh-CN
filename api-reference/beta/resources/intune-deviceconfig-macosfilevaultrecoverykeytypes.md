---
title: macOSFileVaultRecoveryKeyTypes 枚举类型
description: MacOS FileVault 的恢复密钥类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1a72cc8ddb4e9ce28a65e3af006ebec097eda247
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365053"
---
# <a name="macosfilevaultrecoverykeytypes-enum-type"></a><span data-ttu-id="32a2e-103">macOSFileVaultRecoveryKeyTypes 枚举类型</span><span class="sxs-lookup"><span data-stu-id="32a2e-103">macOSFileVaultRecoveryKeyTypes enum type</span></span>

> <span data-ttu-id="32a2e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="32a2e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32a2e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="32a2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32a2e-106">MacOS FileVault 的恢复密钥类型</span><span class="sxs-lookup"><span data-stu-id="32a2e-106">Recovery key types for macOS FileVault</span></span>

## <a name="members"></a><span data-ttu-id="32a2e-107">成员</span><span class="sxs-lookup"><span data-stu-id="32a2e-107">Members</span></span>
|<span data-ttu-id="32a2e-108">成员</span><span class="sxs-lookup"><span data-stu-id="32a2e-108">Member</span></span>|<span data-ttu-id="32a2e-109">值</span><span class="sxs-lookup"><span data-stu-id="32a2e-109">Value</span></span>|<span data-ttu-id="32a2e-110">说明</span><span class="sxs-lookup"><span data-stu-id="32a2e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32a2e-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="32a2e-111">notConfigured</span></span>|<span data-ttu-id="32a2e-112">0</span><span class="sxs-lookup"><span data-stu-id="32a2e-112">0</span></span>|<span data-ttu-id="32a2e-113">设备默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="32a2e-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="32a2e-114">institutionalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="32a2e-114">institutionalRecoveryKey</span></span>|<span data-ttu-id="32a2e-115">1</span><span class="sxs-lookup"><span data-stu-id="32a2e-115">1</span></span>|<span data-ttu-id="32a2e-116">机构恢复密钥类似于 "主" 恢复密钥, 可用于解锁已丢失密码的任何设备。</span><span class="sxs-lookup"><span data-stu-id="32a2e-116">An institutional recovery key is like a “master” recovery key that can be used to unlock any device whose password has been lost.</span></span>|
|<span data-ttu-id="32a2e-117">personalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="32a2e-117">personalRecoveryKey</span></span>|<span data-ttu-id="32a2e-118">双面</span><span class="sxs-lookup"><span data-stu-id="32a2e-118">2</span></span>|<span data-ttu-id="32a2e-119">个人恢复密钥是唯一的代码, 可用于解锁用户的设备, 即使设备的密码丢失也是如此。</span><span class="sxs-lookup"><span data-stu-id="32a2e-119">A personal recovery key is a unique code that can be used to unlock the user’s device, even if the password to the device is lost.</span></span>|



