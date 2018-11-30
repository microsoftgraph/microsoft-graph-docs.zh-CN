---
title: folderProtectionType 枚举类型
description: 可能的值的文件夹保护
ms.openlocfilehash: a02f1602f8b9a962124fb7bf2a9731662a6f3057
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044352"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="1cebb-103">folderProtectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1cebb-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="1cebb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1cebb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1cebb-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1cebb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1cebb-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1cebb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1cebb-107">可能的值的文件夹保护</span><span class="sxs-lookup"><span data-stu-id="1cebb-107">Possible values of Folder Protection</span></span>
## <a name="members"></a><span data-ttu-id="1cebb-108">成员</span><span class="sxs-lookup"><span data-stu-id="1cebb-108">Members</span></span>
|<span data-ttu-id="1cebb-109">成员</span><span class="sxs-lookup"><span data-stu-id="1cebb-109">Member</span></span>|<span data-ttu-id="1cebb-110">值</span><span class="sxs-lookup"><span data-stu-id="1cebb-110">Value</span></span>|<span data-ttu-id="1cebb-111">说明</span><span class="sxs-lookup"><span data-stu-id="1cebb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cebb-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="1cebb-112">userDefined</span></span>|<span data-ttu-id="1cebb-113">0</span><span class="sxs-lookup"><span data-stu-id="1cebb-113">0</span></span>|<span data-ttu-id="1cebb-114">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="1cebb-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="1cebb-115">启用</span><span class="sxs-lookup"><span data-stu-id="1cebb-115">enable</span></span>|<span data-ttu-id="1cebb-116">1</span><span class="sxs-lookup"><span data-stu-id="1cebb-116">1</span></span>|<span data-ttu-id="1cebb-117">阻止功能。</span><span class="sxs-lookup"><span data-stu-id="1cebb-117">Block functionality.</span></span>|
|<span data-ttu-id="1cebb-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="1cebb-118">auditMode</span></span>|<span data-ttu-id="1cebb-119">2</span><span class="sxs-lookup"><span data-stu-id="1cebb-119">2</span></span>|<span data-ttu-id="1cebb-120">允许功能，但生成日志。</span><span class="sxs-lookup"><span data-stu-id="1cebb-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="1cebb-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="1cebb-121">blockDiskModification</span></span>|<span data-ttu-id="1cebb-122">3</span><span class="sxs-lookup"><span data-stu-id="1cebb-122">3</span></span>|<span data-ttu-id="1cebb-123">阻止来自写入磁盘扇区的不受信任应用程序。</span><span class="sxs-lookup"><span data-stu-id="1cebb-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="1cebb-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="1cebb-124">auditDiskModification</span></span>|<span data-ttu-id="1cebb-125">4</span><span class="sxs-lookup"><span data-stu-id="1cebb-125">4</span></span>|<span data-ttu-id="1cebb-126">时不受信任应用程序写入磁盘扇区生成日志。</span><span class="sxs-lookup"><span data-stu-id="1cebb-126">Generate logs when untrusted apps write to disk sectors.</span></span>|





