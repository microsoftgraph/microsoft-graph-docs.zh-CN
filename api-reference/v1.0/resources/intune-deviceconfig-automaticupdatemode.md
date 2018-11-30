---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的的可能值。
ms.openlocfilehash: c98927e1c1f66e3bf10fa07496aa54ac91bad20b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008077"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="b0c09-103">automaticUpdateMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b0c09-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="b0c09-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b0c09-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0c09-105">自动更新模式的的可能值。</span><span class="sxs-lookup"><span data-stu-id="b0c09-105">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="b0c09-106">成员</span><span class="sxs-lookup"><span data-stu-id="b0c09-106">Members</span></span>
|<span data-ttu-id="b0c09-107">成员</span><span class="sxs-lookup"><span data-stu-id="b0c09-107">Member</span></span>|<span data-ttu-id="b0c09-108">值</span><span class="sxs-lookup"><span data-stu-id="b0c09-108">Value</span></span>|<span data-ttu-id="b0c09-109">说明</span><span class="sxs-lookup"><span data-stu-id="b0c09-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0c09-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="b0c09-110">userDefined</span></span>|<span data-ttu-id="b0c09-111">0</span><span class="sxs-lookup"><span data-stu-id="b0c09-111">0</span></span>|<span data-ttu-id="b0c09-112">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="b0c09-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="b0c09-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="b0c09-113">notifyDownload</span></span>|<span data-ttu-id="b0c09-114">1</span><span class="sxs-lookup"><span data-stu-id="b0c09-114">1</span></span>|<span data-ttu-id="b0c09-115">在下载通知。</span><span class="sxs-lookup"><span data-stu-id="b0c09-115">Notify on download.</span></span>|
|<span data-ttu-id="b0c09-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="b0c09-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="b0c09-117">2</span><span class="sxs-lookup"><span data-stu-id="b0c09-117">2</span></span>|<span data-ttu-id="b0c09-118">自动安装在维护时间。</span><span class="sxs-lookup"><span data-stu-id="b0c09-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="b0c09-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="b0c09-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="b0c09-120">3</span><span class="sxs-lookup"><span data-stu-id="b0c09-120">3</span></span>|<span data-ttu-id="b0c09-121">自动安装和维护时间重新启动。</span><span class="sxs-lookup"><span data-stu-id="b0c09-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="b0c09-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="b0c09-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="b0c09-123">4</span><span class="sxs-lookup"><span data-stu-id="b0c09-123">4</span></span>|<span data-ttu-id="b0c09-124">自动安装并在计划时间重新启动。</span><span class="sxs-lookup"><span data-stu-id="b0c09-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="b0c09-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="b0c09-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="b0c09-126">5</span><span class="sxs-lookup"><span data-stu-id="b0c09-126">5</span></span>|<span data-ttu-id="b0c09-127">自动安装并重新启动不最终用户控件</span><span class="sxs-lookup"><span data-stu-id="b0c09-127">Auto-install and restart without end-user control</span></span>|



