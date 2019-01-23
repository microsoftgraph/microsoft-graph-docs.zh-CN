---
title: defenderPromptForSampleSubmission 枚举类型
description: 提示用户输入示例提交的可能值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b706c0086791543a5cbb13d26ae1d86a2e3b1760
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403313"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="3cfab-103">defenderPromptForSampleSubmission 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3cfab-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="3cfab-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="3cfab-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3cfab-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3cfab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3cfab-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3cfab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cfab-107">提示用户输入示例提交的可能值。</span><span class="sxs-lookup"><span data-stu-id="3cfab-107">Possible values for prompting user for samples submission.</span></span>

## <a name="members"></a><span data-ttu-id="3cfab-108">成员</span><span class="sxs-lookup"><span data-stu-id="3cfab-108">Members</span></span>
|<span data-ttu-id="3cfab-109">成员</span><span class="sxs-lookup"><span data-stu-id="3cfab-109">Member</span></span>|<span data-ttu-id="3cfab-110">值</span><span class="sxs-lookup"><span data-stu-id="3cfab-110">Value</span></span>|<span data-ttu-id="3cfab-111">说明</span><span class="sxs-lookup"><span data-stu-id="3cfab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cfab-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="3cfab-112">userDefined</span></span>|<span data-ttu-id="3cfab-113">0</span><span class="sxs-lookup"><span data-stu-id="3cfab-113">0</span></span>|<span data-ttu-id="3cfab-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="3cfab-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="3cfab-115">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="3cfab-115">alwaysPrompt</span></span>|<span data-ttu-id="3cfab-116">1</span><span class="sxs-lookup"><span data-stu-id="3cfab-116">1</span></span>|<span data-ttu-id="3cfab-117">始终提示。</span><span class="sxs-lookup"><span data-stu-id="3cfab-117">Always prompt.</span></span>|
|<span data-ttu-id="3cfab-118">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="3cfab-118">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="3cfab-119">2</span><span class="sxs-lookup"><span data-stu-id="3cfab-119">2</span></span>|<span data-ttu-id="3cfab-120">将个人数据发送前提示。</span><span class="sxs-lookup"><span data-stu-id="3cfab-120">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="3cfab-121">neverSendData</span><span class="sxs-lookup"><span data-stu-id="3cfab-121">neverSendData</span></span>|<span data-ttu-id="3cfab-122">3</span><span class="sxs-lookup"><span data-stu-id="3cfab-122">3</span></span>|<span data-ttu-id="3cfab-123">从不发送数据。</span><span class="sxs-lookup"><span data-stu-id="3cfab-123">Never send data.</span></span>|
|<span data-ttu-id="3cfab-124">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="3cfab-124">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="3cfab-125">4</span><span class="sxs-lookup"><span data-stu-id="3cfab-125">4</span></span>|<span data-ttu-id="3cfab-126">发送所有数据，而不提示。</span><span class="sxs-lookup"><span data-stu-id="3cfab-126">Send all data without prompting.</span></span>|




