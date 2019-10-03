---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c46f059721727e8752df6f7b0ad99a48c3104d64
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366725"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="7c41f-103">appListType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7c41f-103">appListType enum type</span></span>

> <span data-ttu-id="7c41f-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7c41f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c41f-105">合规性应用程序列表的可能值。</span><span class="sxs-lookup"><span data-stu-id="7c41f-105">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="7c41f-106">成员</span><span class="sxs-lookup"><span data-stu-id="7c41f-106">Members</span></span>
|<span data-ttu-id="7c41f-107">成员</span><span class="sxs-lookup"><span data-stu-id="7c41f-107">Member</span></span>|<span data-ttu-id="7c41f-108">值</span><span class="sxs-lookup"><span data-stu-id="7c41f-108">Value</span></span>|<span data-ttu-id="7c41f-109">说明</span><span class="sxs-lookup"><span data-stu-id="7c41f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c41f-110">无</span><span class="sxs-lookup"><span data-stu-id="7c41f-110">none</span></span>|<span data-ttu-id="7c41f-111">0</span><span class="sxs-lookup"><span data-stu-id="7c41f-111">0</span></span>|<span data-ttu-id="7c41f-112">默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="7c41f-112">Default value, no intent.</span></span>|
|<span data-ttu-id="7c41f-113">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="7c41f-113">appsInListCompliant</span></span>|<span data-ttu-id="7c41f-114">1</span><span class="sxs-lookup"><span data-stu-id="7c41f-114">1</span></span>|<span data-ttu-id="7c41f-115">此列表表示将被视为合规性的应用程序（仅符合列表中的应用程序）。</span><span class="sxs-lookup"><span data-stu-id="7c41f-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="7c41f-116">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="7c41f-116">appsNotInListCompliant</span></span>|<span data-ttu-id="7c41f-117">双面</span><span class="sxs-lookup"><span data-stu-id="7c41f-117">2</span></span>|<span data-ttu-id="7c41f-118">此列表表示将被视为不合规的应用程序（所有应用程序都符合列表中的应用程序）。</span><span class="sxs-lookup"><span data-stu-id="7c41f-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|




