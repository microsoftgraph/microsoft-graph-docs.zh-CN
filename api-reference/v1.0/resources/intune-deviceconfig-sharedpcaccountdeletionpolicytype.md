---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 当共享 PC 上删除帐户可能值。
author: tfitzmac
ms.openlocfilehash: 8789faeeec7772cd6115cae82691c62894446f59
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27300999"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="f3466-103">sharedPCAccountDeletionPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f3466-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="f3466-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f3466-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3466-105">当共享 PC 上删除帐户可能值。</span><span class="sxs-lookup"><span data-stu-id="f3466-105">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="f3466-106">成员</span><span class="sxs-lookup"><span data-stu-id="f3466-106">Members</span></span>
|<span data-ttu-id="f3466-107">成员</span><span class="sxs-lookup"><span data-stu-id="f3466-107">Member</span></span>|<span data-ttu-id="f3466-108">值</span><span class="sxs-lookup"><span data-stu-id="f3466-108">Value</span></span>|<span data-ttu-id="f3466-109">说明</span><span class="sxs-lookup"><span data-stu-id="f3466-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3466-110">立即</span><span class="sxs-lookup"><span data-stu-id="f3466-110">immediate</span></span>|<span data-ttu-id="f3466-111">0</span><span class="sxs-lookup"><span data-stu-id="f3466-111">0</span></span>|<span data-ttu-id="f3466-112">立即删除。</span><span class="sxs-lookup"><span data-stu-id="f3466-112">Delete immediately.</span></span>|
|<span data-ttu-id="f3466-113">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="f3466-113">diskSpaceThreshold</span></span>|<span data-ttu-id="f3466-114">1</span><span class="sxs-lookup"><span data-stu-id="f3466-114">1</span></span>|<span data-ttu-id="f3466-115">删除在磁盘空间阈值。</span><span class="sxs-lookup"><span data-stu-id="f3466-115">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="f3466-116">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="f3466-116">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="f3466-117">2</span><span class="sxs-lookup"><span data-stu-id="f3466-117">2</span></span>|<span data-ttu-id="f3466-118">删除在磁盘空间阈值或非活动状态的阈值。</span><span class="sxs-lookup"><span data-stu-id="f3466-118">Delete at disk space threshold or inactive threshold.</span></span>|



