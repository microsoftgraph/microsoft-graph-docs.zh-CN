---
title: defenderCloudBlockLevelType 枚举类型
description: 云块级别的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3afc9a0bdf5d25c4496cb2dcf4a7ef013ac0785d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795619"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="74a0a-103">defenderCloudBlockLevelType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="74a0a-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="74a0a-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="74a0a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74a0a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="74a0a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74a0a-106">云块级别的可能值</span><span class="sxs-lookup"><span data-stu-id="74a0a-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="74a0a-107">成员</span><span class="sxs-lookup"><span data-stu-id="74a0a-107">Members</span></span>
|<span data-ttu-id="74a0a-108">成员</span><span class="sxs-lookup"><span data-stu-id="74a0a-108">Member</span></span>|<span data-ttu-id="74a0a-109">值</span><span class="sxs-lookup"><span data-stu-id="74a0a-109">Value</span></span>|<span data-ttu-id="74a0a-110">说明</span><span class="sxs-lookup"><span data-stu-id="74a0a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74a0a-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="74a0a-111">notConfigured</span></span>|<span data-ttu-id="74a0a-112">0</span><span class="sxs-lookup"><span data-stu-id="74a0a-112">0</span></span>|<span data-ttu-id="74a0a-113">默认值是，使用默认的 Windows Defender 防病毒阻止级别，并提供强大的检测功能，而不会增加检测合法文件的风险</span><span class="sxs-lookup"><span data-stu-id="74a0a-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="74a0a-114">高效</span><span class="sxs-lookup"><span data-stu-id="74a0a-114">high</span></span>|<span data-ttu-id="74a0a-115">1</span><span class="sxs-lookup"><span data-stu-id="74a0a-115">1</span></span>|<span data-ttu-id="74a0a-116">High 适用于强级别的检测。</span><span class="sxs-lookup"><span data-stu-id="74a0a-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="74a0a-117">highPlus</span><span class="sxs-lookup"><span data-stu-id="74a0a-117">highPlus</span></span>|<span data-ttu-id="74a0a-118">双面</span><span class="sxs-lookup"><span data-stu-id="74a0a-118">2</span></span>|<span data-ttu-id="74a0a-119">高级别 + 使用高级别，并应用附加保护措施</span><span class="sxs-lookup"><span data-stu-id="74a0a-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="74a0a-120">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="74a0a-120">zeroTolerance</span></span>|<span data-ttu-id="74a0a-121">第三章</span><span class="sxs-lookup"><span data-stu-id="74a0a-121">3</span></span>|<span data-ttu-id="74a0a-122">零耐受性阻止所有未知可执行文件</span><span class="sxs-lookup"><span data-stu-id="74a0a-122">Zero tolerance blocks all unknown executables</span></span>|



