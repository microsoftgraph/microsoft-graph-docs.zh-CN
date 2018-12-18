---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
author: tfitzmac
ms.openlocfilehash: 3f0fa162131fc1f59beba1f057fa888e0f2260c5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331190"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="3c67b-103">appListType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3c67b-103">appListType enum type</span></span>

> <span data-ttu-id="3c67b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3c67b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c67b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3c67b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c67b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3c67b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c67b-107">合规性应用程序列表的可能值。</span><span class="sxs-lookup"><span data-stu-id="3c67b-107">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="3c67b-108">成员</span><span class="sxs-lookup"><span data-stu-id="3c67b-108">Members</span></span>
|<span data-ttu-id="3c67b-109">成员</span><span class="sxs-lookup"><span data-stu-id="3c67b-109">Member</span></span>|<span data-ttu-id="3c67b-110">值</span><span class="sxs-lookup"><span data-stu-id="3c67b-110">Value</span></span>|<span data-ttu-id="3c67b-111">说明</span><span class="sxs-lookup"><span data-stu-id="3c67b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c67b-112">无</span><span class="sxs-lookup"><span data-stu-id="3c67b-112">none</span></span>|<span data-ttu-id="3c67b-113">0</span><span class="sxs-lookup"><span data-stu-id="3c67b-113">0</span></span>|<span data-ttu-id="3c67b-114">默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="3c67b-114">Default value, no intent.</span></span>|
|<span data-ttu-id="3c67b-115">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="3c67b-115">appsInListCompliant</span></span>|<span data-ttu-id="3c67b-116">1</span><span class="sxs-lookup"><span data-stu-id="3c67b-116">1</span></span>|<span data-ttu-id="3c67b-117">在列表代表将被视为符合 （仅在列表上的应用程序都符合） 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="3c67b-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="3c67b-118">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="3c67b-118">appsNotInListCompliant</span></span>|<span data-ttu-id="3c67b-119">2</span><span class="sxs-lookup"><span data-stu-id="3c67b-119">2</span></span>|<span data-ttu-id="3c67b-120">在列表代表将被视为不符合标准的应用程序 （所有应用程序是除列表上的应用程序兼容）。</span><span class="sxs-lookup"><span data-stu-id="3c67b-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|





