---
title: folderProtectionType 枚举类型
description: 文件夹保护的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0682f5bfbef65b982762e10a9425a8381d645d7d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170334"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="d6bdc-103">folderProtectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d6bdc-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="d6bdc-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d6bdc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6bdc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d6bdc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6bdc-106">文件夹保护的可能值</span><span class="sxs-lookup"><span data-stu-id="d6bdc-106">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="d6bdc-107">成员</span><span class="sxs-lookup"><span data-stu-id="d6bdc-107">Members</span></span>
|<span data-ttu-id="d6bdc-108">成员</span><span class="sxs-lookup"><span data-stu-id="d6bdc-108">Member</span></span>|<span data-ttu-id="d6bdc-109">值</span><span class="sxs-lookup"><span data-stu-id="d6bdc-109">Value</span></span>|<span data-ttu-id="d6bdc-110">说明</span><span class="sxs-lookup"><span data-stu-id="d6bdc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6bdc-111">定制</span><span class="sxs-lookup"><span data-stu-id="d6bdc-111">userDefined</span></span>|<span data-ttu-id="d6bdc-112">0</span><span class="sxs-lookup"><span data-stu-id="d6bdc-112">0</span></span>|<span data-ttu-id="d6bdc-113">设备默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="d6bdc-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="d6bdc-114">启用</span><span class="sxs-lookup"><span data-stu-id="d6bdc-114">enable</span></span>|<span data-ttu-id="d6bdc-115">1</span><span class="sxs-lookup"><span data-stu-id="d6bdc-115">1</span></span>|<span data-ttu-id="d6bdc-116">阻止功能。</span><span class="sxs-lookup"><span data-stu-id="d6bdc-116">Block functionality.</span></span>|
|<span data-ttu-id="d6bdc-117">auditMode</span><span class="sxs-lookup"><span data-stu-id="d6bdc-117">auditMode</span></span>|<span data-ttu-id="d6bdc-118">双面</span><span class="sxs-lookup"><span data-stu-id="d6bdc-118">2</span></span>|<span data-ttu-id="d6bdc-119">允许功能, 但生成日志。</span><span class="sxs-lookup"><span data-stu-id="d6bdc-119">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="d6bdc-120">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="d6bdc-120">blockDiskModification</span></span>|<span data-ttu-id="d6bdc-121">第三章</span><span class="sxs-lookup"><span data-stu-id="d6bdc-121">3</span></span>|<span data-ttu-id="d6bdc-122">阻止不受信任的应用写入磁盘扇区。</span><span class="sxs-lookup"><span data-stu-id="d6bdc-122">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="d6bdc-123">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="d6bdc-123">auditDiskModification</span></span>|<span data-ttu-id="d6bdc-124">4</span><span class="sxs-lookup"><span data-stu-id="d6bdc-124">4</span></span>|<span data-ttu-id="d6bdc-125">在不受信任的应用写入磁盘扇区时生成日志。</span><span class="sxs-lookup"><span data-stu-id="d6bdc-125">Generate logs when untrusted apps write to disk sectors.</span></span>|




