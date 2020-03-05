---
title: defenderPotentiallyUnwantedAppAction 枚举类型
description: 要对检测到的可能有害的应用程序（PUA）执行的 Defender 操作。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4eeadad81c86217048590cff73a212e830e1f94f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526885"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="4da9c-103">defenderPotentiallyUnwantedAppAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4da9c-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

<span data-ttu-id="4da9c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4da9c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4da9c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4da9c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4da9c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4da9c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4da9c-107">要对检测到的可能有害的应用程序（PUA）执行的 Defender 操作。</span><span class="sxs-lookup"><span data-stu-id="4da9c-107">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="4da9c-108">成员</span><span class="sxs-lookup"><span data-stu-id="4da9c-108">Members</span></span>
|<span data-ttu-id="4da9c-109">成员</span><span class="sxs-lookup"><span data-stu-id="4da9c-109">Member</span></span>|<span data-ttu-id="4da9c-110">值</span><span class="sxs-lookup"><span data-stu-id="4da9c-110">Value</span></span>|<span data-ttu-id="4da9c-111">说明</span><span class="sxs-lookup"><span data-stu-id="4da9c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4da9c-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="4da9c-112">deviceDefault</span></span>|<span data-ttu-id="4da9c-113">0</span><span class="sxs-lookup"><span data-stu-id="4da9c-113">0</span></span>|<span data-ttu-id="4da9c-114">PUA 保护已关闭。</span><span class="sxs-lookup"><span data-stu-id="4da9c-114">PUA Protection is off.</span></span> <span data-ttu-id="4da9c-115">Defender 将无法抵御可能有害的应用程序。</span><span class="sxs-lookup"><span data-stu-id="4da9c-115">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="4da9c-116">数据</span><span class="sxs-lookup"><span data-stu-id="4da9c-116">block</span></span>|<span data-ttu-id="4da9c-117">1 </span><span class="sxs-lookup"><span data-stu-id="4da9c-117">1</span></span>|<span data-ttu-id="4da9c-118">PUA 保护已开启。</span><span class="sxs-lookup"><span data-stu-id="4da9c-118">PUA Protection is on.</span></span> <span data-ttu-id="4da9c-119">已检测到的项目被阻止。</span><span class="sxs-lookup"><span data-stu-id="4da9c-119">Detected items are blocked.</span></span> <span data-ttu-id="4da9c-120">它们将显示在历史记录中，以及其他威胁。</span><span class="sxs-lookup"><span data-stu-id="4da9c-120">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="4da9c-121">跟踪</span><span class="sxs-lookup"><span data-stu-id="4da9c-121">audit</span></span>|<span data-ttu-id="4da9c-122">2 </span><span class="sxs-lookup"><span data-stu-id="4da9c-122">2</span></span>|<span data-ttu-id="4da9c-123">审核模式。</span><span class="sxs-lookup"><span data-stu-id="4da9c-123">Audit mode.</span></span> <span data-ttu-id="4da9c-124">Defender 将检测可能有害的应用程序，但不执行任何操作。</span><span class="sxs-lookup"><span data-stu-id="4da9c-124">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="4da9c-125">您可以通过在事件查看器中搜索由 Defender 创建的事件，查看有关应用程序 Defender 执行操作的相关信息。</span><span class="sxs-lookup"><span data-stu-id="4da9c-125">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|



