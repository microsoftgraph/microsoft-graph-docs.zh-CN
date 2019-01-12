---
title: managedAppClipboardSharingLevel 枚举类型
description: 代表到设备的剪贴板可能共享应用程序之间的级别
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 349f0ee08b8e3bff4e627c58318e2c21fa00847c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946782"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="48770-103">managedAppClipboardSharingLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="48770-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="48770-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="48770-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48770-105">代表到设备的剪贴板可能共享应用程序之间的级别</span><span class="sxs-lookup"><span data-stu-id="48770-105">Represents the level to which the device's clipboard may be shared between apps</span></span>
## <a name="members"></a><span data-ttu-id="48770-106">成员</span><span class="sxs-lookup"><span data-stu-id="48770-106">Members</span></span>
|<span data-ttu-id="48770-107">成员</span><span class="sxs-lookup"><span data-stu-id="48770-107">Member</span></span>|<span data-ttu-id="48770-108">值</span><span class="sxs-lookup"><span data-stu-id="48770-108">Value</span></span>|<span data-ttu-id="48770-109">Description</span><span class="sxs-lookup"><span data-stu-id="48770-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48770-110">allApps</span><span class="sxs-lookup"><span data-stu-id="48770-110">allApps</span></span>|<span data-ttu-id="48770-111">0</span><span class="sxs-lookup"><span data-stu-id="48770-111">0</span></span>|<span data-ttu-id="48770-112">共享之间所有的应用程序、 托管或不允许</span><span class="sxs-lookup"><span data-stu-id="48770-112">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="48770-113">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="48770-113">managedAppsWithPasteIn</span></span>|<span data-ttu-id="48770-114">1</span><span class="sxs-lookup"><span data-stu-id="48770-114">1</span></span>|<span data-ttu-id="48770-115">共享之间不允许与粘贴中的所有托管应用程序启用</span><span class="sxs-lookup"><span data-stu-id="48770-115">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="48770-116">managedApps</span><span class="sxs-lookup"><span data-stu-id="48770-116">managedApps</span></span>|<span data-ttu-id="48770-117">2</span><span class="sxs-lookup"><span data-stu-id="48770-117">2</span></span>|<span data-ttu-id="48770-118">共享之间所有的托管应用程序不允许</span><span class="sxs-lookup"><span data-stu-id="48770-118">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="48770-119">已阻止</span><span class="sxs-lookup"><span data-stu-id="48770-119">blocked</span></span>|<span data-ttu-id="48770-120">3</span><span class="sxs-lookup"><span data-stu-id="48770-120">3</span></span>|<span data-ttu-id="48770-121">禁用应用程序之间共享</span><span class="sxs-lookup"><span data-stu-id="48770-121">Sharing between apps is disabled</span></span>|



