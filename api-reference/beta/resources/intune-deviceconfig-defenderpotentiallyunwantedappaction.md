---
title: defenderPotentiallyUnwantedAppAction 枚举类型
description: 要对检测到的可能有害的应用程序（PUA）执行的 Defender 操作。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0c99cf04b217239fb1a06b2a6c26dcacc6c61cf7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42794464"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="b9354-103">defenderPotentiallyUnwantedAppAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b9354-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="b9354-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b9354-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9354-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9354-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9354-106">要对检测到的可能有害的应用程序（PUA）执行的 Defender 操作。</span><span class="sxs-lookup"><span data-stu-id="b9354-106">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="b9354-107">成员</span><span class="sxs-lookup"><span data-stu-id="b9354-107">Members</span></span>
|<span data-ttu-id="b9354-108">成员</span><span class="sxs-lookup"><span data-stu-id="b9354-108">Member</span></span>|<span data-ttu-id="b9354-109">值</span><span class="sxs-lookup"><span data-stu-id="b9354-109">Value</span></span>|<span data-ttu-id="b9354-110">说明</span><span class="sxs-lookup"><span data-stu-id="b9354-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9354-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b9354-111">deviceDefault</span></span>|<span data-ttu-id="b9354-112">0</span><span class="sxs-lookup"><span data-stu-id="b9354-112">0</span></span>|<span data-ttu-id="b9354-113">PUA 保护已关闭。</span><span class="sxs-lookup"><span data-stu-id="b9354-113">PUA Protection is off.</span></span> <span data-ttu-id="b9354-114">Defender 将无法抵御可能有害的应用程序。</span><span class="sxs-lookup"><span data-stu-id="b9354-114">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="b9354-115">数据</span><span class="sxs-lookup"><span data-stu-id="b9354-115">block</span></span>|<span data-ttu-id="b9354-116">1</span><span class="sxs-lookup"><span data-stu-id="b9354-116">1</span></span>|<span data-ttu-id="b9354-117">PUA 保护已开启。</span><span class="sxs-lookup"><span data-stu-id="b9354-117">PUA Protection is on.</span></span> <span data-ttu-id="b9354-118">已检测到的项目被阻止。</span><span class="sxs-lookup"><span data-stu-id="b9354-118">Detected items are blocked.</span></span> <span data-ttu-id="b9354-119">它们将显示在历史记录中，以及其他威胁。</span><span class="sxs-lookup"><span data-stu-id="b9354-119">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="b9354-120">跟踪</span><span class="sxs-lookup"><span data-stu-id="b9354-120">audit</span></span>|<span data-ttu-id="b9354-121">双面</span><span class="sxs-lookup"><span data-stu-id="b9354-121">2</span></span>|<span data-ttu-id="b9354-122">审核模式。</span><span class="sxs-lookup"><span data-stu-id="b9354-122">Audit mode.</span></span> <span data-ttu-id="b9354-123">Defender 将检测可能有害的应用程序，但不执行任何操作。</span><span class="sxs-lookup"><span data-stu-id="b9354-123">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="b9354-124">您可以通过在事件查看器中搜索由 Defender 创建的事件，查看有关应用程序 Defender 执行操作的相关信息。</span><span class="sxs-lookup"><span data-stu-id="b9354-124">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|



