---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8e76b06d474f642f26655fa7f1b8e07e540b7495
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051100"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="73c11-103">appListType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="73c11-103">appListType enum type</span></span>

<span data-ttu-id="73c11-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73c11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73c11-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="73c11-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73c11-106">合规性应用程序列表的可能值。</span><span class="sxs-lookup"><span data-stu-id="73c11-106">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="73c11-107">成员</span><span class="sxs-lookup"><span data-stu-id="73c11-107">Members</span></span>
|<span data-ttu-id="73c11-108">成员</span><span class="sxs-lookup"><span data-stu-id="73c11-108">Member</span></span>|<span data-ttu-id="73c11-109">值</span><span class="sxs-lookup"><span data-stu-id="73c11-109">Value</span></span>|<span data-ttu-id="73c11-110">说明</span><span class="sxs-lookup"><span data-stu-id="73c11-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73c11-111">无</span><span class="sxs-lookup"><span data-stu-id="73c11-111">none</span></span>|<span data-ttu-id="73c11-112">0</span><span class="sxs-lookup"><span data-stu-id="73c11-112">0</span></span>|<span data-ttu-id="73c11-113">默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="73c11-113">Default value, no intent.</span></span>|
|<span data-ttu-id="73c11-114">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="73c11-114">appsInListCompliant</span></span>|<span data-ttu-id="73c11-115">1 </span><span class="sxs-lookup"><span data-stu-id="73c11-115">1</span></span>|<span data-ttu-id="73c11-116">此列表代表只有列表中的应用程序符合标准的应用程序，才会被视为合规 (性的) 。</span><span class="sxs-lookup"><span data-stu-id="73c11-116">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="73c11-117">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="73c11-117">appsNotInListCompliant</span></span>|<span data-ttu-id="73c11-118">2 </span><span class="sxs-lookup"><span data-stu-id="73c11-118">2</span></span>|<span data-ttu-id="73c11-119">此列表表示将被视为不合规的应用程序 (所有应用程序不符合列表) 中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="73c11-119">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|









