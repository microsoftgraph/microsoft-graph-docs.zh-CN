---
title: managedAppClipboardSharingLevel 枚举类型
description: 代表到设备的剪贴板可能共享应用程序之间的级别
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6ccd90e4d704a075eaf43650fa765fabf3ab0b99
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410985"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="2cc9d-103">managedAppClipboardSharingLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2cc9d-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="2cc9d-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="2cc9d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2cc9d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2cc9d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2cc9d-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2cc9d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cc9d-107">代表到设备的剪贴板可能共享应用程序之间的级别</span><span class="sxs-lookup"><span data-stu-id="2cc9d-107">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="2cc9d-108">成员</span><span class="sxs-lookup"><span data-stu-id="2cc9d-108">Members</span></span>
|<span data-ttu-id="2cc9d-109">成员</span><span class="sxs-lookup"><span data-stu-id="2cc9d-109">Member</span></span>|<span data-ttu-id="2cc9d-110">值</span><span class="sxs-lookup"><span data-stu-id="2cc9d-110">Value</span></span>|<span data-ttu-id="2cc9d-111">说明</span><span class="sxs-lookup"><span data-stu-id="2cc9d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cc9d-112">allApps</span><span class="sxs-lookup"><span data-stu-id="2cc9d-112">allApps</span></span>|<span data-ttu-id="2cc9d-113">0</span><span class="sxs-lookup"><span data-stu-id="2cc9d-113">0</span></span>|<span data-ttu-id="2cc9d-114">共享之间所有的应用程序、 托管或不允许</span><span class="sxs-lookup"><span data-stu-id="2cc9d-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="2cc9d-115">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="2cc9d-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="2cc9d-116">1</span><span class="sxs-lookup"><span data-stu-id="2cc9d-116">1</span></span>|<span data-ttu-id="2cc9d-117">共享之间不允许与粘贴中的所有托管应用程序启用</span><span class="sxs-lookup"><span data-stu-id="2cc9d-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="2cc9d-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="2cc9d-118">managedApps</span></span>|<span data-ttu-id="2cc9d-119">2</span><span class="sxs-lookup"><span data-stu-id="2cc9d-119">2</span></span>|<span data-ttu-id="2cc9d-120">共享之间所有的托管应用程序不允许</span><span class="sxs-lookup"><span data-stu-id="2cc9d-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="2cc9d-121">已阻止</span><span class="sxs-lookup"><span data-stu-id="2cc9d-121">blocked</span></span>|<span data-ttu-id="2cc9d-122">3</span><span class="sxs-lookup"><span data-stu-id="2cc9d-122">3</span></span>|<span data-ttu-id="2cc9d-123">禁用应用程序之间共享</span><span class="sxs-lookup"><span data-stu-id="2cc9d-123">Sharing between apps is disabled</span></span>|




