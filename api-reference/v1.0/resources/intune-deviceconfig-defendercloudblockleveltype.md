---
title: defenderCloudBlockLevelType 枚举类型
description: 云块级别的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 658a484a29ebed8cb111ded81ef439a560c87ac0
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366627"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="db8fa-103">defenderCloudBlockLevelType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="db8fa-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="db8fa-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="db8fa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db8fa-105">云块级别的可能值</span><span class="sxs-lookup"><span data-stu-id="db8fa-105">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="db8fa-106">成员</span><span class="sxs-lookup"><span data-stu-id="db8fa-106">Members</span></span>
|<span data-ttu-id="db8fa-107">成员</span><span class="sxs-lookup"><span data-stu-id="db8fa-107">Member</span></span>|<span data-ttu-id="db8fa-108">值</span><span class="sxs-lookup"><span data-stu-id="db8fa-108">Value</span></span>|<span data-ttu-id="db8fa-109">说明</span><span class="sxs-lookup"><span data-stu-id="db8fa-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db8fa-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="db8fa-110">notConfigured</span></span>|<span data-ttu-id="db8fa-111">0</span><span class="sxs-lookup"><span data-stu-id="db8fa-111">0</span></span>|<span data-ttu-id="db8fa-112">默认值是，使用默认的 Windows Defender 防病毒阻止级别，并提供强大的检测功能，而不会增加检测合法文件的风险</span><span class="sxs-lookup"><span data-stu-id="db8fa-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="db8fa-113">高效</span><span class="sxs-lookup"><span data-stu-id="db8fa-113">high</span></span>|<span data-ttu-id="db8fa-114">1</span><span class="sxs-lookup"><span data-stu-id="db8fa-114">1</span></span>|<span data-ttu-id="db8fa-115">High 适用于强级别的检测。</span><span class="sxs-lookup"><span data-stu-id="db8fa-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="db8fa-116">highPlus</span><span class="sxs-lookup"><span data-stu-id="db8fa-116">highPlus</span></span>|<span data-ttu-id="db8fa-117">双面</span><span class="sxs-lookup"><span data-stu-id="db8fa-117">2</span></span>|<span data-ttu-id="db8fa-118">高级别 + 使用高级别，并应用附加保护措施</span><span class="sxs-lookup"><span data-stu-id="db8fa-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="db8fa-119">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="db8fa-119">zeroTolerance</span></span>|<span data-ttu-id="db8fa-120">第三章</span><span class="sxs-lookup"><span data-stu-id="db8fa-120">3</span></span>|<span data-ttu-id="db8fa-121">零耐受性阻止所有未知可执行文件</span><span class="sxs-lookup"><span data-stu-id="db8fa-121">Zero tolerance blocks all unknown executables</span></span>|




