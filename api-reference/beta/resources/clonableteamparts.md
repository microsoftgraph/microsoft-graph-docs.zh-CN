---
title: clonableTeamParts 枚举类型
description: '描述应克隆的工作组的一部分。 '
ms.openlocfilehash: 123cdb5ff7fd4a4291df5d9352b0db466908cc3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042811"
---
# <a name="clonableteamparts-enum-type"></a><span data-ttu-id="49c52-103">clonableTeamParts 枚举类型</span><span class="sxs-lookup"><span data-stu-id="49c52-103">clonableTeamParts enum type</span></span>

> <span data-ttu-id="49c52-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="49c52-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49c52-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="49c52-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="49c52-106">描述应克隆的[工作组](../resources/team.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="49c52-106">Describes which part of a [team](../resources/team.md) should be cloned.</span></span> 

## <a name="members"></a><span data-ttu-id="49c52-107">成员</span><span class="sxs-lookup"><span data-stu-id="49c52-107">Members</span></span>

| <span data-ttu-id="49c52-108">成员</span><span class="sxs-lookup"><span data-stu-id="49c52-108">Member</span></span> | <span data-ttu-id="49c52-109">值</span><span class="sxs-lookup"><span data-stu-id="49c52-109">Value</span></span>| <span data-ttu-id="49c52-110">说明</span><span class="sxs-lookup"><span data-stu-id="49c52-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="49c52-111">apps</span><span class="sxs-lookup"><span data-stu-id="49c52-111">apps</span></span>|<span data-ttu-id="49c52-112">1</span><span class="sxs-lookup"><span data-stu-id="49c52-112">1</span></span>|<span data-ttu-id="49c52-113">将复制已安装的应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="49c52-113">Copy the list of installed apps.</span></span>|
|<span data-ttu-id="49c52-114">选项卡</span><span class="sxs-lookup"><span data-stu-id="49c52-114">tabs</span></span>|<span data-ttu-id="49c52-115">2</span><span class="sxs-lookup"><span data-stu-id="49c52-115">2</span></span>|<span data-ttu-id="49c52-116">将复制通道中的选项卡。</span><span class="sxs-lookup"><span data-stu-id="49c52-116">copies the tabs within channels.</span></span>|
|<span data-ttu-id="49c52-117">settings</span><span class="sxs-lookup"><span data-stu-id="49c52-117">settings</span></span>|<span data-ttu-id="49c52-118">4</span><span class="sxs-lookup"><span data-stu-id="49c52-118">4</span></span>|<span data-ttu-id="49c52-119">将复制的团队，以及关键组设置中的所有设置。</span><span class="sxs-lookup"><span data-stu-id="49c52-119">Copies all settings within the team, along with key group settings.</span></span>|
|<span data-ttu-id="49c52-120">通道</span><span class="sxs-lookup"><span data-stu-id="49c52-120">channels</span></span>|<span data-ttu-id="49c52-121">8</span><span class="sxs-lookup"><span data-stu-id="49c52-121">8</span></span>|<span data-ttu-id="49c52-122">将复制的通道结构 （但不是在进入频道的消息）。</span><span class="sxs-lookup"><span data-stu-id="49c52-122">copies the channel structure (but not the messages in the channel).</span></span>|
|<span data-ttu-id="49c52-123">members</span><span class="sxs-lookup"><span data-stu-id="49c52-123">members</span></span>|<span data-ttu-id="49c52-124">16</span><span class="sxs-lookup"><span data-stu-id="49c52-124">16</span></span>|<span data-ttu-id="49c52-125">将复制的成员和所有者的团队。</span><span class="sxs-lookup"><span data-stu-id="49c52-125">copies the members and owners of the team.</span></span>|
