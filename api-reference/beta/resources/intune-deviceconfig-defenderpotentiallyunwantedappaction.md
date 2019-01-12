---
title: defenderPotentiallyUnwantedAppAction 枚举类型
description: Defender 的操作，才能检测到可能有害的应用程序 (PUA)。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 96a3dd70ae0f56f2d0d5a9d6c4f87846e10bba45
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938557"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="4da08-103">defenderPotentiallyUnwantedAppAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4da08-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="4da08-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4da08-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4da08-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4da08-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4da08-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4da08-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4da08-107">Defender 的操作，才能检测到可能有害的应用程序 (PUA)。</span><span class="sxs-lookup"><span data-stu-id="4da08-107">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>
## <a name="members"></a><span data-ttu-id="4da08-108">成员</span><span class="sxs-lookup"><span data-stu-id="4da08-108">Members</span></span>
|<span data-ttu-id="4da08-109">成员</span><span class="sxs-lookup"><span data-stu-id="4da08-109">Member</span></span>|<span data-ttu-id="4da08-110">值</span><span class="sxs-lookup"><span data-stu-id="4da08-110">Value</span></span>|<span data-ttu-id="4da08-111">说明</span><span class="sxs-lookup"><span data-stu-id="4da08-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4da08-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="4da08-112">deviceDefault</span></span>|<span data-ttu-id="4da08-113">0</span><span class="sxs-lookup"><span data-stu-id="4da08-113">0</span></span>|<span data-ttu-id="4da08-114">PUA 保护处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="4da08-114">PUA Protection is off.</span></span> <span data-ttu-id="4da08-115">Defender 将不能防范可能有害的应用程序。</span><span class="sxs-lookup"><span data-stu-id="4da08-115">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="4da08-116">阻止</span><span class="sxs-lookup"><span data-stu-id="4da08-116">block</span></span>|<span data-ttu-id="4da08-117">1</span><span class="sxs-lookup"><span data-stu-id="4da08-117">1</span></span>|<span data-ttu-id="4da08-118">在 PUA 保护。</span><span class="sxs-lookup"><span data-stu-id="4da08-118">PUA Protection is on.</span></span> <span data-ttu-id="4da08-119">检测到的项目会被阻止。</span><span class="sxs-lookup"><span data-stu-id="4da08-119">Detected items are blocked.</span></span> <span data-ttu-id="4da08-120">它们将显示以及其他威胁的历史记录中。</span><span class="sxs-lookup"><span data-stu-id="4da08-120">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="4da08-121">审核</span><span class="sxs-lookup"><span data-stu-id="4da08-121">audit</span></span>|<span data-ttu-id="4da08-122">2</span><span class="sxs-lookup"><span data-stu-id="4da08-122">2</span></span>|<span data-ttu-id="4da08-123">审核模式。</span><span class="sxs-lookup"><span data-stu-id="4da08-123">Audit mode.</span></span> <span data-ttu-id="4da08-124">Defender 将检测可能有害的应用程序，但不需要任何操作。</span><span class="sxs-lookup"><span data-stu-id="4da08-124">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="4da08-125">您可以查看有关应用程序的信息 Defender 可能需要花费针对操作，通过搜索创建的 Defender 在事件查看器事件。</span><span class="sxs-lookup"><span data-stu-id="4da08-125">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|





