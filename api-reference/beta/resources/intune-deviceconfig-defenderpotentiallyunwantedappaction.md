---
title: defenderPotentiallyUnwantedAppAction 枚举类型
description: Defender 的操作，才能检测到可能有害的应用程序 (PUA)。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2ace0cc29ad284cde63b7e4934fb8cb395f27bbe
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422752"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a><span data-ttu-id="abc27-103">defenderPotentiallyUnwantedAppAction 枚举类型</span><span class="sxs-lookup"><span data-stu-id="abc27-103">defenderPotentiallyUnwantedAppAction enum type</span></span>

> <span data-ttu-id="abc27-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="abc27-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="abc27-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="abc27-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="abc27-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="abc27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abc27-107">Defender 的操作，才能检测到可能有害的应用程序 (PUA)。</span><span class="sxs-lookup"><span data-stu-id="abc27-107">Defender’s action to take on detected Potentially Unwanted Application (PUA).</span></span>

## <a name="members"></a><span data-ttu-id="abc27-108">成员</span><span class="sxs-lookup"><span data-stu-id="abc27-108">Members</span></span>
|<span data-ttu-id="abc27-109">成员</span><span class="sxs-lookup"><span data-stu-id="abc27-109">Member</span></span>|<span data-ttu-id="abc27-110">值</span><span class="sxs-lookup"><span data-stu-id="abc27-110">Value</span></span>|<span data-ttu-id="abc27-111">说明</span><span class="sxs-lookup"><span data-stu-id="abc27-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abc27-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="abc27-112">deviceDefault</span></span>|<span data-ttu-id="abc27-113">0</span><span class="sxs-lookup"><span data-stu-id="abc27-113">0</span></span>|<span data-ttu-id="abc27-114">PUA 保护处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="abc27-114">PUA Protection is off.</span></span> <span data-ttu-id="abc27-115">Defender 将不能防范可能有害的应用程序。</span><span class="sxs-lookup"><span data-stu-id="abc27-115">Defender will not protect against potentially unwanted applications.</span></span>|
|<span data-ttu-id="abc27-116">阻止</span><span class="sxs-lookup"><span data-stu-id="abc27-116">block</span></span>|<span data-ttu-id="abc27-117">1</span><span class="sxs-lookup"><span data-stu-id="abc27-117">1</span></span>|<span data-ttu-id="abc27-118">在 PUA 保护。</span><span class="sxs-lookup"><span data-stu-id="abc27-118">PUA Protection is on.</span></span> <span data-ttu-id="abc27-119">检测到的项目会被阻止。</span><span class="sxs-lookup"><span data-stu-id="abc27-119">Detected items are blocked.</span></span> <span data-ttu-id="abc27-120">它们将显示以及其他威胁的历史记录中。</span><span class="sxs-lookup"><span data-stu-id="abc27-120">They will show in history along with other threats.</span></span>|
|<span data-ttu-id="abc27-121">审核</span><span class="sxs-lookup"><span data-stu-id="abc27-121">audit</span></span>|<span data-ttu-id="abc27-122">2</span><span class="sxs-lookup"><span data-stu-id="abc27-122">2</span></span>|<span data-ttu-id="abc27-123">审核模式。</span><span class="sxs-lookup"><span data-stu-id="abc27-123">Audit mode.</span></span> <span data-ttu-id="abc27-124">Defender 将检测可能有害的应用程序，但不需要任何操作。</span><span class="sxs-lookup"><span data-stu-id="abc27-124">Defender will detect potentially unwanted applications, but take no actions.</span></span> <span data-ttu-id="abc27-125">您可以查看有关应用程序的信息 Defender 可能需要花费针对操作，通过搜索创建的 Defender 在事件查看器事件。</span><span class="sxs-lookup"><span data-stu-id="abc27-125">You can review information about applications Defender would have taken action against by searching for events created by Defender in the Event Viewer.</span></span>|




