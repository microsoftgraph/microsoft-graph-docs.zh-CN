---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 61999950fbf9a54a2d93576fe77d950e30b8b561
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469950"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="29a12-103">appListType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="29a12-103">appListType enum type</span></span>

<span data-ttu-id="29a12-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29a12-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29a12-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="29a12-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29a12-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="29a12-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29a12-107">合规性应用程序列表的可能值。</span><span class="sxs-lookup"><span data-stu-id="29a12-107">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="29a12-108">成员</span><span class="sxs-lookup"><span data-stu-id="29a12-108">Members</span></span>
|<span data-ttu-id="29a12-109">成员</span><span class="sxs-lookup"><span data-stu-id="29a12-109">Member</span></span>|<span data-ttu-id="29a12-110">值</span><span class="sxs-lookup"><span data-stu-id="29a12-110">Value</span></span>|<span data-ttu-id="29a12-111">说明</span><span class="sxs-lookup"><span data-stu-id="29a12-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29a12-112">无</span><span class="sxs-lookup"><span data-stu-id="29a12-112">none</span></span>|<span data-ttu-id="29a12-113">0</span><span class="sxs-lookup"><span data-stu-id="29a12-113">0</span></span>|<span data-ttu-id="29a12-114">默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="29a12-114">Default value, no intent.</span></span>|
|<span data-ttu-id="29a12-115">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="29a12-115">appsInListCompliant</span></span>|<span data-ttu-id="29a12-116">1</span><span class="sxs-lookup"><span data-stu-id="29a12-116">1</span></span>|<span data-ttu-id="29a12-117">此列表表示将被视为合规性的应用程序（仅符合列表中的应用程序）。</span><span class="sxs-lookup"><span data-stu-id="29a12-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="29a12-118">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="29a12-118">appsNotInListCompliant</span></span>|<span data-ttu-id="29a12-119">双面</span><span class="sxs-lookup"><span data-stu-id="29a12-119">2</span></span>|<span data-ttu-id="29a12-120">此列表表示将被视为不合规的应用程序（所有应用程序都符合列表中的应用程序）。</span><span class="sxs-lookup"><span data-stu-id="29a12-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



