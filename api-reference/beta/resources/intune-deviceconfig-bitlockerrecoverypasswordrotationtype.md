---
title: bitLockerRecoveryPasswordRotationType 枚举类型
description: BitLocker 恢复密码旋转类型
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e0be99dd7307c13975c430a5693098ca57e9eb6e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795741"
---
# <a name="bitlockerrecoverypasswordrotationtype-enum-type"></a><span data-ttu-id="c5d5a-103">bitLockerRecoveryPasswordRotationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c5d5a-103">bitLockerRecoveryPasswordRotationType enum type</span></span>

> <span data-ttu-id="c5d5a-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c5d5a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5d5a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c5d5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5d5a-106">BitLocker 恢复密码旋转类型</span><span class="sxs-lookup"><span data-stu-id="c5d5a-106">BitLocker recovery password rotation type</span></span>

## <a name="members"></a><span data-ttu-id="c5d5a-107">成员</span><span class="sxs-lookup"><span data-stu-id="c5d5a-107">Members</span></span>
|<span data-ttu-id="c5d5a-108">成员</span><span class="sxs-lookup"><span data-stu-id="c5d5a-108">Member</span></span>|<span data-ttu-id="c5d5a-109">值</span><span class="sxs-lookup"><span data-stu-id="c5d5a-109">Value</span></span>|<span data-ttu-id="c5d5a-110">说明</span><span class="sxs-lookup"><span data-stu-id="c5d5a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5d5a-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c5d5a-111">notConfigured</span></span>|<span data-ttu-id="c5d5a-112">0</span><span class="sxs-lookup"><span data-stu-id="c5d5a-112">0</span></span>|<span data-ttu-id="c5d5a-113">未配置</span><span class="sxs-lookup"><span data-stu-id="c5d5a-113">Not configured</span></span>|
|<span data-ttu-id="c5d5a-114">禁用</span><span class="sxs-lookup"><span data-stu-id="c5d5a-114">disabled</span></span>|<span data-ttu-id="c5d5a-115">1</span><span class="sxs-lookup"><span data-stu-id="c5d5a-115">1</span></span>|<span data-ttu-id="c5d5a-116">恢复密码旋转关闭</span><span class="sxs-lookup"><span data-stu-id="c5d5a-116">Recovery password rotation off</span></span>|
|<span data-ttu-id="c5d5a-117">enabledForAzureAd</span><span class="sxs-lookup"><span data-stu-id="c5d5a-117">enabledForAzureAd</span></span>|<span data-ttu-id="c5d5a-118">双面</span><span class="sxs-lookup"><span data-stu-id="c5d5a-118">2</span></span>|<span data-ttu-id="c5d5a-119">Azure AD 加入设备的恢复密码轮替</span><span class="sxs-lookup"><span data-stu-id="c5d5a-119">Recovery password rotation on for Azure AD joined devices</span></span>|
|<span data-ttu-id="c5d5a-120">enabledForAzureAdAndHybrid</span><span class="sxs-lookup"><span data-stu-id="c5d5a-120">enabledForAzureAdAndHybrid</span></span>|<span data-ttu-id="c5d5a-121">第三章</span><span class="sxs-lookup"><span data-stu-id="c5d5a-121">3</span></span>|<span data-ttu-id="c5d5a-122">Azure AD 加入设备和混合加入设备的恢复密码轮替</span><span class="sxs-lookup"><span data-stu-id="c5d5a-122">Recovery password rotation on for both Azure AD joined and hybrid joined devices</span></span>|



