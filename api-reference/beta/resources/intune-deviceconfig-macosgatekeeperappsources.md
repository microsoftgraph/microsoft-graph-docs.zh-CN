---
title: macOSGatekeeperAppSources 枚举类型
description: 应用程序 macOS 网关守卫源选项。
ms.openlocfilehash: 97e8159c575c99fe142b67b4c6eeb24642cd0754
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047260"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="17d91-103">macOSGatekeeperAppSources 枚举类型</span><span class="sxs-lookup"><span data-stu-id="17d91-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="17d91-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="17d91-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17d91-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="17d91-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17d91-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="17d91-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17d91-107">应用程序 macOS 网关守卫源选项。</span><span class="sxs-lookup"><span data-stu-id="17d91-107">App source options for macOS Gatekeeper.</span></span>
## <a name="members"></a><span data-ttu-id="17d91-108">成员</span><span class="sxs-lookup"><span data-stu-id="17d91-108">Members</span></span>
|<span data-ttu-id="17d91-109">成员</span><span class="sxs-lookup"><span data-stu-id="17d91-109">Member</span></span>|<span data-ttu-id="17d91-110">值</span><span class="sxs-lookup"><span data-stu-id="17d91-110">Value</span></span>|<span data-ttu-id="17d91-111">说明</span><span class="sxs-lookup"><span data-stu-id="17d91-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17d91-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="17d91-112">notConfigured</span></span>|<span data-ttu-id="17d91-113">0</span><span class="sxs-lookup"><span data-stu-id="17d91-113">0</span></span>|<span data-ttu-id="17d91-114">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="17d91-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="17d91-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="17d91-115">macAppStore</span></span>|<span data-ttu-id="17d91-116">1</span><span class="sxs-lookup"><span data-stu-id="17d91-116">1</span></span>|<span data-ttu-id="17d91-117">可以运行从 Mac AppStore 仅应用程序。</span><span class="sxs-lookup"><span data-stu-id="17d91-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="17d91-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="17d91-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="17d91-119">2</span><span class="sxs-lookup"><span data-stu-id="17d91-119">2</span></span>|<span data-ttu-id="17d91-120">可以运行从 Mac AppStore 和标识的开发人员的唯一应用程序。</span><span class="sxs-lookup"><span data-stu-id="17d91-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="17d91-121">任意位置</span><span class="sxs-lookup"><span data-stu-id="17d91-121">anywhere</span></span>|<span data-ttu-id="17d91-122">3</span><span class="sxs-lookup"><span data-stu-id="17d91-122">3</span></span>|<span data-ttu-id="17d91-123">可以运行从任何位置的应用程序。</span><span class="sxs-lookup"><span data-stu-id="17d91-123">Apps from anywhere can be run.</span></span>|





