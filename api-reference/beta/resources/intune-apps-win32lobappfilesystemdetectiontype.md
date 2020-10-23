---
title: win32LobAppFileSystemDetectionType 枚举类型
description: 包含所有受支持的文件系统检测类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 68136da5618db38c4ac44edf2a42741867ff86f9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696410"
---
# <a name="win32lobappfilesystemdetectiontype-enum-type"></a><span data-ttu-id="19f7c-103">win32LobAppFileSystemDetectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="19f7c-103">win32LobAppFileSystemDetectionType enum type</span></span>

<span data-ttu-id="19f7c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19f7c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19f7c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="19f7c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19f7c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="19f7c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19f7c-107">包含所有受支持的文件系统检测类型。</span><span class="sxs-lookup"><span data-stu-id="19f7c-107">Contains all supported file system detection type.</span></span>

## <a name="members"></a><span data-ttu-id="19f7c-108">成员</span><span class="sxs-lookup"><span data-stu-id="19f7c-108">Members</span></span>
|<span data-ttu-id="19f7c-109">成员</span><span class="sxs-lookup"><span data-stu-id="19f7c-109">Member</span></span>|<span data-ttu-id="19f7c-110">值</span><span class="sxs-lookup"><span data-stu-id="19f7c-110">Value</span></span>|<span data-ttu-id="19f7c-111">说明</span><span class="sxs-lookup"><span data-stu-id="19f7c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19f7c-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="19f7c-112">notConfigured</span></span>|<span data-ttu-id="19f7c-113">0</span><span class="sxs-lookup"><span data-stu-id="19f7c-113">0</span></span>|<span data-ttu-id="19f7c-114">未配置。</span><span class="sxs-lookup"><span data-stu-id="19f7c-114">Not configured.</span></span>|
|<span data-ttu-id="19f7c-115">存在</span><span class="sxs-lookup"><span data-stu-id="19f7c-115">exists</span></span>|<span data-ttu-id="19f7c-116">1</span><span class="sxs-lookup"><span data-stu-id="19f7c-116">1</span></span>|<span data-ttu-id="19f7c-117">指定的文件或文件夹是否存在。</span><span class="sxs-lookup"><span data-stu-id="19f7c-117">Whether the specified file or folder exists.</span></span>|
|<span data-ttu-id="19f7c-118">modifiedDate</span><span class="sxs-lookup"><span data-stu-id="19f7c-118">modifiedDate</span></span>|<span data-ttu-id="19f7c-119">双面</span><span class="sxs-lookup"><span data-stu-id="19f7c-119">2</span></span>|<span data-ttu-id="19f7c-120">上次修改日期。</span><span class="sxs-lookup"><span data-stu-id="19f7c-120">Last modified date.</span></span>|
|<span data-ttu-id="19f7c-121">createdDate</span><span class="sxs-lookup"><span data-stu-id="19f7c-121">createdDate</span></span>|<span data-ttu-id="19f7c-122">第三章</span><span class="sxs-lookup"><span data-stu-id="19f7c-122">3</span></span>|<span data-ttu-id="19f7c-123">创建日期。</span><span class="sxs-lookup"><span data-stu-id="19f7c-123">Created date.</span></span>|
|<span data-ttu-id="19f7c-124">version</span><span class="sxs-lookup"><span data-stu-id="19f7c-124">version</span></span>|<span data-ttu-id="19f7c-125">4 </span><span class="sxs-lookup"><span data-stu-id="19f7c-125">4</span></span>|<span data-ttu-id="19f7c-126">版本值类型。</span><span class="sxs-lookup"><span data-stu-id="19f7c-126">Version value type.</span></span>|
|<span data-ttu-id="19f7c-127">sizeInMB</span><span class="sxs-lookup"><span data-stu-id="19f7c-127">sizeInMB</span></span>|<span data-ttu-id="19f7c-128">5 </span><span class="sxs-lookup"><span data-stu-id="19f7c-128">5</span></span>|<span data-ttu-id="19f7c-129">大小检测类型。</span><span class="sxs-lookup"><span data-stu-id="19f7c-129">Size detection type.</span></span>|
|<span data-ttu-id="19f7c-130">doesNotExist</span><span class="sxs-lookup"><span data-stu-id="19f7c-130">doesNotExist</span></span>|<span data-ttu-id="19f7c-131">6 </span><span class="sxs-lookup"><span data-stu-id="19f7c-131">6</span></span>|<span data-ttu-id="19f7c-132">指定的文件或文件夹不存在。</span><span class="sxs-lookup"><span data-stu-id="19f7c-132">The specified file or folder does not exist.</span></span>|





