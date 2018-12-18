---
title: defenderPromptForSampleSubmission 枚举类型
description: 提示用户输入示例提交的可能值。
author: tfitzmac
ms.openlocfilehash: 19498f587759df56ae671b119b59abe7e7acd62c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314929"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="06c68-103">defenderPromptForSampleSubmission 枚举类型</span><span class="sxs-lookup"><span data-stu-id="06c68-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="06c68-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="06c68-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06c68-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="06c68-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06c68-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="06c68-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06c68-107">提示用户输入示例提交的可能值。</span><span class="sxs-lookup"><span data-stu-id="06c68-107">Possible values for prompting user for samples submission.</span></span>
## <a name="members"></a><span data-ttu-id="06c68-108">成员</span><span class="sxs-lookup"><span data-stu-id="06c68-108">Members</span></span>
|<span data-ttu-id="06c68-109">成员</span><span class="sxs-lookup"><span data-stu-id="06c68-109">Member</span></span>|<span data-ttu-id="06c68-110">值</span><span class="sxs-lookup"><span data-stu-id="06c68-110">Value</span></span>|<span data-ttu-id="06c68-111">说明</span><span class="sxs-lookup"><span data-stu-id="06c68-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06c68-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="06c68-112">userDefined</span></span>|<span data-ttu-id="06c68-113">0</span><span class="sxs-lookup"><span data-stu-id="06c68-113">0</span></span>|<span data-ttu-id="06c68-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="06c68-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="06c68-115">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="06c68-115">alwaysPrompt</span></span>|<span data-ttu-id="06c68-116">1</span><span class="sxs-lookup"><span data-stu-id="06c68-116">1</span></span>|<span data-ttu-id="06c68-117">始终提示。</span><span class="sxs-lookup"><span data-stu-id="06c68-117">Always prompt.</span></span>|
|<span data-ttu-id="06c68-118">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="06c68-118">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="06c68-119">2</span><span class="sxs-lookup"><span data-stu-id="06c68-119">2</span></span>|<span data-ttu-id="06c68-120">将个人数据发送前提示。</span><span class="sxs-lookup"><span data-stu-id="06c68-120">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="06c68-121">neverSendData</span><span class="sxs-lookup"><span data-stu-id="06c68-121">neverSendData</span></span>|<span data-ttu-id="06c68-122">3</span><span class="sxs-lookup"><span data-stu-id="06c68-122">3</span></span>|<span data-ttu-id="06c68-123">从不发送数据。</span><span class="sxs-lookup"><span data-stu-id="06c68-123">Never send data.</span></span>|
|<span data-ttu-id="06c68-124">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="06c68-124">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="06c68-125">4</span><span class="sxs-lookup"><span data-stu-id="06c68-125">4</span></span>|<span data-ttu-id="06c68-126">发送所有数据，而不提示。</span><span class="sxs-lookup"><span data-stu-id="06c68-126">Send all data without prompting.</span></span>|





