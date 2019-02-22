---
title: defenderCloudBlockLevelType 枚举类型
description: 云块级别的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cbf442a11335602c510a210d7bd805b2a76eb7df
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156922"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="b6cb2-103">defenderCloudBlockLevelType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b6cb2-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="b6cb2-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b6cb2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6cb2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b6cb2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6cb2-106">云块级别的可能值</span><span class="sxs-lookup"><span data-stu-id="b6cb2-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="b6cb2-107">成员</span><span class="sxs-lookup"><span data-stu-id="b6cb2-107">Members</span></span>
|<span data-ttu-id="b6cb2-108">成员</span><span class="sxs-lookup"><span data-stu-id="b6cb2-108">Member</span></span>|<span data-ttu-id="b6cb2-109">值</span><span class="sxs-lookup"><span data-stu-id="b6cb2-109">Value</span></span>|<span data-ttu-id="b6cb2-110">说明</span><span class="sxs-lookup"><span data-stu-id="b6cb2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6cb2-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b6cb2-111">notConfigured</span></span>|<span data-ttu-id="b6cb2-112">0</span><span class="sxs-lookup"><span data-stu-id="b6cb2-112">0</span></span>|<span data-ttu-id="b6cb2-113">默认值是, 使用默认的 Windows Defender 防病毒阻止级别, 并提供强大的检测功能, 而不会增加检测合法文件的风险</span><span class="sxs-lookup"><span data-stu-id="b6cb2-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="b6cb2-114">高效</span><span class="sxs-lookup"><span data-stu-id="b6cb2-114">high</span></span>|<span data-ttu-id="b6cb2-115">1</span><span class="sxs-lookup"><span data-stu-id="b6cb2-115">1</span></span>|<span data-ttu-id="b6cb2-116">High 适用于强级别的检测。</span><span class="sxs-lookup"><span data-stu-id="b6cb2-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="b6cb2-117">highPlus</span><span class="sxs-lookup"><span data-stu-id="b6cb2-117">highPlus</span></span>|<span data-ttu-id="b6cb2-118">双面</span><span class="sxs-lookup"><span data-stu-id="b6cb2-118">2</span></span>|<span data-ttu-id="b6cb2-119">高级别 + 使用高级别, 并应用附加保护措施</span><span class="sxs-lookup"><span data-stu-id="b6cb2-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="b6cb2-120">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="b6cb2-120">zeroTolerance</span></span>|<span data-ttu-id="b6cb2-121">第三章</span><span class="sxs-lookup"><span data-stu-id="b6cb2-121">3</span></span>|<span data-ttu-id="b6cb2-122">零耐受性阻止所有未知可执行文件</span><span class="sxs-lookup"><span data-stu-id="b6cb2-122">Zero tolerance blocks all unknown executables</span></span>|




