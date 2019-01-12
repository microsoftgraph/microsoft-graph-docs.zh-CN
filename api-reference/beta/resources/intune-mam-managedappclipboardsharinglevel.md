---
title: managedAppClipboardSharingLevel 枚举类型
description: 代表到设备的剪贴板可能共享应用程序之间的级别
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 41983b9bb30880768fff0ee02883c32fcb5305a6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968413"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="909e4-103">managedAppClipboardSharingLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="909e4-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="909e4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="909e4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="909e4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="909e4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="909e4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="909e4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="909e4-107">代表到设备的剪贴板可能共享应用程序之间的级别</span><span class="sxs-lookup"><span data-stu-id="909e4-107">Represents the level to which the device's clipboard may be shared between apps</span></span>
## <a name="members"></a><span data-ttu-id="909e4-108">成员</span><span class="sxs-lookup"><span data-stu-id="909e4-108">Members</span></span>
|<span data-ttu-id="909e4-109">成员</span><span class="sxs-lookup"><span data-stu-id="909e4-109">Member</span></span>|<span data-ttu-id="909e4-110">值</span><span class="sxs-lookup"><span data-stu-id="909e4-110">Value</span></span>|<span data-ttu-id="909e4-111">说明</span><span class="sxs-lookup"><span data-stu-id="909e4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="909e4-112">allApps</span><span class="sxs-lookup"><span data-stu-id="909e4-112">allApps</span></span>|<span data-ttu-id="909e4-113">0</span><span class="sxs-lookup"><span data-stu-id="909e4-113">0</span></span>|<span data-ttu-id="909e4-114">共享之间所有的应用程序、 托管或不允许</span><span class="sxs-lookup"><span data-stu-id="909e4-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="909e4-115">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="909e4-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="909e4-116">1</span><span class="sxs-lookup"><span data-stu-id="909e4-116">1</span></span>|<span data-ttu-id="909e4-117">共享之间不允许与粘贴中的所有托管应用程序启用</span><span class="sxs-lookup"><span data-stu-id="909e4-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="909e4-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="909e4-118">managedApps</span></span>|<span data-ttu-id="909e4-119">2</span><span class="sxs-lookup"><span data-stu-id="909e4-119">2</span></span>|<span data-ttu-id="909e4-120">共享之间所有的托管应用程序不允许</span><span class="sxs-lookup"><span data-stu-id="909e4-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="909e4-121">已阻止</span><span class="sxs-lookup"><span data-stu-id="909e4-121">blocked</span></span>|<span data-ttu-id="909e4-122">3</span><span class="sxs-lookup"><span data-stu-id="909e4-122">3</span></span>|<span data-ttu-id="909e4-123">禁用应用程序之间共享</span><span class="sxs-lookup"><span data-stu-id="909e4-123">Sharing between apps is disabled</span></span>|





