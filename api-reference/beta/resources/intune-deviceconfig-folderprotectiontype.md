---
title: folderProtectionType 枚举类型
description: 可能的值的文件夹保护
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 435f3ea01f5a8ffc3c4cb54034d415d54732db5d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826129"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="89b93-103">folderProtectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="89b93-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="89b93-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="89b93-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89b93-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="89b93-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="89b93-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="89b93-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89b93-107">可能的值的文件夹保护</span><span class="sxs-lookup"><span data-stu-id="89b93-107">Possible values of Folder Protection</span></span>
## <a name="members"></a><span data-ttu-id="89b93-108">成员</span><span class="sxs-lookup"><span data-stu-id="89b93-108">Members</span></span>
|<span data-ttu-id="89b93-109">成员</span><span class="sxs-lookup"><span data-stu-id="89b93-109">Member</span></span>|<span data-ttu-id="89b93-110">值</span><span class="sxs-lookup"><span data-stu-id="89b93-110">Value</span></span>|<span data-ttu-id="89b93-111">Description</span><span class="sxs-lookup"><span data-stu-id="89b93-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89b93-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="89b93-112">userDefined</span></span>|<span data-ttu-id="89b93-113">0</span><span class="sxs-lookup"><span data-stu-id="89b93-113">0</span></span>|<span data-ttu-id="89b93-114">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="89b93-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="89b93-115">启用</span><span class="sxs-lookup"><span data-stu-id="89b93-115">enable</span></span>|<span data-ttu-id="89b93-116">1</span><span class="sxs-lookup"><span data-stu-id="89b93-116">1</span></span>|<span data-ttu-id="89b93-117">阻止功能。</span><span class="sxs-lookup"><span data-stu-id="89b93-117">Block functionality.</span></span>|
|<span data-ttu-id="89b93-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="89b93-118">auditMode</span></span>|<span data-ttu-id="89b93-119">2</span><span class="sxs-lookup"><span data-stu-id="89b93-119">2</span></span>|<span data-ttu-id="89b93-120">允许功能，但生成日志。</span><span class="sxs-lookup"><span data-stu-id="89b93-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="89b93-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="89b93-121">blockDiskModification</span></span>|<span data-ttu-id="89b93-122">3</span><span class="sxs-lookup"><span data-stu-id="89b93-122">3</span></span>|<span data-ttu-id="89b93-123">阻止来自写入磁盘扇区的不受信任应用程序。</span><span class="sxs-lookup"><span data-stu-id="89b93-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="89b93-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="89b93-124">auditDiskModification</span></span>|<span data-ttu-id="89b93-125">4</span><span class="sxs-lookup"><span data-stu-id="89b93-125">4</span></span>|<span data-ttu-id="89b93-126">时不受信任应用程序写入磁盘扇区生成日志。</span><span class="sxs-lookup"><span data-stu-id="89b93-126">Generate logs when untrusted apps write to disk sectors.</span></span>|





