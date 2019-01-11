---
title: win32LobAppReturnCodeType 枚举类型
description: 指示返回代码的类型。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 684aa4f717adb0841c9f6c983c39afee2bf7210a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807299"
---
# <a name="win32lobappreturncodetype-enum-type"></a><span data-ttu-id="fb586-103">win32LobAppReturnCodeType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fb586-103">win32LobAppReturnCodeType enum type</span></span>

> <span data-ttu-id="fb586-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fb586-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb586-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fb586-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb586-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fb586-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb586-107">指示返回代码的类型。</span><span class="sxs-lookup"><span data-stu-id="fb586-107">Indicates the type of return code.</span></span>
## <a name="members"></a><span data-ttu-id="fb586-108">成员</span><span class="sxs-lookup"><span data-stu-id="fb586-108">Members</span></span>
|<span data-ttu-id="fb586-109">成员</span><span class="sxs-lookup"><span data-stu-id="fb586-109">Member</span></span>|<span data-ttu-id="fb586-110">值</span><span class="sxs-lookup"><span data-stu-id="fb586-110">Value</span></span>|<span data-ttu-id="fb586-111">Description</span><span class="sxs-lookup"><span data-stu-id="fb586-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb586-112">failed</span><span class="sxs-lookup"><span data-stu-id="fb586-112">failed</span></span>|<span data-ttu-id="fb586-113">0</span><span class="sxs-lookup"><span data-stu-id="fb586-113">0</span></span>|<span data-ttu-id="fb586-114">失败。</span><span class="sxs-lookup"><span data-stu-id="fb586-114">Failed.</span></span>|
|<span data-ttu-id="fb586-115">success</span><span class="sxs-lookup"><span data-stu-id="fb586-115">success</span></span>|<span data-ttu-id="fb586-116">1</span><span class="sxs-lookup"><span data-stu-id="fb586-116">1</span></span>|<span data-ttu-id="fb586-117">成功。</span><span class="sxs-lookup"><span data-stu-id="fb586-117">Success.</span></span>|
|<span data-ttu-id="fb586-118">softReboot</span><span class="sxs-lookup"><span data-stu-id="fb586-118">softReboot</span></span>|<span data-ttu-id="fb586-119">2</span><span class="sxs-lookup"><span data-stu-id="fb586-119">2</span></span>|<span data-ttu-id="fb586-120">软重启是必需的。</span><span class="sxs-lookup"><span data-stu-id="fb586-120">Soft-reboot is required.</span></span>|
|<span data-ttu-id="fb586-121">hardReboot</span><span class="sxs-lookup"><span data-stu-id="fb586-121">hardReboot</span></span>|<span data-ttu-id="fb586-122">3</span><span class="sxs-lookup"><span data-stu-id="fb586-122">3</span></span>|<span data-ttu-id="fb586-123">硬重新启动，则需要。</span><span class="sxs-lookup"><span data-stu-id="fb586-123">Hard-reboot is required.</span></span>|
|<span data-ttu-id="fb586-124">重试</span><span class="sxs-lookup"><span data-stu-id="fb586-124">retry</span></span>|<span data-ttu-id="fb586-125">4</span><span class="sxs-lookup"><span data-stu-id="fb586-125">4</span></span>|<span data-ttu-id="fb586-126">重试。</span><span class="sxs-lookup"><span data-stu-id="fb586-126">Retry.</span></span>|





