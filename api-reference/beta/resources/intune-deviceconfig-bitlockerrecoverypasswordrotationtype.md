---
title: bitLockerRecoveryPasswordRotationType 枚举类型
description: BitLocker 恢复密码旋转类型
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c8a597619c0fa7358f6d86fec3ce12d89257b849
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469670"
---
# <a name="bitlockerrecoverypasswordrotationtype-enum-type"></a><span data-ttu-id="9a016-103">bitLockerRecoveryPasswordRotationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9a016-103">bitLockerRecoveryPasswordRotationType enum type</span></span>

<span data-ttu-id="9a016-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a016-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a016-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9a016-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a016-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9a016-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a016-107">BitLocker 恢复密码旋转类型</span><span class="sxs-lookup"><span data-stu-id="9a016-107">BitLocker recovery password rotation type</span></span>

## <a name="members"></a><span data-ttu-id="9a016-108">成员</span><span class="sxs-lookup"><span data-stu-id="9a016-108">Members</span></span>
|<span data-ttu-id="9a016-109">成员</span><span class="sxs-lookup"><span data-stu-id="9a016-109">Member</span></span>|<span data-ttu-id="9a016-110">值</span><span class="sxs-lookup"><span data-stu-id="9a016-110">Value</span></span>|<span data-ttu-id="9a016-111">说明</span><span class="sxs-lookup"><span data-stu-id="9a016-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a016-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9a016-112">notConfigured</span></span>|<span data-ttu-id="9a016-113">0</span><span class="sxs-lookup"><span data-stu-id="9a016-113">0</span></span>|<span data-ttu-id="9a016-114">未配置</span><span class="sxs-lookup"><span data-stu-id="9a016-114">Not configured</span></span>|
|<span data-ttu-id="9a016-115">禁用</span><span class="sxs-lookup"><span data-stu-id="9a016-115">disabled</span></span>|<span data-ttu-id="9a016-116">1</span><span class="sxs-lookup"><span data-stu-id="9a016-116">1</span></span>|<span data-ttu-id="9a016-117">恢复密码旋转关闭</span><span class="sxs-lookup"><span data-stu-id="9a016-117">Recovery password rotation off</span></span>|
|<span data-ttu-id="9a016-118">enabledForAzureAd</span><span class="sxs-lookup"><span data-stu-id="9a016-118">enabledForAzureAd</span></span>|<span data-ttu-id="9a016-119">双面</span><span class="sxs-lookup"><span data-stu-id="9a016-119">2</span></span>|<span data-ttu-id="9a016-120">Azure AD 加入设备的恢复密码轮替</span><span class="sxs-lookup"><span data-stu-id="9a016-120">Recovery password rotation on for Azure AD joined devices</span></span>|
|<span data-ttu-id="9a016-121">enabledForAzureAdAndHybrid</span><span class="sxs-lookup"><span data-stu-id="9a016-121">enabledForAzureAdAndHybrid</span></span>|<span data-ttu-id="9a016-122">第三章</span><span class="sxs-lookup"><span data-stu-id="9a016-122">3</span></span>|<span data-ttu-id="9a016-123">Azure AD 加入设备和混合加入设备的恢复密码轮替</span><span class="sxs-lookup"><span data-stu-id="9a016-123">Recovery password rotation on for both Azure AD joined and hybrid joined devices</span></span>|



