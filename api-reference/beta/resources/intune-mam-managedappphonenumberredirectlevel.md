---
title: managedAppPhoneNumberRedirectLevel 枚举类型
description: 允许单击以打开电话号码的应用程序的类，用于电话呼叫或发送短信。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1b0e37364bd505dada24d0283477742f70183b83
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722807"
---
# <a name="managedappphonenumberredirectlevel-enum-type"></a><span data-ttu-id="e558e-103">managedAppPhoneNumberRedirectLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e558e-103">managedAppPhoneNumberRedirectLevel enum type</span></span>

<span data-ttu-id="e558e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e558e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e558e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e558e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e558e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e558e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e558e-107">允许单击以打开电话号码的应用程序的类，用于电话呼叫或发送短信。</span><span class="sxs-lookup"><span data-stu-id="e558e-107">The classes of apps that are allowed to click-to-open a phone number, for making phone calls or sending text messages.</span></span>

## <a name="members"></a><span data-ttu-id="e558e-108">成员</span><span class="sxs-lookup"><span data-stu-id="e558e-108">Members</span></span>
|<span data-ttu-id="e558e-109">成员</span><span class="sxs-lookup"><span data-stu-id="e558e-109">Member</span></span>|<span data-ttu-id="e558e-110">值</span><span class="sxs-lookup"><span data-stu-id="e558e-110">Value</span></span>|<span data-ttu-id="e558e-111">说明</span><span class="sxs-lookup"><span data-stu-id="e558e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e558e-112">allApps</span><span class="sxs-lookup"><span data-stu-id="e558e-112">allApps</span></span>|<span data-ttu-id="e558e-113">0</span><span class="sxs-lookup"><span data-stu-id="e558e-113">0</span></span>|<span data-ttu-id="e558e-114">允许共享所有应用。</span><span class="sxs-lookup"><span data-stu-id="e558e-114">Sharing is allowed to all apps.</span></span>|
|<span data-ttu-id="e558e-115">managedApps</span><span class="sxs-lookup"><span data-stu-id="e558e-115">managedApps</span></span>|<span data-ttu-id="e558e-116">1</span><span class="sxs-lookup"><span data-stu-id="e558e-116">1</span></span>|<span data-ttu-id="e558e-117">允许对所有托管应用进行共享。</span><span class="sxs-lookup"><span data-stu-id="e558e-117">Sharing is allowed to all managed apps.</span></span>|
|<span data-ttu-id="e558e-118">Customapp.baz</span><span class="sxs-lookup"><span data-stu-id="e558e-118">customApp</span></span>|<span data-ttu-id="e558e-119">双面</span><span class="sxs-lookup"><span data-stu-id="e558e-119">2</span></span>|<span data-ttu-id="e558e-120">允许共享到自定义应用程序。</span><span class="sxs-lookup"><span data-stu-id="e558e-120">Sharing is allowed to a custom app.</span></span>|
|<span data-ttu-id="e558e-121">堵塞</span><span class="sxs-lookup"><span data-stu-id="e558e-121">blocked</span></span>|<span data-ttu-id="e558e-122">第三章</span><span class="sxs-lookup"><span data-stu-id="e558e-122">3</span></span>|<span data-ttu-id="e558e-123">阻止在应用之间共享。</span><span class="sxs-lookup"><span data-stu-id="e558e-123">Sharing between apps is blocked.</span></span>|





