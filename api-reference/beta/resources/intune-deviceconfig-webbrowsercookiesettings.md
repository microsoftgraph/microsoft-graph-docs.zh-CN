---
title: webBrowserCookieSettings 枚举类型
description: Web 浏览器 Cookie 设置。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 54fe38b9227c38f3af13ec242ece2d0bd6c144fa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927388"
---
# <a name="webbrowsercookiesettings-enum-type"></a><span data-ttu-id="4dd12-103">webBrowserCookieSettings 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4dd12-103">webBrowserCookieSettings enum type</span></span>

> <span data-ttu-id="4dd12-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4dd12-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4dd12-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4dd12-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4dd12-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4dd12-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4dd12-107">Web 浏览器 Cookie 设置。</span><span class="sxs-lookup"><span data-stu-id="4dd12-107">Web Browser Cookie Settings.</span></span>
## <a name="members"></a><span data-ttu-id="4dd12-108">成员</span><span class="sxs-lookup"><span data-stu-id="4dd12-108">Members</span></span>
|<span data-ttu-id="4dd12-109">成员</span><span class="sxs-lookup"><span data-stu-id="4dd12-109">Member</span></span>|<span data-ttu-id="4dd12-110">值</span><span class="sxs-lookup"><span data-stu-id="4dd12-110">Value</span></span>|<span data-ttu-id="4dd12-111">Description</span><span class="sxs-lookup"><span data-stu-id="4dd12-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dd12-112">browserDefault</span><span class="sxs-lookup"><span data-stu-id="4dd12-112">browserDefault</span></span>|<span data-ttu-id="4dd12-113">0</span><span class="sxs-lookup"><span data-stu-id="4dd12-113">0</span></span>|<span data-ttu-id="4dd12-114">浏览器默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="4dd12-114">Browser default value, no intent.</span></span>|
|<span data-ttu-id="4dd12-115">blockAlways</span><span class="sxs-lookup"><span data-stu-id="4dd12-115">blockAlways</span></span>|<span data-ttu-id="4dd12-116">1</span><span class="sxs-lookup"><span data-stu-id="4dd12-116">1</span></span>|<span data-ttu-id="4dd12-117">始终阻止 cookie。</span><span class="sxs-lookup"><span data-stu-id="4dd12-117">Always block cookies.</span></span>|
|<span data-ttu-id="4dd12-118">allowCurrentWebSite</span><span class="sxs-lookup"><span data-stu-id="4dd12-118">allowCurrentWebSite</span></span>|<span data-ttu-id="4dd12-119">2</span><span class="sxs-lookup"><span data-stu-id="4dd12-119">2</span></span>|<span data-ttu-id="4dd12-120">允许从当前网站的 cookie。</span><span class="sxs-lookup"><span data-stu-id="4dd12-120">Allow cookies from current Web site.</span></span>|
|<span data-ttu-id="4dd12-121">allowFromWebsitesVisited</span><span class="sxs-lookup"><span data-stu-id="4dd12-121">allowFromWebsitesVisited</span></span>|<span data-ttu-id="4dd12-122">3</span><span class="sxs-lookup"><span data-stu-id="4dd12-122">3</span></span>|<span data-ttu-id="4dd12-123">允许来自访问网站的 Cookie。</span><span class="sxs-lookup"><span data-stu-id="4dd12-123">Allow Cookies from websites visited.</span></span>|
|<span data-ttu-id="4dd12-124">allowAlways</span><span class="sxs-lookup"><span data-stu-id="4dd12-124">allowAlways</span></span>|<span data-ttu-id="4dd12-125">4</span><span class="sxs-lookup"><span data-stu-id="4dd12-125">4</span></span>|<span data-ttu-id="4dd12-126">始终允许 cookie。</span><span class="sxs-lookup"><span data-stu-id="4dd12-126">Always allow cookies.</span></span>|





