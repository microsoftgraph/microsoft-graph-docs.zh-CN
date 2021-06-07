---
title: appListType 枚举类型
description: 合规性应用列表的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2b8126ded9f6d0e9f68c6a9f5e8bcbcbbb216294
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755915"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="2dc95-103">appListType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2dc95-103">appListType enum type</span></span>

<span data-ttu-id="2dc95-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2dc95-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2dc95-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2dc95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2dc95-106">合规性应用列表的可能值。</span><span class="sxs-lookup"><span data-stu-id="2dc95-106">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="2dc95-107">成员</span><span class="sxs-lookup"><span data-stu-id="2dc95-107">Members</span></span>
|<span data-ttu-id="2dc95-108">成员</span><span class="sxs-lookup"><span data-stu-id="2dc95-108">Member</span></span>|<span data-ttu-id="2dc95-109">值</span><span class="sxs-lookup"><span data-stu-id="2dc95-109">Value</span></span>|<span data-ttu-id="2dc95-110">Description</span><span class="sxs-lookup"><span data-stu-id="2dc95-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dc95-111">无</span><span class="sxs-lookup"><span data-stu-id="2dc95-111">none</span></span>|<span data-ttu-id="2dc95-112">0</span><span class="sxs-lookup"><span data-stu-id="2dc95-112">0</span></span>|<span data-ttu-id="2dc95-113">默认值，无意图。</span><span class="sxs-lookup"><span data-stu-id="2dc95-113">Default value, no intent.</span></span>|
|<span data-ttu-id="2dc95-114">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="2dc95-114">appsInListCompliant</span></span>|<span data-ttu-id="2dc95-115">1</span><span class="sxs-lookup"><span data-stu-id="2dc95-115">1</span></span>|<span data-ttu-id="2dc95-116">该列表表示将被视为合规的应用 (只有列表上的应用符合) 。</span><span class="sxs-lookup"><span data-stu-id="2dc95-116">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="2dc95-117">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="2dc95-117">appsNotInListCompliant</span></span>|<span data-ttu-id="2dc95-118">2</span><span class="sxs-lookup"><span data-stu-id="2dc95-118">2</span></span>|<span data-ttu-id="2dc95-119">该列表表示被视为不合规的应用 (所有应用都合规，列表上的应用除外) 。</span><span class="sxs-lookup"><span data-stu-id="2dc95-119">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|




