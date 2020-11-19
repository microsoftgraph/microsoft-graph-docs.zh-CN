---
title: defenderCloudBlockLevelType 枚举类型
description: 云块级别的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7760fa978f6b25eb9a0a176b237d2595cc682e9c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256657"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="dab20-103">defenderCloudBlockLevelType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="dab20-103">defenderCloudBlockLevelType enum type</span></span>

<span data-ttu-id="dab20-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dab20-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dab20-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dab20-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dab20-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dab20-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dab20-107">云块级别的可能值</span><span class="sxs-lookup"><span data-stu-id="dab20-107">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="dab20-108">成员</span><span class="sxs-lookup"><span data-stu-id="dab20-108">Members</span></span>
|<span data-ttu-id="dab20-109">成员</span><span class="sxs-lookup"><span data-stu-id="dab20-109">Member</span></span>|<span data-ttu-id="dab20-110">值</span><span class="sxs-lookup"><span data-stu-id="dab20-110">Value</span></span>|<span data-ttu-id="dab20-111">说明</span><span class="sxs-lookup"><span data-stu-id="dab20-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dab20-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="dab20-112">notConfigured</span></span>|<span data-ttu-id="dab20-113">0</span><span class="sxs-lookup"><span data-stu-id="dab20-113">0</span></span>|<span data-ttu-id="dab20-114">默认值是，使用默认的 Windows Defender 防病毒阻止级别，并提供强大的检测功能，而不会增加检测合法文件的风险</span><span class="sxs-lookup"><span data-stu-id="dab20-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="dab20-115">高效</span><span class="sxs-lookup"><span data-stu-id="dab20-115">high</span></span>|<span data-ttu-id="dab20-116">1</span><span class="sxs-lookup"><span data-stu-id="dab20-116">1</span></span>|<span data-ttu-id="dab20-117">High 适用于强级别的检测。</span><span class="sxs-lookup"><span data-stu-id="dab20-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="dab20-118">highPlus</span><span class="sxs-lookup"><span data-stu-id="dab20-118">highPlus</span></span>|<span data-ttu-id="dab20-119">双面</span><span class="sxs-lookup"><span data-stu-id="dab20-119">2</span></span>|<span data-ttu-id="dab20-120">高级别 + 使用高级别，并应用附加保护措施</span><span class="sxs-lookup"><span data-stu-id="dab20-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="dab20-121">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="dab20-121">zeroTolerance</span></span>|<span data-ttu-id="dab20-122">第三章</span><span class="sxs-lookup"><span data-stu-id="dab20-122">3</span></span>|<span data-ttu-id="dab20-123">零耐受性阻止所有未知可执行文件</span><span class="sxs-lookup"><span data-stu-id="dab20-123">Zero tolerance blocks all unknown executables</span></span>|




