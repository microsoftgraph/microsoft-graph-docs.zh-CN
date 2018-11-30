---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 当共享 PC 上删除帐户可能值。
ms.openlocfilehash: 48d36881646bce344d99bc3d1a15a2679ddeb11d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009291"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="8fd1f-103">sharedPCAccountDeletionPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8fd1f-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="8fd1f-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8fd1f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8fd1f-105">当共享 PC 上删除帐户可能值。</span><span class="sxs-lookup"><span data-stu-id="8fd1f-105">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="8fd1f-106">成员</span><span class="sxs-lookup"><span data-stu-id="8fd1f-106">Members</span></span>
|<span data-ttu-id="8fd1f-107">成员</span><span class="sxs-lookup"><span data-stu-id="8fd1f-107">Member</span></span>|<span data-ttu-id="8fd1f-108">值</span><span class="sxs-lookup"><span data-stu-id="8fd1f-108">Value</span></span>|<span data-ttu-id="8fd1f-109">说明</span><span class="sxs-lookup"><span data-stu-id="8fd1f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fd1f-110">立即</span><span class="sxs-lookup"><span data-stu-id="8fd1f-110">immediate</span></span>|<span data-ttu-id="8fd1f-111">0</span><span class="sxs-lookup"><span data-stu-id="8fd1f-111">0</span></span>|<span data-ttu-id="8fd1f-112">立即删除。</span><span class="sxs-lookup"><span data-stu-id="8fd1f-112">Delete immediately.</span></span>|
|<span data-ttu-id="8fd1f-113">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="8fd1f-113">diskSpaceThreshold</span></span>|<span data-ttu-id="8fd1f-114">1</span><span class="sxs-lookup"><span data-stu-id="8fd1f-114">1</span></span>|<span data-ttu-id="8fd1f-115">删除在磁盘空间阈值。</span><span class="sxs-lookup"><span data-stu-id="8fd1f-115">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="8fd1f-116">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="8fd1f-116">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="8fd1f-117">2</span><span class="sxs-lookup"><span data-stu-id="8fd1f-117">2</span></span>|<span data-ttu-id="8fd1f-118">删除在磁盘空间阈值或非活动状态的阈值。</span><span class="sxs-lookup"><span data-stu-id="8fd1f-118">Delete at disk space threshold or inactive threshold.</span></span>|



