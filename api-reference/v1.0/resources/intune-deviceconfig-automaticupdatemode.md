---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的的可能值。
author: tfitzmac
ms.openlocfilehash: 01e71e51a47a06aff12dd82e132d7eb468f26229
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346989"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="b0fce-103">automaticUpdateMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b0fce-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="b0fce-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b0fce-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0fce-105">自动更新模式的的可能值。</span><span class="sxs-lookup"><span data-stu-id="b0fce-105">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="b0fce-106">成员</span><span class="sxs-lookup"><span data-stu-id="b0fce-106">Members</span></span>
|<span data-ttu-id="b0fce-107">成员</span><span class="sxs-lookup"><span data-stu-id="b0fce-107">Member</span></span>|<span data-ttu-id="b0fce-108">值</span><span class="sxs-lookup"><span data-stu-id="b0fce-108">Value</span></span>|<span data-ttu-id="b0fce-109">说明</span><span class="sxs-lookup"><span data-stu-id="b0fce-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0fce-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="b0fce-110">userDefined</span></span>|<span data-ttu-id="b0fce-111">0</span><span class="sxs-lookup"><span data-stu-id="b0fce-111">0</span></span>|<span data-ttu-id="b0fce-112">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="b0fce-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="b0fce-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="b0fce-113">notifyDownload</span></span>|<span data-ttu-id="b0fce-114">1</span><span class="sxs-lookup"><span data-stu-id="b0fce-114">1</span></span>|<span data-ttu-id="b0fce-115">在下载通知。</span><span class="sxs-lookup"><span data-stu-id="b0fce-115">Notify on download.</span></span>|
|<span data-ttu-id="b0fce-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="b0fce-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="b0fce-117">2</span><span class="sxs-lookup"><span data-stu-id="b0fce-117">2</span></span>|<span data-ttu-id="b0fce-118">自动安装在维护时间。</span><span class="sxs-lookup"><span data-stu-id="b0fce-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="b0fce-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="b0fce-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="b0fce-120">3</span><span class="sxs-lookup"><span data-stu-id="b0fce-120">3</span></span>|<span data-ttu-id="b0fce-121">自动安装和维护时间重新启动。</span><span class="sxs-lookup"><span data-stu-id="b0fce-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="b0fce-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="b0fce-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="b0fce-123">4</span><span class="sxs-lookup"><span data-stu-id="b0fce-123">4</span></span>|<span data-ttu-id="b0fce-124">自动安装并在计划时间重新启动。</span><span class="sxs-lookup"><span data-stu-id="b0fce-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="b0fce-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="b0fce-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="b0fce-126">5</span><span class="sxs-lookup"><span data-stu-id="b0fce-126">5</span></span>|<span data-ttu-id="b0fce-127">自动安装并重新启动不最终用户控件</span><span class="sxs-lookup"><span data-stu-id="b0fce-127">Auto-install and restart without end-user control</span></span>|



