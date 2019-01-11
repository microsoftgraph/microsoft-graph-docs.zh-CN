---
title: macOSGatekeeperAppSources 枚举类型
description: 应用程序 macOS 网关守卫源选项。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6c784dba6a79b6a9d406e3632d2ac4beaf2a47ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888366"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="c7ba8-103">macOSGatekeeperAppSources 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c7ba8-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="c7ba8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c7ba8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7ba8-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c7ba8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7ba8-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c7ba8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7ba8-107">应用程序 macOS 网关守卫源选项。</span><span class="sxs-lookup"><span data-stu-id="c7ba8-107">App source options for macOS Gatekeeper.</span></span>
## <a name="members"></a><span data-ttu-id="c7ba8-108">成员</span><span class="sxs-lookup"><span data-stu-id="c7ba8-108">Members</span></span>
|<span data-ttu-id="c7ba8-109">成员</span><span class="sxs-lookup"><span data-stu-id="c7ba8-109">Member</span></span>|<span data-ttu-id="c7ba8-110">值</span><span class="sxs-lookup"><span data-stu-id="c7ba8-110">Value</span></span>|<span data-ttu-id="c7ba8-111">Description</span><span class="sxs-lookup"><span data-stu-id="c7ba8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7ba8-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c7ba8-112">notConfigured</span></span>|<span data-ttu-id="c7ba8-113">0</span><span class="sxs-lookup"><span data-stu-id="c7ba8-113">0</span></span>|<span data-ttu-id="c7ba8-114">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="c7ba8-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="c7ba8-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="c7ba8-115">macAppStore</span></span>|<span data-ttu-id="c7ba8-116">1</span><span class="sxs-lookup"><span data-stu-id="c7ba8-116">1</span></span>|<span data-ttu-id="c7ba8-117">可以运行从 Mac AppStore 仅应用程序。</span><span class="sxs-lookup"><span data-stu-id="c7ba8-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="c7ba8-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="c7ba8-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="c7ba8-119">2</span><span class="sxs-lookup"><span data-stu-id="c7ba8-119">2</span></span>|<span data-ttu-id="c7ba8-120">可以运行从 Mac AppStore 和标识的开发人员的唯一应用程序。</span><span class="sxs-lookup"><span data-stu-id="c7ba8-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="c7ba8-121">任意位置</span><span class="sxs-lookup"><span data-stu-id="c7ba8-121">anywhere</span></span>|<span data-ttu-id="c7ba8-122">3</span><span class="sxs-lookup"><span data-stu-id="c7ba8-122">3</span></span>|<span data-ttu-id="c7ba8-123">可以运行从任何位置的应用程序。</span><span class="sxs-lookup"><span data-stu-id="c7ba8-123">Apps from anywhere can be run.</span></span>|





