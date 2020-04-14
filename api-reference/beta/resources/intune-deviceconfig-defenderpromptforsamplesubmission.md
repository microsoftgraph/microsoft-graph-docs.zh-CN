---
title: defenderPromptForSampleSubmission 枚举类型
description: 提示用户提交示例的可能值。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6f346797813e2589bf35e9e9c45243192fe16ac8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43413109"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="14d0d-103">defenderPromptForSampleSubmission 枚举类型</span><span class="sxs-lookup"><span data-stu-id="14d0d-103">defenderPromptForSampleSubmission enum type</span></span>

<span data-ttu-id="14d0d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14d0d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14d0d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="14d0d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14d0d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="14d0d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14d0d-107">提示用户提交示例的可能值。</span><span class="sxs-lookup"><span data-stu-id="14d0d-107">Possible values for prompting user for samples submission.</span></span>

## <a name="members"></a><span data-ttu-id="14d0d-108">成员</span><span class="sxs-lookup"><span data-stu-id="14d0d-108">Members</span></span>
|<span data-ttu-id="14d0d-109">成员</span><span class="sxs-lookup"><span data-stu-id="14d0d-109">Member</span></span>|<span data-ttu-id="14d0d-110">值</span><span class="sxs-lookup"><span data-stu-id="14d0d-110">Value</span></span>|<span data-ttu-id="14d0d-111">说明</span><span class="sxs-lookup"><span data-stu-id="14d0d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14d0d-112">定制</span><span class="sxs-lookup"><span data-stu-id="14d0d-112">userDefined</span></span>|<span data-ttu-id="14d0d-113">0</span><span class="sxs-lookup"><span data-stu-id="14d0d-113">0</span></span>|<span data-ttu-id="14d0d-114">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="14d0d-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="14d0d-115">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="14d0d-115">alwaysPrompt</span></span>|<span data-ttu-id="14d0d-116">1</span><span class="sxs-lookup"><span data-stu-id="14d0d-116">1</span></span>|<span data-ttu-id="14d0d-117">始终提示。</span><span class="sxs-lookup"><span data-stu-id="14d0d-117">Always prompt.</span></span>|
|<span data-ttu-id="14d0d-118">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="14d0d-118">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="14d0d-119">双面</span><span class="sxs-lookup"><span data-stu-id="14d0d-119">2</span></span>|<span data-ttu-id="14d0d-120">发送个人数据前提示。</span><span class="sxs-lookup"><span data-stu-id="14d0d-120">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="14d0d-121">neverSendData</span><span class="sxs-lookup"><span data-stu-id="14d0d-121">neverSendData</span></span>|<span data-ttu-id="14d0d-122">第三章</span><span class="sxs-lookup"><span data-stu-id="14d0d-122">3</span></span>|<span data-ttu-id="14d0d-123">从不发送数据。</span><span class="sxs-lookup"><span data-stu-id="14d0d-123">Never send data.</span></span>|
|<span data-ttu-id="14d0d-124">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="14d0d-124">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="14d0d-125">4 </span><span class="sxs-lookup"><span data-stu-id="14d0d-125">4</span></span>|<span data-ttu-id="14d0d-126">在不提示的情况下发送所有数据。</span><span class="sxs-lookup"><span data-stu-id="14d0d-126">Send all data without prompting.</span></span>|



