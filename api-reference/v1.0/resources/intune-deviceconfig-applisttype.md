---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 76c13c26812fd8ab7c8e1224b55e616502b514ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839268"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="b1baf-103">appListType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b1baf-103">appListType enum type</span></span>

> <span data-ttu-id="b1baf-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b1baf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1baf-105">合规性应用程序列表的可能值。</span><span class="sxs-lookup"><span data-stu-id="b1baf-105">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="b1baf-106">成员</span><span class="sxs-lookup"><span data-stu-id="b1baf-106">Members</span></span>
|<span data-ttu-id="b1baf-107">成员</span><span class="sxs-lookup"><span data-stu-id="b1baf-107">Member</span></span>|<span data-ttu-id="b1baf-108">值</span><span class="sxs-lookup"><span data-stu-id="b1baf-108">Value</span></span>|<span data-ttu-id="b1baf-109">Description</span><span class="sxs-lookup"><span data-stu-id="b1baf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1baf-110">无</span><span class="sxs-lookup"><span data-stu-id="b1baf-110">none</span></span>|<span data-ttu-id="b1baf-111">0</span><span class="sxs-lookup"><span data-stu-id="b1baf-111">0</span></span>|<span data-ttu-id="b1baf-112">默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="b1baf-112">Default value, no intent.</span></span>|
|<span data-ttu-id="b1baf-113">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="b1baf-113">appsInListCompliant</span></span>|<span data-ttu-id="b1baf-114">1</span><span class="sxs-lookup"><span data-stu-id="b1baf-114">1</span></span>|<span data-ttu-id="b1baf-115">在列表代表将被视为符合 （仅在列表上的应用程序都符合） 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="b1baf-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="b1baf-116">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="b1baf-116">appsNotInListCompliant</span></span>|<span data-ttu-id="b1baf-117">2</span><span class="sxs-lookup"><span data-stu-id="b1baf-117">2</span></span>|<span data-ttu-id="b1baf-118">在列表代表将被视为不符合标准的应用程序 （所有应用程序是除列表上的应用程序兼容）。</span><span class="sxs-lookup"><span data-stu-id="b1baf-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



