---
title: bitLockerRecoveryPasswordRotationType 枚举类型
description: BitLocker 恢复密码旋转类型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2e146e7ea01b2fd6bc89c659c14e6cd8c2692159
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075789"
---
# <a name="bitlockerrecoverypasswordrotationtype-enum-type"></a><span data-ttu-id="c8469-103">bitLockerRecoveryPasswordRotationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c8469-103">bitLockerRecoveryPasswordRotationType enum type</span></span>

<span data-ttu-id="c8469-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8469-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8469-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c8469-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8469-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c8469-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8469-107">BitLocker 恢复密码旋转类型</span><span class="sxs-lookup"><span data-stu-id="c8469-107">BitLocker recovery password rotation type</span></span>

## <a name="members"></a><span data-ttu-id="c8469-108">成员</span><span class="sxs-lookup"><span data-stu-id="c8469-108">Members</span></span>
|<span data-ttu-id="c8469-109">成员</span><span class="sxs-lookup"><span data-stu-id="c8469-109">Member</span></span>|<span data-ttu-id="c8469-110">值</span><span class="sxs-lookup"><span data-stu-id="c8469-110">Value</span></span>|<span data-ttu-id="c8469-111">说明</span><span class="sxs-lookup"><span data-stu-id="c8469-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8469-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c8469-112">notConfigured</span></span>|<span data-ttu-id="c8469-113">0</span><span class="sxs-lookup"><span data-stu-id="c8469-113">0</span></span>|<span data-ttu-id="c8469-114">未配置</span><span class="sxs-lookup"><span data-stu-id="c8469-114">Not configured</span></span>|
|<span data-ttu-id="c8469-115">禁用</span><span class="sxs-lookup"><span data-stu-id="c8469-115">disabled</span></span>|<span data-ttu-id="c8469-116">1 </span><span class="sxs-lookup"><span data-stu-id="c8469-116">1</span></span>|<span data-ttu-id="c8469-117">恢复密码旋转关闭</span><span class="sxs-lookup"><span data-stu-id="c8469-117">Recovery password rotation off</span></span>|
|<span data-ttu-id="c8469-118">enabledForAzureAd</span><span class="sxs-lookup"><span data-stu-id="c8469-118">enabledForAzureAd</span></span>|<span data-ttu-id="c8469-119">2 </span><span class="sxs-lookup"><span data-stu-id="c8469-119">2</span></span>|<span data-ttu-id="c8469-120">Azure AD 加入设备的恢复密码轮替</span><span class="sxs-lookup"><span data-stu-id="c8469-120">Recovery password rotation on for Azure AD joined devices</span></span>|
|<span data-ttu-id="c8469-121">enabledForAzureAdAndHybrid</span><span class="sxs-lookup"><span data-stu-id="c8469-121">enabledForAzureAdAndHybrid</span></span>|<span data-ttu-id="c8469-122">第三章</span><span class="sxs-lookup"><span data-stu-id="c8469-122">3</span></span>|<span data-ttu-id="c8469-123">Azure AD 加入设备和混合加入设备的恢复密码轮替</span><span class="sxs-lookup"><span data-stu-id="c8469-123">Recovery password rotation on for both Azure AD joined and hybrid joined devices</span></span>|






