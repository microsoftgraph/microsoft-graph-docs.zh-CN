---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 当共享 PC 上删除帐户可能值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 645cd3dfd4121c6c9bdd9d57a0dc3b63723cc461
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415164"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="d9260-103">sharedPCAccountDeletionPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d9260-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="d9260-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d9260-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d9260-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d9260-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9260-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d9260-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9260-107">当共享 PC 上删除帐户可能值。</span><span class="sxs-lookup"><span data-stu-id="d9260-107">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="d9260-108">成员</span><span class="sxs-lookup"><span data-stu-id="d9260-108">Members</span></span>
|<span data-ttu-id="d9260-109">成员</span><span class="sxs-lookup"><span data-stu-id="d9260-109">Member</span></span>|<span data-ttu-id="d9260-110">值</span><span class="sxs-lookup"><span data-stu-id="d9260-110">Value</span></span>|<span data-ttu-id="d9260-111">说明</span><span class="sxs-lookup"><span data-stu-id="d9260-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9260-112">立即</span><span class="sxs-lookup"><span data-stu-id="d9260-112">immediate</span></span>|<span data-ttu-id="d9260-113">0</span><span class="sxs-lookup"><span data-stu-id="d9260-113">0</span></span>|<span data-ttu-id="d9260-114">立即删除。</span><span class="sxs-lookup"><span data-stu-id="d9260-114">Delete immediately.</span></span>|
|<span data-ttu-id="d9260-115">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="d9260-115">diskSpaceThreshold</span></span>|<span data-ttu-id="d9260-116">1</span><span class="sxs-lookup"><span data-stu-id="d9260-116">1</span></span>|<span data-ttu-id="d9260-117">删除在磁盘空间阈值。</span><span class="sxs-lookup"><span data-stu-id="d9260-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="d9260-118">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="d9260-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="d9260-119">2</span><span class="sxs-lookup"><span data-stu-id="d9260-119">2</span></span>|<span data-ttu-id="d9260-120">删除在磁盘空间阈值或非活动状态的阈值。</span><span class="sxs-lookup"><span data-stu-id="d9260-120">Delete at disk space threshold or inactive threshold.</span></span>|




