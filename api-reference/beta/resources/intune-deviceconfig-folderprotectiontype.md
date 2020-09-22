---
title: folderProtectionType 枚举类型
description: 文件夹保护的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9ccdaf6625685a0e9e317ad01c8b81fffa04f651
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994069"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="bc5bf-103">folderProtectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="bc5bf-103">folderProtectionType enum type</span></span>

<span data-ttu-id="bc5bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc5bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc5bf-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bc5bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc5bf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bc5bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc5bf-107">文件夹保护的可能值</span><span class="sxs-lookup"><span data-stu-id="bc5bf-107">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="bc5bf-108">成员</span><span class="sxs-lookup"><span data-stu-id="bc5bf-108">Members</span></span>
|<span data-ttu-id="bc5bf-109">成员</span><span class="sxs-lookup"><span data-stu-id="bc5bf-109">Member</span></span>|<span data-ttu-id="bc5bf-110">值</span><span class="sxs-lookup"><span data-stu-id="bc5bf-110">Value</span></span>|<span data-ttu-id="bc5bf-111">说明</span><span class="sxs-lookup"><span data-stu-id="bc5bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc5bf-112">定制</span><span class="sxs-lookup"><span data-stu-id="bc5bf-112">userDefined</span></span>|<span data-ttu-id="bc5bf-113">0</span><span class="sxs-lookup"><span data-stu-id="bc5bf-113">0</span></span>|<span data-ttu-id="bc5bf-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="bc5bf-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="bc5bf-115">启用</span><span class="sxs-lookup"><span data-stu-id="bc5bf-115">enable</span></span>|<span data-ttu-id="bc5bf-116">1 </span><span class="sxs-lookup"><span data-stu-id="bc5bf-116">1</span></span>|<span data-ttu-id="bc5bf-117">阻止功能。</span><span class="sxs-lookup"><span data-stu-id="bc5bf-117">Block functionality.</span></span>|
|<span data-ttu-id="bc5bf-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="bc5bf-118">auditMode</span></span>|<span data-ttu-id="bc5bf-119">2 </span><span class="sxs-lookup"><span data-stu-id="bc5bf-119">2</span></span>|<span data-ttu-id="bc5bf-120">允许功能，但生成日志。</span><span class="sxs-lookup"><span data-stu-id="bc5bf-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="bc5bf-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="bc5bf-121">blockDiskModification</span></span>|<span data-ttu-id="bc5bf-122">第三章</span><span class="sxs-lookup"><span data-stu-id="bc5bf-122">3</span></span>|<span data-ttu-id="bc5bf-123">阻止不受信任的应用写入磁盘扇区。</span><span class="sxs-lookup"><span data-stu-id="bc5bf-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="bc5bf-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="bc5bf-124">auditDiskModification</span></span>|<span data-ttu-id="bc5bf-125">4 </span><span class="sxs-lookup"><span data-stu-id="bc5bf-125">4</span></span>|<span data-ttu-id="bc5bf-126">在不受信任的应用写入磁盘扇区时生成日志。</span><span class="sxs-lookup"><span data-stu-id="bc5bf-126">Generate logs when untrusted apps write to disk sectors.</span></span>|






