---
title: folderProtectionType 枚举类型
description: 可能的值的文件夹保护
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e2abbb719ab93b53ad276f8391d4028c4f8b40b4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405714"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="bd0ee-103">folderProtectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="bd0ee-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="bd0ee-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="bd0ee-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bd0ee-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bd0ee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd0ee-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bd0ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd0ee-107">可能的值的文件夹保护</span><span class="sxs-lookup"><span data-stu-id="bd0ee-107">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="bd0ee-108">成员</span><span class="sxs-lookup"><span data-stu-id="bd0ee-108">Members</span></span>
|<span data-ttu-id="bd0ee-109">成员</span><span class="sxs-lookup"><span data-stu-id="bd0ee-109">Member</span></span>|<span data-ttu-id="bd0ee-110">值</span><span class="sxs-lookup"><span data-stu-id="bd0ee-110">Value</span></span>|<span data-ttu-id="bd0ee-111">说明</span><span class="sxs-lookup"><span data-stu-id="bd0ee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd0ee-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="bd0ee-112">userDefined</span></span>|<span data-ttu-id="bd0ee-113">0</span><span class="sxs-lookup"><span data-stu-id="bd0ee-113">0</span></span>|<span data-ttu-id="bd0ee-114">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="bd0ee-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="bd0ee-115">启用</span><span class="sxs-lookup"><span data-stu-id="bd0ee-115">enable</span></span>|<span data-ttu-id="bd0ee-116">1</span><span class="sxs-lookup"><span data-stu-id="bd0ee-116">1</span></span>|<span data-ttu-id="bd0ee-117">阻止功能。</span><span class="sxs-lookup"><span data-stu-id="bd0ee-117">Block functionality.</span></span>|
|<span data-ttu-id="bd0ee-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="bd0ee-118">auditMode</span></span>|<span data-ttu-id="bd0ee-119">2</span><span class="sxs-lookup"><span data-stu-id="bd0ee-119">2</span></span>|<span data-ttu-id="bd0ee-120">允许功能，但生成日志。</span><span class="sxs-lookup"><span data-stu-id="bd0ee-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="bd0ee-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="bd0ee-121">blockDiskModification</span></span>|<span data-ttu-id="bd0ee-122">3</span><span class="sxs-lookup"><span data-stu-id="bd0ee-122">3</span></span>|<span data-ttu-id="bd0ee-123">阻止来自写入磁盘扇区的不受信任应用程序。</span><span class="sxs-lookup"><span data-stu-id="bd0ee-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="bd0ee-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="bd0ee-124">auditDiskModification</span></span>|<span data-ttu-id="bd0ee-125">4</span><span class="sxs-lookup"><span data-stu-id="bd0ee-125">4</span></span>|<span data-ttu-id="bd0ee-126">时不受信任应用程序写入磁盘扇区生成日志。</span><span class="sxs-lookup"><span data-stu-id="bd0ee-126">Generate logs when untrusted apps write to disk sectors.</span></span>|




