---
title: groupPolicyMigrationReadiness 枚举类型
description: 指示组策略对象文件是否已被覆盖并准备好进行 Intune 迁移。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e6b2ec4f8363f6ad68cd34a77287502eaadf2d52
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524481"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a><span data-ttu-id="beab4-103">groupPolicyMigrationReadiness 枚举类型</span><span class="sxs-lookup"><span data-stu-id="beab4-103">groupPolicyMigrationReadiness enum type</span></span>

<span data-ttu-id="beab4-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="beab4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="beab4-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="beab4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="beab4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="beab4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="beab4-107">指示组策略对象文件是否已被覆盖并准备好进行 Intune 迁移。</span><span class="sxs-lookup"><span data-stu-id="beab4-107">Indicates if the Group Policy Object file is covered and ready for Intune migration.</span></span>

## <a name="members"></a><span data-ttu-id="beab4-108">成员</span><span class="sxs-lookup"><span data-stu-id="beab4-108">Members</span></span>
|<span data-ttu-id="beab4-109">成员</span><span class="sxs-lookup"><span data-stu-id="beab4-109">Member</span></span>|<span data-ttu-id="beab4-110">值</span><span class="sxs-lookup"><span data-stu-id="beab4-110">Value</span></span>|<span data-ttu-id="beab4-111">说明</span><span class="sxs-lookup"><span data-stu-id="beab4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beab4-112">无</span><span class="sxs-lookup"><span data-stu-id="beab4-112">none</span></span>|<span data-ttu-id="beab4-113">1 </span><span class="sxs-lookup"><span data-stu-id="beab4-113">1</span></span>|<span data-ttu-id="beab4-114">无 Intune 覆盖范围</span><span class="sxs-lookup"><span data-stu-id="beab4-114">No Intune coverage</span></span>|
|<span data-ttu-id="beab4-115">环</span><span class="sxs-lookup"><span data-stu-id="beab4-115">partial</span></span>|<span data-ttu-id="beab4-116">2 </span><span class="sxs-lookup"><span data-stu-id="beab4-116">2</span></span>|<span data-ttu-id="beab4-117">部分 Intune 覆盖范围</span><span class="sxs-lookup"><span data-stu-id="beab4-117">Partial Intune coverage</span></span>|
|<span data-ttu-id="beab4-118">complete</span><span class="sxs-lookup"><span data-stu-id="beab4-118">complete</span></span>|<span data-ttu-id="beab4-119">3 </span><span class="sxs-lookup"><span data-stu-id="beab4-119">3</span></span>|<span data-ttu-id="beab4-120">完成 Intune 覆盖范围</span><span class="sxs-lookup"><span data-stu-id="beab4-120">Complete Intune coverage</span></span>|
|<span data-ttu-id="beab4-121">error</span><span class="sxs-lookup"><span data-stu-id="beab4-121">error</span></span>|<span data-ttu-id="beab4-122">4 </span><span class="sxs-lookup"><span data-stu-id="beab4-122">4</span></span>|<span data-ttu-id="beab4-123">分析覆盖率时出错</span><span class="sxs-lookup"><span data-stu-id="beab4-123">Error when analyzing coverage</span></span>|
|<span data-ttu-id="beab4-124">notApplicable</span><span class="sxs-lookup"><span data-stu-id="beab4-124">notApplicable</span></span>|<span data-ttu-id="beab4-125">5 </span><span class="sxs-lookup"><span data-stu-id="beab4-125">5</span></span>|<span data-ttu-id="beab4-126">GPO 中没有组策略设置</span><span class="sxs-lookup"><span data-stu-id="beab4-126">No Group Policy settings in GPO</span></span>|



