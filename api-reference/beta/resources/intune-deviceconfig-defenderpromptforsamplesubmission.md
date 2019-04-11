---
title: defenderPromptForSampleSubmission 枚举类型
description: 提示用户提交示例的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c81fe62d7ed2696b233b8684c665f7cf8341fbcd
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778374"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="3f678-103">defenderPromptForSampleSubmission 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3f678-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="3f678-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3f678-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f678-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3f678-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f678-106">提示用户提交示例的可能值。</span><span class="sxs-lookup"><span data-stu-id="3f678-106">Possible values for prompting user for samples submission.</span></span>

## <a name="members"></a><span data-ttu-id="3f678-107">成员</span><span class="sxs-lookup"><span data-stu-id="3f678-107">Members</span></span>
|<span data-ttu-id="3f678-108">成员</span><span class="sxs-lookup"><span data-stu-id="3f678-108">Member</span></span>|<span data-ttu-id="3f678-109">值</span><span class="sxs-lookup"><span data-stu-id="3f678-109">Value</span></span>|<span data-ttu-id="3f678-110">说明</span><span class="sxs-lookup"><span data-stu-id="3f678-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f678-111">定制</span><span class="sxs-lookup"><span data-stu-id="3f678-111">userDefined</span></span>|<span data-ttu-id="3f678-112">0</span><span class="sxs-lookup"><span data-stu-id="3f678-112">0</span></span>|<span data-ttu-id="3f678-113">用户定义, 默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="3f678-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="3f678-114">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="3f678-114">alwaysPrompt</span></span>|<span data-ttu-id="3f678-115">1</span><span class="sxs-lookup"><span data-stu-id="3f678-115">1</span></span>|<span data-ttu-id="3f678-116">始终提示。</span><span class="sxs-lookup"><span data-stu-id="3f678-116">Always prompt.</span></span>|
|<span data-ttu-id="3f678-117">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="3f678-117">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="3f678-118">双面</span><span class="sxs-lookup"><span data-stu-id="3f678-118">2</span></span>|<span data-ttu-id="3f678-119">发送个人数据前提示。</span><span class="sxs-lookup"><span data-stu-id="3f678-119">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="3f678-120">neverSendData</span><span class="sxs-lookup"><span data-stu-id="3f678-120">neverSendData</span></span>|<span data-ttu-id="3f678-121">第三章</span><span class="sxs-lookup"><span data-stu-id="3f678-121">3</span></span>|<span data-ttu-id="3f678-122">从不发送数据。</span><span class="sxs-lookup"><span data-stu-id="3f678-122">Never send data.</span></span>|
|<span data-ttu-id="3f678-123">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="3f678-123">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="3f678-124">4</span><span class="sxs-lookup"><span data-stu-id="3f678-124">4</span></span>|<span data-ttu-id="3f678-125">在不提示的情况下发送所有数据。</span><span class="sxs-lookup"><span data-stu-id="3f678-125">Send all data without prompting.</span></span>|





