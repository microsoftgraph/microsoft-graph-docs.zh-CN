---
title: groupPolicyMigrationReadiness 枚举类型
description: 指示组策略对象文件是否已被覆盖并准备好进行 Intune 迁移。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: efd579adb3c3408eda9b87ffb7f48e98c836065f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783170"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a><span data-ttu-id="3ecc5-103">groupPolicyMigrationReadiness 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3ecc5-103">groupPolicyMigrationReadiness enum type</span></span>

> <span data-ttu-id="3ecc5-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3ecc5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ecc5-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3ecc5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ecc5-106">指示组策略对象文件是否已被覆盖并准备好进行 Intune 迁移。</span><span class="sxs-lookup"><span data-stu-id="3ecc5-106">Indicates if the Group Policy Object file is covered and ready for Intune migration.</span></span>

## <a name="members"></a><span data-ttu-id="3ecc5-107">成员</span><span class="sxs-lookup"><span data-stu-id="3ecc5-107">Members</span></span>
|<span data-ttu-id="3ecc5-108">成员</span><span class="sxs-lookup"><span data-stu-id="3ecc5-108">Member</span></span>|<span data-ttu-id="3ecc5-109">值</span><span class="sxs-lookup"><span data-stu-id="3ecc5-109">Value</span></span>|<span data-ttu-id="3ecc5-110">说明</span><span class="sxs-lookup"><span data-stu-id="3ecc5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ecc5-111">无</span><span class="sxs-lookup"><span data-stu-id="3ecc5-111">none</span></span>|<span data-ttu-id="3ecc5-112">1</span><span class="sxs-lookup"><span data-stu-id="3ecc5-112">1</span></span>|<span data-ttu-id="3ecc5-113">无 Intune 覆盖范围</span><span class="sxs-lookup"><span data-stu-id="3ecc5-113">No Intune coverage</span></span>|
|<span data-ttu-id="3ecc5-114">环</span><span class="sxs-lookup"><span data-stu-id="3ecc5-114">partial</span></span>|<span data-ttu-id="3ecc5-115">双面</span><span class="sxs-lookup"><span data-stu-id="3ecc5-115">2</span></span>|<span data-ttu-id="3ecc5-116">部分 Intune 覆盖范围</span><span class="sxs-lookup"><span data-stu-id="3ecc5-116">Partial Intune coverage</span></span>|
|<span data-ttu-id="3ecc5-117">complete</span><span class="sxs-lookup"><span data-stu-id="3ecc5-117">complete</span></span>|<span data-ttu-id="3ecc5-118">第三章</span><span class="sxs-lookup"><span data-stu-id="3ecc5-118">3</span></span>|<span data-ttu-id="3ecc5-119">完成 Intune 覆盖范围</span><span class="sxs-lookup"><span data-stu-id="3ecc5-119">Complete Intune coverage</span></span>|
|<span data-ttu-id="3ecc5-120">error</span><span class="sxs-lookup"><span data-stu-id="3ecc5-120">error</span></span>|<span data-ttu-id="3ecc5-121">4 </span><span class="sxs-lookup"><span data-stu-id="3ecc5-121">4</span></span>|<span data-ttu-id="3ecc5-122">分析覆盖率时出错</span><span class="sxs-lookup"><span data-stu-id="3ecc5-122">Error when analyzing coverage</span></span>|
|<span data-ttu-id="3ecc5-123">notApplicable</span><span class="sxs-lookup"><span data-stu-id="3ecc5-123">notApplicable</span></span>|<span data-ttu-id="3ecc5-124">5 </span><span class="sxs-lookup"><span data-stu-id="3ecc5-124">5</span></span>|<span data-ttu-id="3ecc5-125">GPO 中没有组策略设置</span><span class="sxs-lookup"><span data-stu-id="3ecc5-125">No Group Policy settings in GPO</span></span>|



