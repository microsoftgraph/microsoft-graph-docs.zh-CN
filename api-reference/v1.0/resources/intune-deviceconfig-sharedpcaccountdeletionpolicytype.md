---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 在共享电脑上删除帐户时的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c547a59c02e3c4cad9bd8140a2e11ca6e3c84a7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534617"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="a85b0-103">sharedPCAccountDeletionPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a85b0-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="a85b0-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a85b0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a85b0-105">在共享电脑上删除帐户时的可能值。</span><span class="sxs-lookup"><span data-stu-id="a85b0-105">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="a85b0-106">成员</span><span class="sxs-lookup"><span data-stu-id="a85b0-106">Members</span></span>
|<span data-ttu-id="a85b0-107">成员</span><span class="sxs-lookup"><span data-stu-id="a85b0-107">Member</span></span>|<span data-ttu-id="a85b0-108">值</span><span class="sxs-lookup"><span data-stu-id="a85b0-108">Value</span></span>|<span data-ttu-id="a85b0-109">说明</span><span class="sxs-lookup"><span data-stu-id="a85b0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a85b0-110">迫切</span><span class="sxs-lookup"><span data-stu-id="a85b0-110">immediate</span></span>|<span data-ttu-id="a85b0-111">0</span><span class="sxs-lookup"><span data-stu-id="a85b0-111">0</span></span>|<span data-ttu-id="a85b0-112">立即删除。</span><span class="sxs-lookup"><span data-stu-id="a85b0-112">Delete immediately.</span></span>|
|<span data-ttu-id="a85b0-113">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="a85b0-113">diskSpaceThreshold</span></span>|<span data-ttu-id="a85b0-114">1</span><span class="sxs-lookup"><span data-stu-id="a85b0-114">1</span></span>|<span data-ttu-id="a85b0-115">在磁盘空间阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="a85b0-115">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="a85b0-116">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="a85b0-116">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="a85b0-117">2 </span><span class="sxs-lookup"><span data-stu-id="a85b0-117">2</span></span>|<span data-ttu-id="a85b0-118">在磁盘空间阈值或非活动阈值中删除。</span><span class="sxs-lookup"><span data-stu-id="a85b0-118">Delete at disk space threshold or inactive threshold.</span></span>|



