---
title: defenderCloudBlockLevelType 枚举类型
description: 云块级别的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5bdc4730684afb7856df0a29210b37f78bdb7ca1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042483"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="81680-103">defenderCloudBlockLevelType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="81680-103">defenderCloudBlockLevelType enum type</span></span>

<span data-ttu-id="81680-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81680-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81680-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="81680-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81680-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="81680-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81680-107">云块级别的可能值</span><span class="sxs-lookup"><span data-stu-id="81680-107">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="81680-108">成员</span><span class="sxs-lookup"><span data-stu-id="81680-108">Members</span></span>
|<span data-ttu-id="81680-109">成员</span><span class="sxs-lookup"><span data-stu-id="81680-109">Member</span></span>|<span data-ttu-id="81680-110">值</span><span class="sxs-lookup"><span data-stu-id="81680-110">Value</span></span>|<span data-ttu-id="81680-111">说明</span><span class="sxs-lookup"><span data-stu-id="81680-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81680-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="81680-112">notConfigured</span></span>|<span data-ttu-id="81680-113">0</span><span class="sxs-lookup"><span data-stu-id="81680-113">0</span></span>|<span data-ttu-id="81680-114">默认值是，使用默认的 Windows Defender 防病毒阻止级别，并提供强大的检测功能，而不会增加检测合法文件的风险</span><span class="sxs-lookup"><span data-stu-id="81680-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="81680-115">高效</span><span class="sxs-lookup"><span data-stu-id="81680-115">high</span></span>|<span data-ttu-id="81680-116">1 </span><span class="sxs-lookup"><span data-stu-id="81680-116">1</span></span>|<span data-ttu-id="81680-117">High 适用于强级别的检测。</span><span class="sxs-lookup"><span data-stu-id="81680-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="81680-118">highPlus</span><span class="sxs-lookup"><span data-stu-id="81680-118">highPlus</span></span>|<span data-ttu-id="81680-119">2 </span><span class="sxs-lookup"><span data-stu-id="81680-119">2</span></span>|<span data-ttu-id="81680-120">高级别 + 使用高级别，并应用附加保护措施</span><span class="sxs-lookup"><span data-stu-id="81680-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="81680-121">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="81680-121">zeroTolerance</span></span>|<span data-ttu-id="81680-122">第三章</span><span class="sxs-lookup"><span data-stu-id="81680-122">3</span></span>|<span data-ttu-id="81680-123">零耐受性阻止所有未知可执行文件</span><span class="sxs-lookup"><span data-stu-id="81680-123">Zero tolerance blocks all unknown executables</span></span>|






