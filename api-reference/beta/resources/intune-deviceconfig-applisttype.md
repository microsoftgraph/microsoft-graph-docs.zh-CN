---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b9166ef625387b47f07b56efd197dc22f1f440d0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333903"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="d96dc-103">appListType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d96dc-103">appListType enum type</span></span>

> <span data-ttu-id="d96dc-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d96dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d96dc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d96dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d96dc-106">合规性应用程序列表的可能值。</span><span class="sxs-lookup"><span data-stu-id="d96dc-106">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="d96dc-107">成员</span><span class="sxs-lookup"><span data-stu-id="d96dc-107">Members</span></span>
|<span data-ttu-id="d96dc-108">成员</span><span class="sxs-lookup"><span data-stu-id="d96dc-108">Member</span></span>|<span data-ttu-id="d96dc-109">值</span><span class="sxs-lookup"><span data-stu-id="d96dc-109">Value</span></span>|<span data-ttu-id="d96dc-110">说明</span><span class="sxs-lookup"><span data-stu-id="d96dc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d96dc-111">无</span><span class="sxs-lookup"><span data-stu-id="d96dc-111">none</span></span>|<span data-ttu-id="d96dc-112">0</span><span class="sxs-lookup"><span data-stu-id="d96dc-112">0</span></span>|<span data-ttu-id="d96dc-113">默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="d96dc-113">Default value, no intent.</span></span>|
|<span data-ttu-id="d96dc-114">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="d96dc-114">appsInListCompliant</span></span>|<span data-ttu-id="d96dc-115">1</span><span class="sxs-lookup"><span data-stu-id="d96dc-115">1</span></span>|<span data-ttu-id="d96dc-116">此列表表示将被视为合规性的应用程序 (仅符合列表中的应用程序)。</span><span class="sxs-lookup"><span data-stu-id="d96dc-116">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="d96dc-117">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="d96dc-117">appsNotInListCompliant</span></span>|<span data-ttu-id="d96dc-118">双面</span><span class="sxs-lookup"><span data-stu-id="d96dc-118">2</span></span>|<span data-ttu-id="d96dc-119">此列表表示将被视为不合规的应用程序 (所有应用程序都符合列表中的应用程序)。</span><span class="sxs-lookup"><span data-stu-id="d96dc-119">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



