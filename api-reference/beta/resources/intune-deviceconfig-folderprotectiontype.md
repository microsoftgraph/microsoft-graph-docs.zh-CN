---
title: folderProtectionType 枚举类型
description: 可能的值的文件夹保护
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 427bdb4fcb93a831ab120aa0c7eefcbf97675fa8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973748"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="55fc7-103">folderProtectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="55fc7-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="55fc7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="55fc7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55fc7-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="55fc7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="55fc7-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="55fc7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55fc7-107">可能的值的文件夹保护</span><span class="sxs-lookup"><span data-stu-id="55fc7-107">Possible values of Folder Protection</span></span>
## <a name="members"></a><span data-ttu-id="55fc7-108">成员</span><span class="sxs-lookup"><span data-stu-id="55fc7-108">Members</span></span>
|<span data-ttu-id="55fc7-109">成员</span><span class="sxs-lookup"><span data-stu-id="55fc7-109">Member</span></span>|<span data-ttu-id="55fc7-110">值</span><span class="sxs-lookup"><span data-stu-id="55fc7-110">Value</span></span>|<span data-ttu-id="55fc7-111">说明</span><span class="sxs-lookup"><span data-stu-id="55fc7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55fc7-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="55fc7-112">userDefined</span></span>|<span data-ttu-id="55fc7-113">0</span><span class="sxs-lookup"><span data-stu-id="55fc7-113">0</span></span>|<span data-ttu-id="55fc7-114">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="55fc7-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="55fc7-115">启用</span><span class="sxs-lookup"><span data-stu-id="55fc7-115">enable</span></span>|<span data-ttu-id="55fc7-116">1</span><span class="sxs-lookup"><span data-stu-id="55fc7-116">1</span></span>|<span data-ttu-id="55fc7-117">阻止功能。</span><span class="sxs-lookup"><span data-stu-id="55fc7-117">Block functionality.</span></span>|
|<span data-ttu-id="55fc7-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="55fc7-118">auditMode</span></span>|<span data-ttu-id="55fc7-119">2</span><span class="sxs-lookup"><span data-stu-id="55fc7-119">2</span></span>|<span data-ttu-id="55fc7-120">允许功能，但生成日志。</span><span class="sxs-lookup"><span data-stu-id="55fc7-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="55fc7-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="55fc7-121">blockDiskModification</span></span>|<span data-ttu-id="55fc7-122">3</span><span class="sxs-lookup"><span data-stu-id="55fc7-122">3</span></span>|<span data-ttu-id="55fc7-123">阻止来自写入磁盘扇区的不受信任应用程序。</span><span class="sxs-lookup"><span data-stu-id="55fc7-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="55fc7-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="55fc7-124">auditDiskModification</span></span>|<span data-ttu-id="55fc7-125">4</span><span class="sxs-lookup"><span data-stu-id="55fc7-125">4</span></span>|<span data-ttu-id="55fc7-126">时不受信任应用程序写入磁盘扇区生成日志。</span><span class="sxs-lookup"><span data-stu-id="55fc7-126">Generate logs when untrusted apps write to disk sectors.</span></span>|





