---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7a02b8ed105206f53894ddb8d35dc24106eebebc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028600"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="88c54-103">appListType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="88c54-103">appListType enum type</span></span>

> <span data-ttu-id="88c54-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88c54-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88c54-105">合规性应用程序列表的可能值。</span><span class="sxs-lookup"><span data-stu-id="88c54-105">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="88c54-106">成员</span><span class="sxs-lookup"><span data-stu-id="88c54-106">Members</span></span>
|<span data-ttu-id="88c54-107">成员</span><span class="sxs-lookup"><span data-stu-id="88c54-107">Member</span></span>|<span data-ttu-id="88c54-108">值</span><span class="sxs-lookup"><span data-stu-id="88c54-108">Value</span></span>|<span data-ttu-id="88c54-109">说明</span><span class="sxs-lookup"><span data-stu-id="88c54-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88c54-110">无</span><span class="sxs-lookup"><span data-stu-id="88c54-110">none</span></span>|<span data-ttu-id="88c54-111">0</span><span class="sxs-lookup"><span data-stu-id="88c54-111">0</span></span>|<span data-ttu-id="88c54-112">默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="88c54-112">Default value, no intent.</span></span>|
|<span data-ttu-id="88c54-113">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="88c54-113">appsInListCompliant</span></span>|<span data-ttu-id="88c54-114">1</span><span class="sxs-lookup"><span data-stu-id="88c54-114">1</span></span>|<span data-ttu-id="88c54-115">此列表表示将被视为合规性的应用程序 (仅符合列表中的应用程序)。</span><span class="sxs-lookup"><span data-stu-id="88c54-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="88c54-116">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="88c54-116">appsNotInListCompliant</span></span>|<span data-ttu-id="88c54-117">双面</span><span class="sxs-lookup"><span data-stu-id="88c54-117">2</span></span>|<span data-ttu-id="88c54-118">此列表表示将被视为不合规的应用程序 (所有应用程序都符合列表中的应用程序)。</span><span class="sxs-lookup"><span data-stu-id="88c54-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



