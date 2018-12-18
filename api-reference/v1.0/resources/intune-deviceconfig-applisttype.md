---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
author: tfitzmac
ms.openlocfilehash: ab5d8f45343b017693906b13be25c88d5b06e8f7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354717"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="a9146-103">appListType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a9146-103">appListType enum type</span></span>

> <span data-ttu-id="a9146-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a9146-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9146-105">合规性应用程序列表的可能值。</span><span class="sxs-lookup"><span data-stu-id="a9146-105">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="a9146-106">成员</span><span class="sxs-lookup"><span data-stu-id="a9146-106">Members</span></span>
|<span data-ttu-id="a9146-107">成员</span><span class="sxs-lookup"><span data-stu-id="a9146-107">Member</span></span>|<span data-ttu-id="a9146-108">值</span><span class="sxs-lookup"><span data-stu-id="a9146-108">Value</span></span>|<span data-ttu-id="a9146-109">说明</span><span class="sxs-lookup"><span data-stu-id="a9146-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9146-110">无</span><span class="sxs-lookup"><span data-stu-id="a9146-110">none</span></span>|<span data-ttu-id="a9146-111">0</span><span class="sxs-lookup"><span data-stu-id="a9146-111">0</span></span>|<span data-ttu-id="a9146-112">默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="a9146-112">Default value, no intent.</span></span>|
|<span data-ttu-id="a9146-113">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="a9146-113">appsInListCompliant</span></span>|<span data-ttu-id="a9146-114">1</span><span class="sxs-lookup"><span data-stu-id="a9146-114">1</span></span>|<span data-ttu-id="a9146-115">在列表代表将被视为符合 （仅在列表上的应用程序都符合） 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="a9146-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="a9146-116">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="a9146-116">appsNotInListCompliant</span></span>|<span data-ttu-id="a9146-117">2</span><span class="sxs-lookup"><span data-stu-id="a9146-117">2</span></span>|<span data-ttu-id="a9146-118">在列表代表将被视为不符合标准的应用程序 （所有应用程序是除列表上的应用程序兼容）。</span><span class="sxs-lookup"><span data-stu-id="a9146-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



