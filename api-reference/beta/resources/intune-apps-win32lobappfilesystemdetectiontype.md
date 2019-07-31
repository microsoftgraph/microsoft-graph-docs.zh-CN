---
title: win32LobAppFileSystemDetectionType 枚举类型
description: 包含所有受支持的文件系统检测类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e77e1a588946ca3a69a993fb561c1b48602602f2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004972"
---
# <a name="win32lobappfilesystemdetectiontype-enum-type"></a><span data-ttu-id="d3d7f-103">win32LobAppFileSystemDetectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d3d7f-103">win32LobAppFileSystemDetectionType enum type</span></span>

> <span data-ttu-id="d3d7f-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d3d7f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3d7f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3d7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3d7f-106">包含所有受支持的文件系统检测类型。</span><span class="sxs-lookup"><span data-stu-id="d3d7f-106">Contains all supported file system detection type.</span></span>

## <a name="members"></a><span data-ttu-id="d3d7f-107">成员</span><span class="sxs-lookup"><span data-stu-id="d3d7f-107">Members</span></span>
|<span data-ttu-id="d3d7f-108">成员</span><span class="sxs-lookup"><span data-stu-id="d3d7f-108">Member</span></span>|<span data-ttu-id="d3d7f-109">值</span><span class="sxs-lookup"><span data-stu-id="d3d7f-109">Value</span></span>|<span data-ttu-id="d3d7f-110">说明</span><span class="sxs-lookup"><span data-stu-id="d3d7f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3d7f-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d3d7f-111">notConfigured</span></span>|<span data-ttu-id="d3d7f-112">0</span><span class="sxs-lookup"><span data-stu-id="d3d7f-112">0</span></span>|<span data-ttu-id="d3d7f-113">未配置。</span><span class="sxs-lookup"><span data-stu-id="d3d7f-113">Not configured.</span></span>|
|<span data-ttu-id="d3d7f-114">存在</span><span class="sxs-lookup"><span data-stu-id="d3d7f-114">exists</span></span>|<span data-ttu-id="d3d7f-115">1</span><span class="sxs-lookup"><span data-stu-id="d3d7f-115">1</span></span>|<span data-ttu-id="d3d7f-116">指定的文件或文件夹是否存在。</span><span class="sxs-lookup"><span data-stu-id="d3d7f-116">Whether the specified file or folder exists.</span></span>|
|<span data-ttu-id="d3d7f-117">modifiedDate</span><span class="sxs-lookup"><span data-stu-id="d3d7f-117">modifiedDate</span></span>|<span data-ttu-id="d3d7f-118">双面</span><span class="sxs-lookup"><span data-stu-id="d3d7f-118">2</span></span>|<span data-ttu-id="d3d7f-119">上次修改日期。</span><span class="sxs-lookup"><span data-stu-id="d3d7f-119">Last modified date.</span></span>|
|<span data-ttu-id="d3d7f-120">createdDate</span><span class="sxs-lookup"><span data-stu-id="d3d7f-120">createdDate</span></span>|<span data-ttu-id="d3d7f-121">第三章</span><span class="sxs-lookup"><span data-stu-id="d3d7f-121">3</span></span>|<span data-ttu-id="d3d7f-122">创建日期。</span><span class="sxs-lookup"><span data-stu-id="d3d7f-122">Created date.</span></span>|
|<span data-ttu-id="d3d7f-123">version</span><span class="sxs-lookup"><span data-stu-id="d3d7f-123">version</span></span>|<span data-ttu-id="d3d7f-124">4</span><span class="sxs-lookup"><span data-stu-id="d3d7f-124">4</span></span>|<span data-ttu-id="d3d7f-125">版本值类型。</span><span class="sxs-lookup"><span data-stu-id="d3d7f-125">Version value type.</span></span>|
|<span data-ttu-id="d3d7f-126">sizeInMB</span><span class="sxs-lookup"><span data-stu-id="d3d7f-126">sizeInMB</span></span>|<span data-ttu-id="d3d7f-127">5</span><span class="sxs-lookup"><span data-stu-id="d3d7f-127">5</span></span>|<span data-ttu-id="d3d7f-128">大小检测类型。</span><span class="sxs-lookup"><span data-stu-id="d3d7f-128">Size detection type.</span></span>|
|<span data-ttu-id="d3d7f-129">doesNotExist</span><span class="sxs-lookup"><span data-stu-id="d3d7f-129">doesNotExist</span></span>|<span data-ttu-id="d3d7f-130">型</span><span class="sxs-lookup"><span data-stu-id="d3d7f-130">6</span></span>|<span data-ttu-id="d3d7f-131">指定的文件或文件夹不存在。</span><span class="sxs-lookup"><span data-stu-id="d3d7f-131">The specified file or folder does not exist.</span></span>|





