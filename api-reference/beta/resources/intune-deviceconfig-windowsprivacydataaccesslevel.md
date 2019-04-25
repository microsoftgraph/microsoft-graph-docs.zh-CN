---
title: windowsPrivacyDataAccessLevel 枚举类型
description: 确定特定 Windows 隐私数据类别的访问级别。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 10486899094cf275cb3fb9254114d92cb7d12388
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541347"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="d787e-103">windowsPrivacyDataAccessLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d787e-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="d787e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d787e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d787e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d787e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d787e-106">确定特定 Windows 隐私数据类别的访问级别。</span><span class="sxs-lookup"><span data-stu-id="d787e-106">Determine the access level to specific Windows privacy data category.</span></span>

## <a name="members"></a><span data-ttu-id="d787e-107">成员</span><span class="sxs-lookup"><span data-stu-id="d787e-107">Members</span></span>
|<span data-ttu-id="d787e-108">成员</span><span class="sxs-lookup"><span data-stu-id="d787e-108">Member</span></span>|<span data-ttu-id="d787e-109">值</span><span class="sxs-lookup"><span data-stu-id="d787e-109">Value</span></span>|<span data-ttu-id="d787e-110">说明</span><span class="sxs-lookup"><span data-stu-id="d787e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d787e-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d787e-111">notConfigured</span></span>|<span data-ttu-id="d787e-112">0</span><span class="sxs-lookup"><span data-stu-id="d787e-112">0</span></span>|<span data-ttu-id="d787e-113">未指定访问级别, 无意向。</span><span class="sxs-lookup"><span data-stu-id="d787e-113">No access level specified, no intents.</span></span> <span data-ttu-id="d787e-114">在 UserInControl 或 ForceAllow 中, 设备的行为可能是一样的。</span><span class="sxs-lookup"><span data-stu-id="d787e-114">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="d787e-115">它可能取决于访问的隐私数据、Windows 版本和其他因素。</span><span class="sxs-lookup"><span data-stu-id="d787e-115">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="d787e-116">forceAllow</span><span class="sxs-lookup"><span data-stu-id="d787e-116">forceAllow</span></span>|<span data-ttu-id="d787e-117">1</span><span class="sxs-lookup"><span data-stu-id="d787e-117">1</span></span>|<span data-ttu-id="d787e-118">将允许应用访问指定的隐私数据。</span><span class="sxs-lookup"><span data-stu-id="d787e-118">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="d787e-119">forceDeny</span><span class="sxs-lookup"><span data-stu-id="d787e-119">forceDeny</span></span>|<span data-ttu-id="d787e-120">2 </span><span class="sxs-lookup"><span data-stu-id="d787e-120">2</span></span>|<span data-ttu-id="d787e-121">将拒绝应用程序访问指定的隐私数据。</span><span class="sxs-lookup"><span data-stu-id="d787e-121">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="d787e-122">userInControl</span><span class="sxs-lookup"><span data-stu-id="d787e-122">userInControl</span></span>|<span data-ttu-id="d787e-123">3 </span><span class="sxs-lookup"><span data-stu-id="d787e-123">3</span></span>|<span data-ttu-id="d787e-124">当应用尝试访问指定的隐私数据时, 系统将提示用户。</span><span class="sxs-lookup"><span data-stu-id="d787e-124">Users will be prompted when apps try to access specified privacy data.</span></span>|





