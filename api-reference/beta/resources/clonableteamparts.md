---
title: clonableTeamParts 枚举类型
description: '介绍应克隆的团队部分。 '
localization_priority: Normal
doc_type: enumPageType
ms.prod: ''
author: nkramer
ms.openlocfilehash: e08beeb232e5c9b2c77200f75053e3a822945ca6
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810585"
---
# <a name="clonableteamparts-enum-type"></a><span data-ttu-id="73008-103">clonableTeamParts 枚举类型</span><span class="sxs-lookup"><span data-stu-id="73008-103">clonableTeamParts enum type</span></span>

<span data-ttu-id="73008-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73008-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73008-105">介绍应克隆的 [团队](../resources/team.md) 部分。</span><span class="sxs-lookup"><span data-stu-id="73008-105">Describes which part of a [team](../resources/team.md) should be cloned.</span></span>

## <a name="members"></a><span data-ttu-id="73008-106">成员</span><span class="sxs-lookup"><span data-stu-id="73008-106">Members</span></span>

| <span data-ttu-id="73008-107">成员</span><span class="sxs-lookup"><span data-stu-id="73008-107">Member</span></span> | <span data-ttu-id="73008-108">值</span><span class="sxs-lookup"><span data-stu-id="73008-108">Value</span></span>| <span data-ttu-id="73008-109">说明</span><span class="sxs-lookup"><span data-stu-id="73008-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="73008-110">apps</span><span class="sxs-lookup"><span data-stu-id="73008-110">apps</span></span>|<span data-ttu-id="73008-111">1</span><span class="sxs-lookup"><span data-stu-id="73008-111">1</span></span>|<span data-ttu-id="73008-112">复制已安装应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="73008-112">Copy the list of installed apps.</span></span>|
|<span data-ttu-id="73008-113">选项卡</span><span class="sxs-lookup"><span data-stu-id="73008-113">tabs</span></span>|<span data-ttu-id="73008-114">双面</span><span class="sxs-lookup"><span data-stu-id="73008-114">2</span></span>|<span data-ttu-id="73008-115">复制通道中的选项卡。</span><span class="sxs-lookup"><span data-stu-id="73008-115">copies the tabs within channels.</span></span>|
|<span data-ttu-id="73008-116">settings</span><span class="sxs-lookup"><span data-stu-id="73008-116">settings</span></span>|<span data-ttu-id="73008-117">4 </span><span class="sxs-lookup"><span data-stu-id="73008-117">4</span></span>|<span data-ttu-id="73008-118">复制团队中的所有设置以及关键组设置。</span><span class="sxs-lookup"><span data-stu-id="73008-118">Copies all settings within the team, along with key group settings.</span></span>|
|<span data-ttu-id="73008-119">channels</span><span class="sxs-lookup"><span data-stu-id="73008-119">channels</span></span>|<span data-ttu-id="73008-120">8 </span><span class="sxs-lookup"><span data-stu-id="73008-120">8</span></span>|<span data-ttu-id="73008-121">将通道结构 (，但不会复制频道) 中的邮件。</span><span class="sxs-lookup"><span data-stu-id="73008-121">copies the channel structure (but not the messages in the channel).</span></span>|
|<span data-ttu-id="73008-122">members</span><span class="sxs-lookup"><span data-stu-id="73008-122">members</span></span>|<span data-ttu-id="73008-123">16 </span><span class="sxs-lookup"><span data-stu-id="73008-123">16</span></span>|<span data-ttu-id="73008-124">复制团队的成员和所有者。</span><span class="sxs-lookup"><span data-stu-id="73008-124">copies the members and owners of the team.</span></span>|
