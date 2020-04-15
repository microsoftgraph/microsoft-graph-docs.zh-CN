---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8a372f2f160a4a08a1c9f1c3e4276ea10344daff
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449153"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="b973e-103">appListType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b973e-103">appListType enum type</span></span>

<span data-ttu-id="b973e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b973e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b973e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b973e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b973e-106">合规性应用程序列表的可能值。</span><span class="sxs-lookup"><span data-stu-id="b973e-106">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="b973e-107">成员</span><span class="sxs-lookup"><span data-stu-id="b973e-107">Members</span></span>
|<span data-ttu-id="b973e-108">成员</span><span class="sxs-lookup"><span data-stu-id="b973e-108">Member</span></span>|<span data-ttu-id="b973e-109">值</span><span class="sxs-lookup"><span data-stu-id="b973e-109">Value</span></span>|<span data-ttu-id="b973e-110">说明</span><span class="sxs-lookup"><span data-stu-id="b973e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b973e-111">无</span><span class="sxs-lookup"><span data-stu-id="b973e-111">none</span></span>|<span data-ttu-id="b973e-112">0</span><span class="sxs-lookup"><span data-stu-id="b973e-112">0</span></span>|<span data-ttu-id="b973e-113">默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="b973e-113">Default value, no intent.</span></span>|
|<span data-ttu-id="b973e-114">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="b973e-114">appsInListCompliant</span></span>|<span data-ttu-id="b973e-115">1</span><span class="sxs-lookup"><span data-stu-id="b973e-115">1</span></span>|<span data-ttu-id="b973e-116">此列表表示将被视为合规性的应用程序（仅符合列表中的应用程序）。</span><span class="sxs-lookup"><span data-stu-id="b973e-116">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="b973e-117">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="b973e-117">appsNotInListCompliant</span></span>|<span data-ttu-id="b973e-118">双面</span><span class="sxs-lookup"><span data-stu-id="b973e-118">2</span></span>|<span data-ttu-id="b973e-119">此列表表示将被视为不合规的应用程序（所有应用程序都符合列表中的应用程序）。</span><span class="sxs-lookup"><span data-stu-id="b973e-119">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|







