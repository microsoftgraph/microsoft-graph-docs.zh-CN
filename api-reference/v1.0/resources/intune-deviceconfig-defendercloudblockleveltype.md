---
title: defenderCloudBlockLevelType 枚举类型
description: 云块级别的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de81e42827f7c153fc81e7fc19d85e54cb780bfa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575182"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="ae26b-103">defenderCloudBlockLevelType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ae26b-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="ae26b-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ae26b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae26b-105">云块级别的可能值</span><span class="sxs-lookup"><span data-stu-id="ae26b-105">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="ae26b-106">成员</span><span class="sxs-lookup"><span data-stu-id="ae26b-106">Members</span></span>
|<span data-ttu-id="ae26b-107">成员</span><span class="sxs-lookup"><span data-stu-id="ae26b-107">Member</span></span>|<span data-ttu-id="ae26b-108">值</span><span class="sxs-lookup"><span data-stu-id="ae26b-108">Value</span></span>|<span data-ttu-id="ae26b-109">说明</span><span class="sxs-lookup"><span data-stu-id="ae26b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae26b-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ae26b-110">notConfigured</span></span>|<span data-ttu-id="ae26b-111">0</span><span class="sxs-lookup"><span data-stu-id="ae26b-111">0</span></span>|<span data-ttu-id="ae26b-112">默认值是, 使用默认的 Windows Defender 防病毒阻止级别, 并提供强大的检测功能, 而不会增加检测合法文件的风险</span><span class="sxs-lookup"><span data-stu-id="ae26b-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="ae26b-113">高效</span><span class="sxs-lookup"><span data-stu-id="ae26b-113">high</span></span>|<span data-ttu-id="ae26b-114">1</span><span class="sxs-lookup"><span data-stu-id="ae26b-114">1</span></span>|<span data-ttu-id="ae26b-115">High 适用于强级别的检测。</span><span class="sxs-lookup"><span data-stu-id="ae26b-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="ae26b-116">highPlus</span><span class="sxs-lookup"><span data-stu-id="ae26b-116">highPlus</span></span>|<span data-ttu-id="ae26b-117">2 </span><span class="sxs-lookup"><span data-stu-id="ae26b-117">2</span></span>|<span data-ttu-id="ae26b-118">高级别 + 使用高级别, 并应用附加保护措施</span><span class="sxs-lookup"><span data-stu-id="ae26b-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="ae26b-119">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="ae26b-119">zeroTolerance</span></span>|<span data-ttu-id="ae26b-120">3 </span><span class="sxs-lookup"><span data-stu-id="ae26b-120">3</span></span>|<span data-ttu-id="ae26b-121">零耐受性阻止所有未知可执行文件</span><span class="sxs-lookup"><span data-stu-id="ae26b-121">Zero tolerance blocks all unknown executables</span></span>|



