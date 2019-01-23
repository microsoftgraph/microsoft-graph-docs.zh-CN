---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cf8930136b00b7b5579ec5e7266b6a77a9a11968
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415220"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="cbe2b-103">appListType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cbe2b-103">appListType enum type</span></span>

> <span data-ttu-id="cbe2b-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="cbe2b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cbe2b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cbe2b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cbe2b-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cbe2b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbe2b-107">合规性应用程序列表的可能值。</span><span class="sxs-lookup"><span data-stu-id="cbe2b-107">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="cbe2b-108">成员</span><span class="sxs-lookup"><span data-stu-id="cbe2b-108">Members</span></span>
|<span data-ttu-id="cbe2b-109">成员</span><span class="sxs-lookup"><span data-stu-id="cbe2b-109">Member</span></span>|<span data-ttu-id="cbe2b-110">值</span><span class="sxs-lookup"><span data-stu-id="cbe2b-110">Value</span></span>|<span data-ttu-id="cbe2b-111">说明</span><span class="sxs-lookup"><span data-stu-id="cbe2b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbe2b-112">无</span><span class="sxs-lookup"><span data-stu-id="cbe2b-112">none</span></span>|<span data-ttu-id="cbe2b-113">0</span><span class="sxs-lookup"><span data-stu-id="cbe2b-113">0</span></span>|<span data-ttu-id="cbe2b-114">默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="cbe2b-114">Default value, no intent.</span></span>|
|<span data-ttu-id="cbe2b-115">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="cbe2b-115">appsInListCompliant</span></span>|<span data-ttu-id="cbe2b-116">1</span><span class="sxs-lookup"><span data-stu-id="cbe2b-116">1</span></span>|<span data-ttu-id="cbe2b-117">在列表代表将被视为符合 （仅在列表上的应用程序都符合） 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="cbe2b-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="cbe2b-118">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="cbe2b-118">appsNotInListCompliant</span></span>|<span data-ttu-id="cbe2b-119">2</span><span class="sxs-lookup"><span data-stu-id="cbe2b-119">2</span></span>|<span data-ttu-id="cbe2b-120">在列表代表将被视为不符合标准的应用程序 （所有应用程序是除列表上的应用程序兼容）。</span><span class="sxs-lookup"><span data-stu-id="cbe2b-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|




