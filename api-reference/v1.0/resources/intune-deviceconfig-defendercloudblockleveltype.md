---
title: defenderCloudBlockLevelType 枚举类型
description: 云块级别的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8fd63865369371a32a1bda0b2a7438fc851256a3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069020"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="5e58c-103">defenderCloudBlockLevelType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5e58c-103">defenderCloudBlockLevelType enum type</span></span>

<span data-ttu-id="5e58c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e58c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e58c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e58c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e58c-106">云块级别的可能值</span><span class="sxs-lookup"><span data-stu-id="5e58c-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="5e58c-107">成员</span><span class="sxs-lookup"><span data-stu-id="5e58c-107">Members</span></span>
|<span data-ttu-id="5e58c-108">成员</span><span class="sxs-lookup"><span data-stu-id="5e58c-108">Member</span></span>|<span data-ttu-id="5e58c-109">值</span><span class="sxs-lookup"><span data-stu-id="5e58c-109">Value</span></span>|<span data-ttu-id="5e58c-110">说明</span><span class="sxs-lookup"><span data-stu-id="5e58c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e58c-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="5e58c-111">notConfigured</span></span>|<span data-ttu-id="5e58c-112">0</span><span class="sxs-lookup"><span data-stu-id="5e58c-112">0</span></span>|<span data-ttu-id="5e58c-113">默认值是，使用默认的 Windows Defender 防病毒阻止级别，并提供强大的检测功能，而不会增加检测合法文件的风险</span><span class="sxs-lookup"><span data-stu-id="5e58c-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="5e58c-114">高效</span><span class="sxs-lookup"><span data-stu-id="5e58c-114">high</span></span>|<span data-ttu-id="5e58c-115">1 </span><span class="sxs-lookup"><span data-stu-id="5e58c-115">1</span></span>|<span data-ttu-id="5e58c-116">High 适用于强级别的检测。</span><span class="sxs-lookup"><span data-stu-id="5e58c-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="5e58c-117">highPlus</span><span class="sxs-lookup"><span data-stu-id="5e58c-117">highPlus</span></span>|<span data-ttu-id="5e58c-118">2 </span><span class="sxs-lookup"><span data-stu-id="5e58c-118">2</span></span>|<span data-ttu-id="5e58c-119">高级别 + 使用高级别，并应用附加保护措施</span><span class="sxs-lookup"><span data-stu-id="5e58c-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="5e58c-120">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="5e58c-120">zeroTolerance</span></span>|<span data-ttu-id="5e58c-121">第三章</span><span class="sxs-lookup"><span data-stu-id="5e58c-121">3</span></span>|<span data-ttu-id="5e58c-122">零耐受性阻止所有未知可执行文件</span><span class="sxs-lookup"><span data-stu-id="5e58c-122">Zero tolerance blocks all unknown executables</span></span>|









