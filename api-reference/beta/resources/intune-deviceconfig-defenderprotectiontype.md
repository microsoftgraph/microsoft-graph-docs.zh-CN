---
title: defenderProtectionType 枚举类型
description: Defender PUA Protection 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1e64852c08da6853e091beef214e1fd427ecceba
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256373"
---
# <a name="defenderprotectiontype-enum-type"></a><span data-ttu-id="06a5a-103">defenderProtectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="06a5a-103">defenderProtectionType enum type</span></span>

<span data-ttu-id="06a5a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06a5a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06a5a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="06a5a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06a5a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06a5a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06a5a-107">Defender PUA Protection 的可能值</span><span class="sxs-lookup"><span data-stu-id="06a5a-107">Possible values of Defender PUA Protection</span></span>

## <a name="members"></a><span data-ttu-id="06a5a-108">成员</span><span class="sxs-lookup"><span data-stu-id="06a5a-108">Members</span></span>
|<span data-ttu-id="06a5a-109">成员</span><span class="sxs-lookup"><span data-stu-id="06a5a-109">Member</span></span>|<span data-ttu-id="06a5a-110">值</span><span class="sxs-lookup"><span data-stu-id="06a5a-110">Value</span></span>|<span data-ttu-id="06a5a-111">说明</span><span class="sxs-lookup"><span data-stu-id="06a5a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06a5a-112">定制</span><span class="sxs-lookup"><span data-stu-id="06a5a-112">userDefined</span></span>|<span data-ttu-id="06a5a-113">0</span><span class="sxs-lookup"><span data-stu-id="06a5a-113">0</span></span>|<span data-ttu-id="06a5a-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="06a5a-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="06a5a-115">启用</span><span class="sxs-lookup"><span data-stu-id="06a5a-115">enable</span></span>|<span data-ttu-id="06a5a-116">1</span><span class="sxs-lookup"><span data-stu-id="06a5a-116">1</span></span>|<span data-ttu-id="06a5a-117">阻止功能。</span><span class="sxs-lookup"><span data-stu-id="06a5a-117">Block functionality.</span></span>|
|<span data-ttu-id="06a5a-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="06a5a-118">auditMode</span></span>|<span data-ttu-id="06a5a-119">双面</span><span class="sxs-lookup"><span data-stu-id="06a5a-119">2</span></span>|<span data-ttu-id="06a5a-120">允许功能，但生成日志。</span><span class="sxs-lookup"><span data-stu-id="06a5a-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="06a5a-121">警告</span><span class="sxs-lookup"><span data-stu-id="06a5a-121">warn</span></span>|<span data-ttu-id="06a5a-122">6 </span><span class="sxs-lookup"><span data-stu-id="06a5a-122">6</span></span>|<span data-ttu-id="06a5a-123">向最终用户发出的警告消息，能够绕过受攻击面降低规则阻止的阻止。</span><span class="sxs-lookup"><span data-stu-id="06a5a-123">Warning message to end user with ability to bypass block from attack surface reduction rule.</span></span>|
|<span data-ttu-id="06a5a-124">notConfigured</span><span class="sxs-lookup"><span data-stu-id="06a5a-124">notConfigured</span></span>|<span data-ttu-id="06a5a-125">99</span><span class="sxs-lookup"><span data-stu-id="06a5a-125">99</span></span>|<span data-ttu-id="06a5a-126">未配置。</span><span class="sxs-lookup"><span data-stu-id="06a5a-126">Not configured.</span></span>|




