---
title: macOSGatekeeperAppSources 枚举类型
description: 应用程序 macOS 网关守卫源选项。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5c2c1d553408b7269a53f9fc3500493a44bc3645
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918112"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="a4df4-103">macOSGatekeeperAppSources 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a4df4-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="a4df4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a4df4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4df4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a4df4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a4df4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a4df4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4df4-107">应用程序 macOS 网关守卫源选项。</span><span class="sxs-lookup"><span data-stu-id="a4df4-107">App source options for macOS Gatekeeper.</span></span>
## <a name="members"></a><span data-ttu-id="a4df4-108">成员</span><span class="sxs-lookup"><span data-stu-id="a4df4-108">Members</span></span>
|<span data-ttu-id="a4df4-109">成员</span><span class="sxs-lookup"><span data-stu-id="a4df4-109">Member</span></span>|<span data-ttu-id="a4df4-110">值</span><span class="sxs-lookup"><span data-stu-id="a4df4-110">Value</span></span>|<span data-ttu-id="a4df4-111">Description</span><span class="sxs-lookup"><span data-stu-id="a4df4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4df4-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a4df4-112">notConfigured</span></span>|<span data-ttu-id="a4df4-113">0</span><span class="sxs-lookup"><span data-stu-id="a4df4-113">0</span></span>|<span data-ttu-id="a4df4-114">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="a4df4-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="a4df4-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="a4df4-115">macAppStore</span></span>|<span data-ttu-id="a4df4-116">1</span><span class="sxs-lookup"><span data-stu-id="a4df4-116">1</span></span>|<span data-ttu-id="a4df4-117">可以运行从 Mac AppStore 仅应用程序。</span><span class="sxs-lookup"><span data-stu-id="a4df4-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="a4df4-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="a4df4-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="a4df4-119">2</span><span class="sxs-lookup"><span data-stu-id="a4df4-119">2</span></span>|<span data-ttu-id="a4df4-120">可以运行从 Mac AppStore 和标识的开发人员的唯一应用程序。</span><span class="sxs-lookup"><span data-stu-id="a4df4-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="a4df4-121">任意位置</span><span class="sxs-lookup"><span data-stu-id="a4df4-121">anywhere</span></span>|<span data-ttu-id="a4df4-122">3</span><span class="sxs-lookup"><span data-stu-id="a4df4-122">3</span></span>|<span data-ttu-id="a4df4-123">可以运行从任何位置的应用程序。</span><span class="sxs-lookup"><span data-stu-id="a4df4-123">Apps from anywhere can be run.</span></span>|





