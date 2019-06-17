---
title: windowsPrivacyDataAccessLevel 枚举类型
description: 确定特定 Windows 隐私数据类别的访问级别。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c6eea937d05d45e6fcf7fa955df16885067047b3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996481"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="f6c20-103">windowsPrivacyDataAccessLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f6c20-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="f6c20-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f6c20-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6c20-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f6c20-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6c20-106">确定特定 Windows 隐私数据类别的访问级别。</span><span class="sxs-lookup"><span data-stu-id="f6c20-106">Determine the access level to specific Windows privacy data category.</span></span>

## <a name="members"></a><span data-ttu-id="f6c20-107">成员</span><span class="sxs-lookup"><span data-stu-id="f6c20-107">Members</span></span>
|<span data-ttu-id="f6c20-108">成员</span><span class="sxs-lookup"><span data-stu-id="f6c20-108">Member</span></span>|<span data-ttu-id="f6c20-109">值</span><span class="sxs-lookup"><span data-stu-id="f6c20-109">Value</span></span>|<span data-ttu-id="f6c20-110">说明</span><span class="sxs-lookup"><span data-stu-id="f6c20-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6c20-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f6c20-111">notConfigured</span></span>|<span data-ttu-id="f6c20-112">0</span><span class="sxs-lookup"><span data-stu-id="f6c20-112">0</span></span>|<span data-ttu-id="f6c20-113">未指定访问级别, 无意向。</span><span class="sxs-lookup"><span data-stu-id="f6c20-113">No access level specified, no intents.</span></span> <span data-ttu-id="f6c20-114">在 UserInControl 或 ForceAllow 中, 设备的行为可能是一样的。</span><span class="sxs-lookup"><span data-stu-id="f6c20-114">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="f6c20-115">它可能取决于访问的隐私数据、Windows 版本和其他因素。</span><span class="sxs-lookup"><span data-stu-id="f6c20-115">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="f6c20-116">forceAllow</span><span class="sxs-lookup"><span data-stu-id="f6c20-116">forceAllow</span></span>|<span data-ttu-id="f6c20-117">1</span><span class="sxs-lookup"><span data-stu-id="f6c20-117">1</span></span>|<span data-ttu-id="f6c20-118">将允许应用访问指定的隐私数据。</span><span class="sxs-lookup"><span data-stu-id="f6c20-118">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="f6c20-119">forceDeny</span><span class="sxs-lookup"><span data-stu-id="f6c20-119">forceDeny</span></span>|<span data-ttu-id="f6c20-120">双面</span><span class="sxs-lookup"><span data-stu-id="f6c20-120">2</span></span>|<span data-ttu-id="f6c20-121">将拒绝应用程序访问指定的隐私数据。</span><span class="sxs-lookup"><span data-stu-id="f6c20-121">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="f6c20-122">userInControl</span><span class="sxs-lookup"><span data-stu-id="f6c20-122">userInControl</span></span>|<span data-ttu-id="f6c20-123">第三章</span><span class="sxs-lookup"><span data-stu-id="f6c20-123">3</span></span>|<span data-ttu-id="f6c20-124">当应用尝试访问指定的隐私数据时, 系统将提示用户。</span><span class="sxs-lookup"><span data-stu-id="f6c20-124">Users will be prompted when apps try to access specified privacy data.</span></span>|





