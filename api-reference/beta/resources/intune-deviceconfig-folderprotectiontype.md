---
title: folderProtectionType 枚举类型
description: 文件夹保护的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 23717d1e798059f1ca025a3f80279804b616b17f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529985"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="947c7-103">folderProtectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="947c7-103">folderProtectionType enum type</span></span>

<span data-ttu-id="947c7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="947c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="947c7-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="947c7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="947c7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="947c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="947c7-107">文件夹保护的可能值</span><span class="sxs-lookup"><span data-stu-id="947c7-107">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="947c7-108">成员</span><span class="sxs-lookup"><span data-stu-id="947c7-108">Members</span></span>
|<span data-ttu-id="947c7-109">成员</span><span class="sxs-lookup"><span data-stu-id="947c7-109">Member</span></span>|<span data-ttu-id="947c7-110">值</span><span class="sxs-lookup"><span data-stu-id="947c7-110">Value</span></span>|<span data-ttu-id="947c7-111">说明</span><span class="sxs-lookup"><span data-stu-id="947c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="947c7-112">定制</span><span class="sxs-lookup"><span data-stu-id="947c7-112">userDefined</span></span>|<span data-ttu-id="947c7-113">0</span><span class="sxs-lookup"><span data-stu-id="947c7-113">0</span></span>|<span data-ttu-id="947c7-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="947c7-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="947c7-115">启用</span><span class="sxs-lookup"><span data-stu-id="947c7-115">enable</span></span>|<span data-ttu-id="947c7-116">1 </span><span class="sxs-lookup"><span data-stu-id="947c7-116">1</span></span>|<span data-ttu-id="947c7-117">阻止功能。</span><span class="sxs-lookup"><span data-stu-id="947c7-117">Block functionality.</span></span>|
|<span data-ttu-id="947c7-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="947c7-118">auditMode</span></span>|<span data-ttu-id="947c7-119">2 </span><span class="sxs-lookup"><span data-stu-id="947c7-119">2</span></span>|<span data-ttu-id="947c7-120">允许功能，但生成日志。</span><span class="sxs-lookup"><span data-stu-id="947c7-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="947c7-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="947c7-121">blockDiskModification</span></span>|<span data-ttu-id="947c7-122">3 </span><span class="sxs-lookup"><span data-stu-id="947c7-122">3</span></span>|<span data-ttu-id="947c7-123">阻止不受信任的应用写入磁盘扇区。</span><span class="sxs-lookup"><span data-stu-id="947c7-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="947c7-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="947c7-124">auditDiskModification</span></span>|<span data-ttu-id="947c7-125">4 </span><span class="sxs-lookup"><span data-stu-id="947c7-125">4</span></span>|<span data-ttu-id="947c7-126">在不受信任的应用写入磁盘扇区时生成日志。</span><span class="sxs-lookup"><span data-stu-id="947c7-126">Generate logs when untrusted apps write to disk sectors.</span></span>|



