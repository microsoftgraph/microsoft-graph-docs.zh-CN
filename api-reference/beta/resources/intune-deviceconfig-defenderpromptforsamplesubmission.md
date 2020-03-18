---
title: defenderPromptForSampleSubmission 枚举类型
description: 提示用户提交示例的可能值。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7787dc018862a5311f37866957c6df4d968f910a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42794457"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="e9408-103">defenderPromptForSampleSubmission 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e9408-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="e9408-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e9408-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9408-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e9408-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9408-106">提示用户提交示例的可能值。</span><span class="sxs-lookup"><span data-stu-id="e9408-106">Possible values for prompting user for samples submission.</span></span>

## <a name="members"></a><span data-ttu-id="e9408-107">成员</span><span class="sxs-lookup"><span data-stu-id="e9408-107">Members</span></span>
|<span data-ttu-id="e9408-108">成员</span><span class="sxs-lookup"><span data-stu-id="e9408-108">Member</span></span>|<span data-ttu-id="e9408-109">值</span><span class="sxs-lookup"><span data-stu-id="e9408-109">Value</span></span>|<span data-ttu-id="e9408-110">说明</span><span class="sxs-lookup"><span data-stu-id="e9408-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9408-111">定制</span><span class="sxs-lookup"><span data-stu-id="e9408-111">userDefined</span></span>|<span data-ttu-id="e9408-112">0</span><span class="sxs-lookup"><span data-stu-id="e9408-112">0</span></span>|<span data-ttu-id="e9408-113">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="e9408-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="e9408-114">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="e9408-114">alwaysPrompt</span></span>|<span data-ttu-id="e9408-115">1</span><span class="sxs-lookup"><span data-stu-id="e9408-115">1</span></span>|<span data-ttu-id="e9408-116">始终提示。</span><span class="sxs-lookup"><span data-stu-id="e9408-116">Always prompt.</span></span>|
|<span data-ttu-id="e9408-117">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="e9408-117">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="e9408-118">双面</span><span class="sxs-lookup"><span data-stu-id="e9408-118">2</span></span>|<span data-ttu-id="e9408-119">发送个人数据前提示。</span><span class="sxs-lookup"><span data-stu-id="e9408-119">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="e9408-120">neverSendData</span><span class="sxs-lookup"><span data-stu-id="e9408-120">neverSendData</span></span>|<span data-ttu-id="e9408-121">第三章</span><span class="sxs-lookup"><span data-stu-id="e9408-121">3</span></span>|<span data-ttu-id="e9408-122">从不发送数据。</span><span class="sxs-lookup"><span data-stu-id="e9408-122">Never send data.</span></span>|
|<span data-ttu-id="e9408-123">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="e9408-123">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="e9408-124">4 </span><span class="sxs-lookup"><span data-stu-id="e9408-124">4</span></span>|<span data-ttu-id="e9408-125">在不提示的情况下发送所有数据。</span><span class="sxs-lookup"><span data-stu-id="e9408-125">Send all data without prompting.</span></span>|



