---
title: bitLockerRecoveryPasswordRotationType 枚举类型
description: BitLocker 恢复密码旋转类型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d6f77bb5411a7d7a53fd4d95c5740c6044f8b851
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260535"
---
# <a name="bitlockerrecoverypasswordrotationtype-enum-type"></a><span data-ttu-id="b971b-103">bitLockerRecoveryPasswordRotationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b971b-103">bitLockerRecoveryPasswordRotationType enum type</span></span>

<span data-ttu-id="b971b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b971b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b971b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b971b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b971b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b971b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b971b-107">BitLocker 恢复密码旋转类型</span><span class="sxs-lookup"><span data-stu-id="b971b-107">BitLocker recovery password rotation type</span></span>

## <a name="members"></a><span data-ttu-id="b971b-108">成员</span><span class="sxs-lookup"><span data-stu-id="b971b-108">Members</span></span>
|<span data-ttu-id="b971b-109">成员</span><span class="sxs-lookup"><span data-stu-id="b971b-109">Member</span></span>|<span data-ttu-id="b971b-110">值</span><span class="sxs-lookup"><span data-stu-id="b971b-110">Value</span></span>|<span data-ttu-id="b971b-111">说明</span><span class="sxs-lookup"><span data-stu-id="b971b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b971b-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b971b-112">notConfigured</span></span>|<span data-ttu-id="b971b-113">0</span><span class="sxs-lookup"><span data-stu-id="b971b-113">0</span></span>|<span data-ttu-id="b971b-114">未配置</span><span class="sxs-lookup"><span data-stu-id="b971b-114">Not configured</span></span>|
|<span data-ttu-id="b971b-115">禁用</span><span class="sxs-lookup"><span data-stu-id="b971b-115">disabled</span></span>|<span data-ttu-id="b971b-116">1</span><span class="sxs-lookup"><span data-stu-id="b971b-116">1</span></span>|<span data-ttu-id="b971b-117">恢复密码旋转关闭</span><span class="sxs-lookup"><span data-stu-id="b971b-117">Recovery password rotation off</span></span>|
|<span data-ttu-id="b971b-118">enabledForAzureAd</span><span class="sxs-lookup"><span data-stu-id="b971b-118">enabledForAzureAd</span></span>|<span data-ttu-id="b971b-119">双面</span><span class="sxs-lookup"><span data-stu-id="b971b-119">2</span></span>|<span data-ttu-id="b971b-120">Azure AD 加入设备的恢复密码轮替</span><span class="sxs-lookup"><span data-stu-id="b971b-120">Recovery password rotation on for Azure AD joined devices</span></span>|
|<span data-ttu-id="b971b-121">enabledForAzureAdAndHybrid</span><span class="sxs-lookup"><span data-stu-id="b971b-121">enabledForAzureAdAndHybrid</span></span>|<span data-ttu-id="b971b-122">第三章</span><span class="sxs-lookup"><span data-stu-id="b971b-122">3</span></span>|<span data-ttu-id="b971b-123">Azure AD 加入设备和混合加入设备的恢复密码轮替</span><span class="sxs-lookup"><span data-stu-id="b971b-123">Recovery password rotation on for both Azure AD joined and hybrid joined devices</span></span>|




