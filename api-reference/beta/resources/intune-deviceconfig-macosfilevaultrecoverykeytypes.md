---
title: macOSFileVaultRecoveryKeyTypes 枚举类型
description: MacOS FileVault 的恢复密钥类型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 75d6de635ecddf44ce7eaa5f0c731af59125a7d0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724570"
---
# <a name="macosfilevaultrecoverykeytypes-enum-type"></a><span data-ttu-id="12c25-103">macOSFileVaultRecoveryKeyTypes 枚举类型</span><span class="sxs-lookup"><span data-stu-id="12c25-103">macOSFileVaultRecoveryKeyTypes enum type</span></span>

<span data-ttu-id="12c25-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12c25-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12c25-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="12c25-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12c25-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12c25-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12c25-107">MacOS FileVault 的恢复密钥类型</span><span class="sxs-lookup"><span data-stu-id="12c25-107">Recovery key types for macOS FileVault</span></span>

## <a name="members"></a><span data-ttu-id="12c25-108">成员</span><span class="sxs-lookup"><span data-stu-id="12c25-108">Members</span></span>
|<span data-ttu-id="12c25-109">成员</span><span class="sxs-lookup"><span data-stu-id="12c25-109">Member</span></span>|<span data-ttu-id="12c25-110">值</span><span class="sxs-lookup"><span data-stu-id="12c25-110">Value</span></span>|<span data-ttu-id="12c25-111">说明</span><span class="sxs-lookup"><span data-stu-id="12c25-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12c25-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="12c25-112">notConfigured</span></span>|<span data-ttu-id="12c25-113">0</span><span class="sxs-lookup"><span data-stu-id="12c25-113">0</span></span>|<span data-ttu-id="12c25-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="12c25-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="12c25-115">institutionalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="12c25-115">institutionalRecoveryKey</span></span>|<span data-ttu-id="12c25-116">1</span><span class="sxs-lookup"><span data-stu-id="12c25-116">1</span></span>|<span data-ttu-id="12c25-117">机构恢复密钥类似于 "主" 恢复密钥，可用于解锁已丢失密码的任何设备。</span><span class="sxs-lookup"><span data-stu-id="12c25-117">An institutional recovery key is like a “master” recovery key that can be used to unlock any device whose password has been lost.</span></span>|
|<span data-ttu-id="12c25-118">personalRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="12c25-118">personalRecoveryKey</span></span>|<span data-ttu-id="12c25-119">双面</span><span class="sxs-lookup"><span data-stu-id="12c25-119">2</span></span>|<span data-ttu-id="12c25-120">个人恢复密钥是唯一的代码，可用于解锁用户的设备，即使设备的密码丢失也是如此。</span><span class="sxs-lookup"><span data-stu-id="12c25-120">A personal recovery key is a unique code that can be used to unlock the user’s device, even if the password to the device is lost.</span></span>|





