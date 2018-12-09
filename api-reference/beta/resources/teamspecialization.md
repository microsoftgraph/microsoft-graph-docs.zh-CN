---
title: teamSpecialization 枚举类型
description: 描述为团队的特殊的使用情况。
ms.openlocfilehash: 8f50e158e6eedc964226478841c5322eefca9f77
ms.sourcegitcommit: 12c6e82f1417022540e534ebadbd0e8d7fb5abde
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2018
ms.locfileid: "27210136"
---
# <a name="teamspecialization-enum-type"></a><span data-ttu-id="8ba7c-103">teamSpecialization 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8ba7c-103">teamSpecialization enum type</span></span>

> <span data-ttu-id="8ba7c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8ba7c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ba7c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8ba7c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ba7c-106">指示是否[团队](../resources/team.md)适用于特定用例。</span><span class="sxs-lookup"><span data-stu-id="8ba7c-106">Indicates whether the [team](../resources/team.md) is intended for a particular use case.</span></span> <span data-ttu-id="8ba7c-107">每个[团队](../resources/team.md)具专业性有权访问唯一行为和针对其用例的体验。</span><span class="sxs-lookup"><span data-stu-id="8ba7c-107">Each [team](../resources/team.md) specialization has access to unique behaviors and experiences targeted to its use case.</span></span> <span data-ttu-id="8ba7c-108">默认值为无。</span><span class="sxs-lookup"><span data-stu-id="8ba7c-108">Default is 'none'.</span></span>

## <a name="members"></a><span data-ttu-id="8ba7c-109">成员</span><span class="sxs-lookup"><span data-stu-id="8ba7c-109">Members</span></span>

| <span data-ttu-id="8ba7c-110">成员</span><span class="sxs-lookup"><span data-stu-id="8ba7c-110">Member</span></span>             | <span data-ttu-id="8ba7c-111">值</span><span class="sxs-lookup"><span data-stu-id="8ba7c-111">Value</span></span> | <span data-ttu-id="8ba7c-112">说明</span><span class="sxs-lookup"><span data-stu-id="8ba7c-112">Description</span></span>                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| <span data-ttu-id="8ba7c-113">无</span><span class="sxs-lookup"><span data-stu-id="8ba7c-113">none</span></span>               | <span data-ttu-id="8ba7c-114">0</span><span class="sxs-lookup"><span data-stu-id="8ba7c-114">0</span></span>     | <span data-ttu-id="8ba7c-115">默认为团队通过该组件的标准团队体验的类型。</span><span class="sxs-lookup"><span data-stu-id="8ba7c-115">Default type for a team which gives the standard team experience.</span></span>          |
| <span data-ttu-id="8ba7c-116">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="8ba7c-116">unknownFutureValue</span></span> | <span data-ttu-id="8ba7c-117">7</span><span class="sxs-lookup"><span data-stu-id="8ba7c-117">7</span></span>     | <span data-ttu-id="8ba7c-118">Sentinel 保留作为以供将来扩展枚举的占位符值。</span><span class="sxs-lookup"><span data-stu-id="8ba7c-118">Sentinel value reserved as a placeholder for future expansion of the enum.</span></span> |
