---
title: managedAppClipboardSharingLevel 枚举类型
description: 表示设备剪贴板可以在应用之间共享的级别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 28a5d906342cc240d2382ed18c6de572e316f886
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754502"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="9db18-103">managedAppClipboardSharingLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9db18-103">managedAppClipboardSharingLevel enum type</span></span>

<span data-ttu-id="9db18-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9db18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9db18-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9db18-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9db18-106">表示设备剪贴板可以在应用之间共享的级别</span><span class="sxs-lookup"><span data-stu-id="9db18-106">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="9db18-107">成员</span><span class="sxs-lookup"><span data-stu-id="9db18-107">Members</span></span>
|<span data-ttu-id="9db18-108">成员</span><span class="sxs-lookup"><span data-stu-id="9db18-108">Member</span></span>|<span data-ttu-id="9db18-109">值</span><span class="sxs-lookup"><span data-stu-id="9db18-109">Value</span></span>|<span data-ttu-id="9db18-110">说明</span><span class="sxs-lookup"><span data-stu-id="9db18-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9db18-111">allApps</span><span class="sxs-lookup"><span data-stu-id="9db18-111">allApps</span></span>|<span data-ttu-id="9db18-112">0</span><span class="sxs-lookup"><span data-stu-id="9db18-112">0</span></span>|<span data-ttu-id="9db18-113">是否允许在所有应用之间共享（托管或不共享）</span><span class="sxs-lookup"><span data-stu-id="9db18-113">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="9db18-114">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="9db18-114">managedAppsWithPasteIn</span></span>|<span data-ttu-id="9db18-115">1</span><span class="sxs-lookup"><span data-stu-id="9db18-115">1</span></span>|<span data-ttu-id="9db18-116">允许所有已启用粘贴的托管应用之间共享</span><span class="sxs-lookup"><span data-stu-id="9db18-116">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="9db18-117">managedApps</span><span class="sxs-lookup"><span data-stu-id="9db18-117">managedApps</span></span>|<span data-ttu-id="9db18-118">2</span><span class="sxs-lookup"><span data-stu-id="9db18-118">2</span></span>|<span data-ttu-id="9db18-119">允许在所有托管应用之间共享</span><span class="sxs-lookup"><span data-stu-id="9db18-119">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="9db18-120">blocked</span><span class="sxs-lookup"><span data-stu-id="9db18-120">blocked</span></span>|<span data-ttu-id="9db18-121">3</span><span class="sxs-lookup"><span data-stu-id="9db18-121">3</span></span>|<span data-ttu-id="9db18-122">禁用应用之间的共享</span><span class="sxs-lookup"><span data-stu-id="9db18-122">Sharing between apps is disabled</span></span>|




