---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的的可能值。
author: tfitzmac
ms.openlocfilehash: d1bf3903b71dbd06be9151d67a925f374eb1f803
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344042"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="cc79c-103">automaticUpdateMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cc79c-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="cc79c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cc79c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc79c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cc79c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc79c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cc79c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc79c-107">自动更新模式的的可能值。</span><span class="sxs-lookup"><span data-stu-id="cc79c-107">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="cc79c-108">成员</span><span class="sxs-lookup"><span data-stu-id="cc79c-108">Members</span></span>
|<span data-ttu-id="cc79c-109">成员</span><span class="sxs-lookup"><span data-stu-id="cc79c-109">Member</span></span>|<span data-ttu-id="cc79c-110">值</span><span class="sxs-lookup"><span data-stu-id="cc79c-110">Value</span></span>|<span data-ttu-id="cc79c-111">说明</span><span class="sxs-lookup"><span data-stu-id="cc79c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc79c-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="cc79c-112">userDefined</span></span>|<span data-ttu-id="cc79c-113">0</span><span class="sxs-lookup"><span data-stu-id="cc79c-113">0</span></span>|<span data-ttu-id="cc79c-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="cc79c-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="cc79c-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="cc79c-115">notifyDownload</span></span>|<span data-ttu-id="cc79c-116">1</span><span class="sxs-lookup"><span data-stu-id="cc79c-116">1</span></span>|<span data-ttu-id="cc79c-117">在下载通知。</span><span class="sxs-lookup"><span data-stu-id="cc79c-117">Notify on download.</span></span>|
|<span data-ttu-id="cc79c-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="cc79c-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="cc79c-119">2</span><span class="sxs-lookup"><span data-stu-id="cc79c-119">2</span></span>|<span data-ttu-id="cc79c-120">自动安装在维护时间。</span><span class="sxs-lookup"><span data-stu-id="cc79c-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="cc79c-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="cc79c-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="cc79c-122">3</span><span class="sxs-lookup"><span data-stu-id="cc79c-122">3</span></span>|<span data-ttu-id="cc79c-123">自动安装和维护时间重新启动。</span><span class="sxs-lookup"><span data-stu-id="cc79c-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="cc79c-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="cc79c-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="cc79c-125">4</span><span class="sxs-lookup"><span data-stu-id="cc79c-125">4</span></span>|<span data-ttu-id="cc79c-126">自动安装并在计划时间重新启动。</span><span class="sxs-lookup"><span data-stu-id="cc79c-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="cc79c-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="cc79c-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="cc79c-128">5</span><span class="sxs-lookup"><span data-stu-id="cc79c-128">5</span></span>|<span data-ttu-id="cc79c-129">自动安装并重新启动不最终用户控件</span><span class="sxs-lookup"><span data-stu-id="cc79c-129">Auto-install and restart without end-user control</span></span>|





