---
title: defenderCloudBlockLevelType 枚举类型
description: 云块级别的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c00ae796101131456db7206b80e4b6d8999fb86a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729754"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="e2657-103">defenderCloudBlockLevelType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e2657-103">defenderCloudBlockLevelType enum type</span></span>

<span data-ttu-id="e2657-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2657-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2657-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e2657-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2657-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e2657-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2657-107">云块级别的可能值</span><span class="sxs-lookup"><span data-stu-id="e2657-107">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="e2657-108">成员</span><span class="sxs-lookup"><span data-stu-id="e2657-108">Members</span></span>
|<span data-ttu-id="e2657-109">成员</span><span class="sxs-lookup"><span data-stu-id="e2657-109">Member</span></span>|<span data-ttu-id="e2657-110">值</span><span class="sxs-lookup"><span data-stu-id="e2657-110">Value</span></span>|<span data-ttu-id="e2657-111">说明</span><span class="sxs-lookup"><span data-stu-id="e2657-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2657-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e2657-112">notConfigured</span></span>|<span data-ttu-id="e2657-113">0</span><span class="sxs-lookup"><span data-stu-id="e2657-113">0</span></span>|<span data-ttu-id="e2657-114">默认值是，使用默认的 Windows Defender 防病毒阻止级别，并提供强大的检测功能，而不会增加检测合法文件的风险</span><span class="sxs-lookup"><span data-stu-id="e2657-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="e2657-115">高效</span><span class="sxs-lookup"><span data-stu-id="e2657-115">high</span></span>|<span data-ttu-id="e2657-116">1</span><span class="sxs-lookup"><span data-stu-id="e2657-116">1</span></span>|<span data-ttu-id="e2657-117">High 适用于强级别的检测。</span><span class="sxs-lookup"><span data-stu-id="e2657-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="e2657-118">highPlus</span><span class="sxs-lookup"><span data-stu-id="e2657-118">highPlus</span></span>|<span data-ttu-id="e2657-119">双面</span><span class="sxs-lookup"><span data-stu-id="e2657-119">2</span></span>|<span data-ttu-id="e2657-120">高级别 + 使用高级别，并应用附加保护措施</span><span class="sxs-lookup"><span data-stu-id="e2657-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="e2657-121">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="e2657-121">zeroTolerance</span></span>|<span data-ttu-id="e2657-122">第三章</span><span class="sxs-lookup"><span data-stu-id="e2657-122">3</span></span>|<span data-ttu-id="e2657-123">零耐受性阻止所有未知可执行文件</span><span class="sxs-lookup"><span data-stu-id="e2657-123">Zero tolerance blocks all unknown executables</span></span>|





