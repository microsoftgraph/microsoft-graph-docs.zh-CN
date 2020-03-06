---
title: defenderCloudBlockLevelType 枚举类型
description: 云块级别的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bd121a61106ae029ccacf2e393bd28ef34415045
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530894"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="fc80b-103">defenderCloudBlockLevelType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fc80b-103">defenderCloudBlockLevelType enum type</span></span>

<span data-ttu-id="fc80b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc80b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc80b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc80b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc80b-106">云块级别的可能值</span><span class="sxs-lookup"><span data-stu-id="fc80b-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="fc80b-107">成员</span><span class="sxs-lookup"><span data-stu-id="fc80b-107">Members</span></span>
|<span data-ttu-id="fc80b-108">成员</span><span class="sxs-lookup"><span data-stu-id="fc80b-108">Member</span></span>|<span data-ttu-id="fc80b-109">值</span><span class="sxs-lookup"><span data-stu-id="fc80b-109">Value</span></span>|<span data-ttu-id="fc80b-110">说明</span><span class="sxs-lookup"><span data-stu-id="fc80b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc80b-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="fc80b-111">notConfigured</span></span>|<span data-ttu-id="fc80b-112">0</span><span class="sxs-lookup"><span data-stu-id="fc80b-112">0</span></span>|<span data-ttu-id="fc80b-113">默认值是，使用默认的 Windows Defender 防病毒阻止级别，并提供强大的检测功能，而不会增加检测合法文件的风险</span><span class="sxs-lookup"><span data-stu-id="fc80b-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="fc80b-114">高效</span><span class="sxs-lookup"><span data-stu-id="fc80b-114">high</span></span>|<span data-ttu-id="fc80b-115">1 </span><span class="sxs-lookup"><span data-stu-id="fc80b-115">1</span></span>|<span data-ttu-id="fc80b-116">High 适用于强级别的检测。</span><span class="sxs-lookup"><span data-stu-id="fc80b-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="fc80b-117">highPlus</span><span class="sxs-lookup"><span data-stu-id="fc80b-117">highPlus</span></span>|<span data-ttu-id="fc80b-118">2 </span><span class="sxs-lookup"><span data-stu-id="fc80b-118">2</span></span>|<span data-ttu-id="fc80b-119">高级别 + 使用高级别，并应用附加保护措施</span><span class="sxs-lookup"><span data-stu-id="fc80b-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="fc80b-120">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="fc80b-120">zeroTolerance</span></span>|<span data-ttu-id="fc80b-121">3 </span><span class="sxs-lookup"><span data-stu-id="fc80b-121">3</span></span>|<span data-ttu-id="fc80b-122">零耐受性阻止所有未知可执行文件</span><span class="sxs-lookup"><span data-stu-id="fc80b-122">Zero tolerance blocks all unknown executables</span></span>|




