---
title: windowsUpdateStatus 枚举类型
description: Windows 更新的业务配置设备状态
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 74493359eeccdbc6df1c351ecec771b5990649b6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431384"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="83fa1-103">windowsUpdateStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="83fa1-103">windowsUpdateStatus enum type</span></span>

> <span data-ttu-id="83fa1-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="83fa1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="83fa1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="83fa1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83fa1-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="83fa1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83fa1-107">Windows 更新的业务配置设备状态</span><span class="sxs-lookup"><span data-stu-id="83fa1-107">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="83fa1-108">成员</span><span class="sxs-lookup"><span data-stu-id="83fa1-108">Members</span></span>
|<span data-ttu-id="83fa1-109">成员</span><span class="sxs-lookup"><span data-stu-id="83fa1-109">Member</span></span>|<span data-ttu-id="83fa1-110">值</span><span class="sxs-lookup"><span data-stu-id="83fa1-110">Value</span></span>|<span data-ttu-id="83fa1-111">说明</span><span class="sxs-lookup"><span data-stu-id="83fa1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83fa1-112">upToDate</span><span class="sxs-lookup"><span data-stu-id="83fa1-112">upToDate</span></span>|<span data-ttu-id="83fa1-113">0</span><span class="sxs-lookup"><span data-stu-id="83fa1-113">0</span></span>|<span data-ttu-id="83fa1-114">待处理更新，没有挂起的重新启动更新和没有失败的更新。</span><span class="sxs-lookup"><span data-stu-id="83fa1-114">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="83fa1-115">pendingInstallation</span><span class="sxs-lookup"><span data-stu-id="83fa1-115">pendingInstallation</span></span>|<span data-ttu-id="83fa1-116">1</span><span class="sxs-lookup"><span data-stu-id="83fa1-116">1</span></span>|<span data-ttu-id="83fa1-117">有的待处理的安装，其中包括未批准的更新的更新。</span><span class="sxs-lookup"><span data-stu-id="83fa1-117">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="83fa1-118">有任何挂起的重新启动更新、 没有失败的更新。</span><span class="sxs-lookup"><span data-stu-id="83fa1-118">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="83fa1-119">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="83fa1-119">pendingReboot</span></span>|<span data-ttu-id="83fa1-120">2</span><span class="sxs-lookup"><span data-stu-id="83fa1-120">2</span></span>|<span data-ttu-id="83fa1-121">有需要重新启动的更新。</span><span class="sxs-lookup"><span data-stu-id="83fa1-121">There are updates that requires reboot.</span></span> <span data-ttu-id="83fa1-122">不存在失败的更新。</span><span class="sxs-lookup"><span data-stu-id="83fa1-122">There are not failed updates.</span></span>|
|<span data-ttu-id="83fa1-123">failed</span><span class="sxs-lookup"><span data-stu-id="83fa1-123">failed</span></span>|<span data-ttu-id="83fa1-124">3</span><span class="sxs-lookup"><span data-stu-id="83fa1-124">3</span></span>|<span data-ttu-id="83fa1-125">有未能在设备上安装更新。</span><span class="sxs-lookup"><span data-stu-id="83fa1-125">There are updates failed to install on the device.</span></span>|




