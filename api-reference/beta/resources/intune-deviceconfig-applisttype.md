---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 49ef93ede45fd784f4b0b9bc52010dce80fa2eb1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075964"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="63a0d-103">appListType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="63a0d-103">appListType enum type</span></span>

<span data-ttu-id="63a0d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63a0d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63a0d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="63a0d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63a0d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="63a0d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63a0d-107">合规性应用程序列表的可能值。</span><span class="sxs-lookup"><span data-stu-id="63a0d-107">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="63a0d-108">成员</span><span class="sxs-lookup"><span data-stu-id="63a0d-108">Members</span></span>
|<span data-ttu-id="63a0d-109">成员</span><span class="sxs-lookup"><span data-stu-id="63a0d-109">Member</span></span>|<span data-ttu-id="63a0d-110">值</span><span class="sxs-lookup"><span data-stu-id="63a0d-110">Value</span></span>|<span data-ttu-id="63a0d-111">说明</span><span class="sxs-lookup"><span data-stu-id="63a0d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63a0d-112">无</span><span class="sxs-lookup"><span data-stu-id="63a0d-112">none</span></span>|<span data-ttu-id="63a0d-113">0</span><span class="sxs-lookup"><span data-stu-id="63a0d-113">0</span></span>|<span data-ttu-id="63a0d-114">默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="63a0d-114">Default value, no intent.</span></span>|
|<span data-ttu-id="63a0d-115">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="63a0d-115">appsInListCompliant</span></span>|<span data-ttu-id="63a0d-116">1 </span><span class="sxs-lookup"><span data-stu-id="63a0d-116">1</span></span>|<span data-ttu-id="63a0d-117">此列表代表只有列表中的应用程序符合标准的应用程序，才会被视为合规 (性的) 。</span><span class="sxs-lookup"><span data-stu-id="63a0d-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="63a0d-118">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="63a0d-118">appsNotInListCompliant</span></span>|<span data-ttu-id="63a0d-119">2 </span><span class="sxs-lookup"><span data-stu-id="63a0d-119">2</span></span>|<span data-ttu-id="63a0d-120">此列表表示将被视为不合规的应用程序 (所有应用程序不符合列表) 中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="63a0d-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|






