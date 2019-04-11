---
title: win32LobAppFileSystemDetectionType 枚举类型
description: 包含所有受支持的文件系统检测类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 08783d51d6d54b0ccf2cf6d7077185e9e1c286fb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804961"
---
# <a name="win32lobappfilesystemdetectiontype-enum-type"></a><span data-ttu-id="b0d1e-103">win32LobAppFileSystemDetectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b0d1e-103">win32LobAppFileSystemDetectionType enum type</span></span>

> <span data-ttu-id="b0d1e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b0d1e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0d1e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b0d1e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0d1e-106">包含所有受支持的文件系统检测类型。</span><span class="sxs-lookup"><span data-stu-id="b0d1e-106">Contains all supported file system detection type.</span></span>

## <a name="members"></a><span data-ttu-id="b0d1e-107">成员</span><span class="sxs-lookup"><span data-stu-id="b0d1e-107">Members</span></span>
|<span data-ttu-id="b0d1e-108">成员</span><span class="sxs-lookup"><span data-stu-id="b0d1e-108">Member</span></span>|<span data-ttu-id="b0d1e-109">值</span><span class="sxs-lookup"><span data-stu-id="b0d1e-109">Value</span></span>|<span data-ttu-id="b0d1e-110">说明</span><span class="sxs-lookup"><span data-stu-id="b0d1e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0d1e-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b0d1e-111">notConfigured</span></span>|<span data-ttu-id="b0d1e-112">0</span><span class="sxs-lookup"><span data-stu-id="b0d1e-112">0</span></span>|<span data-ttu-id="b0d1e-113">未配置。</span><span class="sxs-lookup"><span data-stu-id="b0d1e-113">Not configured.</span></span>|
|<span data-ttu-id="b0d1e-114">存在</span><span class="sxs-lookup"><span data-stu-id="b0d1e-114">exists</span></span>|<span data-ttu-id="b0d1e-115">1</span><span class="sxs-lookup"><span data-stu-id="b0d1e-115">1</span></span>|<span data-ttu-id="b0d1e-116">指定的文件或文件夹是否存在。</span><span class="sxs-lookup"><span data-stu-id="b0d1e-116">Whether the specified file or folder exists.</span></span>|
|<span data-ttu-id="b0d1e-117">modifiedDate</span><span class="sxs-lookup"><span data-stu-id="b0d1e-117">modifiedDate</span></span>|<span data-ttu-id="b0d1e-118">双面</span><span class="sxs-lookup"><span data-stu-id="b0d1e-118">2</span></span>|<span data-ttu-id="b0d1e-119">上次修改日期。</span><span class="sxs-lookup"><span data-stu-id="b0d1e-119">Last modified date.</span></span>|
|<span data-ttu-id="b0d1e-120">createdDate</span><span class="sxs-lookup"><span data-stu-id="b0d1e-120">createdDate</span></span>|<span data-ttu-id="b0d1e-121">第三章</span><span class="sxs-lookup"><span data-stu-id="b0d1e-121">3</span></span>|<span data-ttu-id="b0d1e-122">创建日期。</span><span class="sxs-lookup"><span data-stu-id="b0d1e-122">Created date.</span></span>|
|<span data-ttu-id="b0d1e-123">version</span><span class="sxs-lookup"><span data-stu-id="b0d1e-123">version</span></span>|<span data-ttu-id="b0d1e-124">4</span><span class="sxs-lookup"><span data-stu-id="b0d1e-124">4</span></span>|<span data-ttu-id="b0d1e-125">版本值类型。</span><span class="sxs-lookup"><span data-stu-id="b0d1e-125">Version value type.</span></span>|
|<span data-ttu-id="b0d1e-126">sizeInMB</span><span class="sxs-lookup"><span data-stu-id="b0d1e-126">sizeInMB</span></span>|<span data-ttu-id="b0d1e-127">5</span><span class="sxs-lookup"><span data-stu-id="b0d1e-127">5</span></span>|<span data-ttu-id="b0d1e-128">大小检测类型。</span><span class="sxs-lookup"><span data-stu-id="b0d1e-128">Size detection type.</span></span>|
|<span data-ttu-id="b0d1e-129">doesNotExist</span><span class="sxs-lookup"><span data-stu-id="b0d1e-129">doesNotExist</span></span>|<span data-ttu-id="b0d1e-130">型</span><span class="sxs-lookup"><span data-stu-id="b0d1e-130">6</span></span>|<span data-ttu-id="b0d1e-131">指定的文件或文件夹不存在。</span><span class="sxs-lookup"><span data-stu-id="b0d1e-131">The specified file or folder does not exist.</span></span>|





