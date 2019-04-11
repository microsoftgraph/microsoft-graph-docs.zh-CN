---
title: defenderCloudBlockLevelType 枚举类型
description: 云块级别的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 88872e6d37afd1820559018bff6943e3ee623a0b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803211"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="a9276-103">defenderCloudBlockLevelType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a9276-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="a9276-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a9276-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9276-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a9276-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9276-106">云块级别的可能值</span><span class="sxs-lookup"><span data-stu-id="a9276-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="a9276-107">成员</span><span class="sxs-lookup"><span data-stu-id="a9276-107">Members</span></span>
|<span data-ttu-id="a9276-108">成员</span><span class="sxs-lookup"><span data-stu-id="a9276-108">Member</span></span>|<span data-ttu-id="a9276-109">值</span><span class="sxs-lookup"><span data-stu-id="a9276-109">Value</span></span>|<span data-ttu-id="a9276-110">说明</span><span class="sxs-lookup"><span data-stu-id="a9276-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9276-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a9276-111">notConfigured</span></span>|<span data-ttu-id="a9276-112">0</span><span class="sxs-lookup"><span data-stu-id="a9276-112">0</span></span>|<span data-ttu-id="a9276-113">默认值是, 使用默认的 Windows Defender 防病毒阻止级别, 并提供强大的检测功能, 而不会增加检测合法文件的风险</span><span class="sxs-lookup"><span data-stu-id="a9276-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="a9276-114">高效</span><span class="sxs-lookup"><span data-stu-id="a9276-114">high</span></span>|<span data-ttu-id="a9276-115">1</span><span class="sxs-lookup"><span data-stu-id="a9276-115">1</span></span>|<span data-ttu-id="a9276-116">High 适用于强级别的检测。</span><span class="sxs-lookup"><span data-stu-id="a9276-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="a9276-117">highPlus</span><span class="sxs-lookup"><span data-stu-id="a9276-117">highPlus</span></span>|<span data-ttu-id="a9276-118">双面</span><span class="sxs-lookup"><span data-stu-id="a9276-118">2</span></span>|<span data-ttu-id="a9276-119">高级别 + 使用高级别, 并应用附加保护措施</span><span class="sxs-lookup"><span data-stu-id="a9276-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="a9276-120">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="a9276-120">zeroTolerance</span></span>|<span data-ttu-id="a9276-121">第三章</span><span class="sxs-lookup"><span data-stu-id="a9276-121">3</span></span>|<span data-ttu-id="a9276-122">零耐受性阻止所有未知可执行文件</span><span class="sxs-lookup"><span data-stu-id="a9276-122">Zero tolerance blocks all unknown executables</span></span>|





