---
title: teamSpecialization 枚举类型
description: 描述为团队的特殊的使用情况。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 02a2272ee085d0c265adc9ce2e3f1c598e45be21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930283"
---
# <a name="teamspecialization-enum-type"></a><span data-ttu-id="6dd80-103">teamSpecialization 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6dd80-103">teamSpecialization enum type</span></span>

> <span data-ttu-id="6dd80-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6dd80-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6dd80-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6dd80-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6dd80-106">指示是否[团队](../resources/team.md)适用于特定用例。</span><span class="sxs-lookup"><span data-stu-id="6dd80-106">Indicates whether the [team](../resources/team.md) is intended for a particular use case.</span></span> <span data-ttu-id="6dd80-107">每个[团队](../resources/team.md)具专业性有权访问唯一行为和针对其用例的体验。</span><span class="sxs-lookup"><span data-stu-id="6dd80-107">Each [team](../resources/team.md) specialization has access to unique behaviors and experiences targeted to its use case.</span></span> <span data-ttu-id="6dd80-108">默认值为无。</span><span class="sxs-lookup"><span data-stu-id="6dd80-108">Default is 'none'.</span></span>

## <a name="members"></a><span data-ttu-id="6dd80-109">成员</span><span class="sxs-lookup"><span data-stu-id="6dd80-109">Members</span></span>

| <span data-ttu-id="6dd80-110">成员</span><span class="sxs-lookup"><span data-stu-id="6dd80-110">Member</span></span>             | <span data-ttu-id="6dd80-111">值</span><span class="sxs-lookup"><span data-stu-id="6dd80-111">Value</span></span> | <span data-ttu-id="6dd80-112">Description</span><span class="sxs-lookup"><span data-stu-id="6dd80-112">Description</span></span>                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| <span data-ttu-id="6dd80-113">无</span><span class="sxs-lookup"><span data-stu-id="6dd80-113">none</span></span>               | <span data-ttu-id="6dd80-114">0</span><span class="sxs-lookup"><span data-stu-id="6dd80-114">0</span></span>     | <span data-ttu-id="6dd80-115">默认为团队通过该组件的标准团队体验的类型。</span><span class="sxs-lookup"><span data-stu-id="6dd80-115">Default type for a team which gives the standard team experience.</span></span>          |
| <span data-ttu-id="6dd80-116">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="6dd80-116">unknownFutureValue</span></span> | <span data-ttu-id="6dd80-117">7</span><span class="sxs-lookup"><span data-stu-id="6dd80-117">7</span></span>     | <span data-ttu-id="6dd80-118">Sentinel 保留作为以供将来扩展枚举的占位符值。</span><span class="sxs-lookup"><span data-stu-id="6dd80-118">Sentinel value reserved as a placeholder for future expansion of the enum.</span></span> |
