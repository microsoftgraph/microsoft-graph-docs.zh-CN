---
title: defenderCloudBlockLevelType 枚举类型
description: 云阻止级别的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: edc8f58be9c9bfdce904988503b42e20ed2d0bfb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755887"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="12ff6-103">defenderCloudBlockLevelType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="12ff6-103">defenderCloudBlockLevelType enum type</span></span>

<span data-ttu-id="12ff6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12ff6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12ff6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12ff6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12ff6-106">云阻止级别的可能值</span><span class="sxs-lookup"><span data-stu-id="12ff6-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="12ff6-107">成员</span><span class="sxs-lookup"><span data-stu-id="12ff6-107">Members</span></span>
|<span data-ttu-id="12ff6-108">成员</span><span class="sxs-lookup"><span data-stu-id="12ff6-108">Member</span></span>|<span data-ttu-id="12ff6-109">值</span><span class="sxs-lookup"><span data-stu-id="12ff6-109">Value</span></span>|<span data-ttu-id="12ff6-110">Description</span><span class="sxs-lookup"><span data-stu-id="12ff6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12ff6-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="12ff6-111">notConfigured</span></span>|<span data-ttu-id="12ff6-112">0</span><span class="sxs-lookup"><span data-stu-id="12ff6-112">0</span></span>|<span data-ttu-id="12ff6-113">默认值，使用默认Windows Defender 防病毒阻止级别并提供强检测，而不会增加检测合法文件的风险</span><span class="sxs-lookup"><span data-stu-id="12ff6-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="12ff6-114">high</span><span class="sxs-lookup"><span data-stu-id="12ff6-114">high</span></span>|<span data-ttu-id="12ff6-115">1</span><span class="sxs-lookup"><span data-stu-id="12ff6-115">1</span></span>|<span data-ttu-id="12ff6-116">High 应用强级别的检测。</span><span class="sxs-lookup"><span data-stu-id="12ff6-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="12ff6-117">highPlus</span><span class="sxs-lookup"><span data-stu-id="12ff6-117">highPlus</span></span>|<span data-ttu-id="12ff6-118">2</span><span class="sxs-lookup"><span data-stu-id="12ff6-118">2</span></span>|<span data-ttu-id="12ff6-119">High + 使用高级别，并应用其他保护措施</span><span class="sxs-lookup"><span data-stu-id="12ff6-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="12ff6-120">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="12ff6-120">zeroTolerance</span></span>|<span data-ttu-id="12ff6-121">3</span><span class="sxs-lookup"><span data-stu-id="12ff6-121">3</span></span>|<span data-ttu-id="12ff6-122">零容限阻止所有未知可执行文件</span><span class="sxs-lookup"><span data-stu-id="12ff6-122">Zero tolerance blocks all unknown executables</span></span>|




