---
title: groupPolicyMigrationReadiness 枚举类型
description: 指示组策略对象文件是否已被覆盖并准备好进行 Intune 迁移。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fb87c31bfe92a8845953e6e2a264ec60c9a3d863
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539104"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a><span data-ttu-id="3df49-103">groupPolicyMigrationReadiness 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3df49-103">groupPolicyMigrationReadiness enum type</span></span>

> <span data-ttu-id="3df49-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3df49-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3df49-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3df49-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3df49-106">指示组策略对象文件是否已被覆盖并准备好进行 Intune 迁移。</span><span class="sxs-lookup"><span data-stu-id="3df49-106">Indicates if the Group Policy Object file is covered and ready for Intune migration.</span></span>

## <a name="members"></a><span data-ttu-id="3df49-107">成员</span><span class="sxs-lookup"><span data-stu-id="3df49-107">Members</span></span>
|<span data-ttu-id="3df49-108">成员</span><span class="sxs-lookup"><span data-stu-id="3df49-108">Member</span></span>|<span data-ttu-id="3df49-109">值</span><span class="sxs-lookup"><span data-stu-id="3df49-109">Value</span></span>|<span data-ttu-id="3df49-110">说明</span><span class="sxs-lookup"><span data-stu-id="3df49-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3df49-111">无</span><span class="sxs-lookup"><span data-stu-id="3df49-111">none</span></span>|<span data-ttu-id="3df49-112">1</span><span class="sxs-lookup"><span data-stu-id="3df49-112">1</span></span>|<span data-ttu-id="3df49-113">无 Intune 覆盖范围</span><span class="sxs-lookup"><span data-stu-id="3df49-113">No Intune coverage</span></span>|
|<span data-ttu-id="3df49-114">环</span><span class="sxs-lookup"><span data-stu-id="3df49-114">partial</span></span>|<span data-ttu-id="3df49-115">双面</span><span class="sxs-lookup"><span data-stu-id="3df49-115">2</span></span>|<span data-ttu-id="3df49-116">部分 Intune 覆盖范围</span><span class="sxs-lookup"><span data-stu-id="3df49-116">Partial Intune coverage</span></span>|
|<span data-ttu-id="3df49-117">complete</span><span class="sxs-lookup"><span data-stu-id="3df49-117">complete</span></span>|<span data-ttu-id="3df49-118">第三章</span><span class="sxs-lookup"><span data-stu-id="3df49-118">3</span></span>|<span data-ttu-id="3df49-119">完成 Intune 覆盖范围</span><span class="sxs-lookup"><span data-stu-id="3df49-119">Complete Intune coverage</span></span>|
|<span data-ttu-id="3df49-120">error</span><span class="sxs-lookup"><span data-stu-id="3df49-120">error</span></span>|<span data-ttu-id="3df49-121">4 </span><span class="sxs-lookup"><span data-stu-id="3df49-121">4</span></span>|<span data-ttu-id="3df49-122">分析覆盖率时出错</span><span class="sxs-lookup"><span data-stu-id="3df49-122">Error when analyzing coverage</span></span>|
|<span data-ttu-id="3df49-123">notApplicable</span><span class="sxs-lookup"><span data-stu-id="3df49-123">notApplicable</span></span>|<span data-ttu-id="3df49-124">5 </span><span class="sxs-lookup"><span data-stu-id="3df49-124">5</span></span>|<span data-ttu-id="3df49-125">GPO 中没有组策略设置</span><span class="sxs-lookup"><span data-stu-id="3df49-125">No Group Policy settings in GPO</span></span>|



