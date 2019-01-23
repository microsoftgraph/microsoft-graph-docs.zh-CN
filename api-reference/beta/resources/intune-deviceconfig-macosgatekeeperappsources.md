---
title: macOSGatekeeperAppSources 枚举类型
description: 应用程序 macOS 网关守卫源选项。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 18ab6884d211faccb81e93a40ee91f742d03475f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394388"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="c6dd7-103">macOSGatekeeperAppSources 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c6dd7-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="c6dd7-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c6dd7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c6dd7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c6dd7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6dd7-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c6dd7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6dd7-107">应用程序 macOS 网关守卫源选项。</span><span class="sxs-lookup"><span data-stu-id="c6dd7-107">App source options for macOS Gatekeeper.</span></span>

## <a name="members"></a><span data-ttu-id="c6dd7-108">成员</span><span class="sxs-lookup"><span data-stu-id="c6dd7-108">Members</span></span>
|<span data-ttu-id="c6dd7-109">成员</span><span class="sxs-lookup"><span data-stu-id="c6dd7-109">Member</span></span>|<span data-ttu-id="c6dd7-110">值</span><span class="sxs-lookup"><span data-stu-id="c6dd7-110">Value</span></span>|<span data-ttu-id="c6dd7-111">说明</span><span class="sxs-lookup"><span data-stu-id="c6dd7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6dd7-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c6dd7-112">notConfigured</span></span>|<span data-ttu-id="c6dd7-113">0</span><span class="sxs-lookup"><span data-stu-id="c6dd7-113">0</span></span>|<span data-ttu-id="c6dd7-114">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="c6dd7-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="c6dd7-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="c6dd7-115">macAppStore</span></span>|<span data-ttu-id="c6dd7-116">1</span><span class="sxs-lookup"><span data-stu-id="c6dd7-116">1</span></span>|<span data-ttu-id="c6dd7-117">可以运行从 Mac AppStore 仅应用程序。</span><span class="sxs-lookup"><span data-stu-id="c6dd7-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="c6dd7-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="c6dd7-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="c6dd7-119">2</span><span class="sxs-lookup"><span data-stu-id="c6dd7-119">2</span></span>|<span data-ttu-id="c6dd7-120">可以运行从 Mac AppStore 和标识的开发人员的唯一应用程序。</span><span class="sxs-lookup"><span data-stu-id="c6dd7-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="c6dd7-121">任意位置</span><span class="sxs-lookup"><span data-stu-id="c6dd7-121">anywhere</span></span>|<span data-ttu-id="c6dd7-122">3</span><span class="sxs-lookup"><span data-stu-id="c6dd7-122">3</span></span>|<span data-ttu-id="c6dd7-123">可以运行从任何位置的应用程序。</span><span class="sxs-lookup"><span data-stu-id="c6dd7-123">Apps from anywhere can be run.</span></span>|




