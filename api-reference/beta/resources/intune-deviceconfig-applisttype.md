---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7cd3e1f8cffa747ca23e00ba0d9264cb1089dee2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260815"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="38cf0-103">appListType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="38cf0-103">appListType enum type</span></span>

<span data-ttu-id="38cf0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38cf0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38cf0-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="38cf0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38cf0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="38cf0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38cf0-107">合规性应用程序列表的可能值。</span><span class="sxs-lookup"><span data-stu-id="38cf0-107">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="38cf0-108">成员</span><span class="sxs-lookup"><span data-stu-id="38cf0-108">Members</span></span>
|<span data-ttu-id="38cf0-109">成员</span><span class="sxs-lookup"><span data-stu-id="38cf0-109">Member</span></span>|<span data-ttu-id="38cf0-110">值</span><span class="sxs-lookup"><span data-stu-id="38cf0-110">Value</span></span>|<span data-ttu-id="38cf0-111">说明</span><span class="sxs-lookup"><span data-stu-id="38cf0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38cf0-112">无</span><span class="sxs-lookup"><span data-stu-id="38cf0-112">none</span></span>|<span data-ttu-id="38cf0-113">0</span><span class="sxs-lookup"><span data-stu-id="38cf0-113">0</span></span>|<span data-ttu-id="38cf0-114">默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="38cf0-114">Default value, no intent.</span></span>|
|<span data-ttu-id="38cf0-115">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="38cf0-115">appsInListCompliant</span></span>|<span data-ttu-id="38cf0-116">1</span><span class="sxs-lookup"><span data-stu-id="38cf0-116">1</span></span>|<span data-ttu-id="38cf0-117">此列表代表只有列表中的应用程序符合标准的应用程序，才会被视为合规 (性的) 。</span><span class="sxs-lookup"><span data-stu-id="38cf0-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="38cf0-118">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="38cf0-118">appsNotInListCompliant</span></span>|<span data-ttu-id="38cf0-119">双面</span><span class="sxs-lookup"><span data-stu-id="38cf0-119">2</span></span>|<span data-ttu-id="38cf0-120">此列表表示将被视为不合规的应用程序 (所有应用程序不符合列表) 中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="38cf0-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|




