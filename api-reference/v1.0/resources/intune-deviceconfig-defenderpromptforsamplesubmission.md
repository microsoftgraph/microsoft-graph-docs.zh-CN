---
title: defenderPromptForSampleSubmission 枚举类型
description: 提示用户提交示例的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c2e038ab28632c790e5ffaa4f6e1ccb3b4415a5f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752369"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="627a1-103">defenderPromptForSampleSubmission 枚举类型</span><span class="sxs-lookup"><span data-stu-id="627a1-103">defenderPromptForSampleSubmission enum type</span></span>

<span data-ttu-id="627a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="627a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="627a1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="627a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="627a1-106">提示用户提交示例的可能值。</span><span class="sxs-lookup"><span data-stu-id="627a1-106">Possible values for prompting user for samples submission.</span></span>

## <a name="members"></a><span data-ttu-id="627a1-107">成员</span><span class="sxs-lookup"><span data-stu-id="627a1-107">Members</span></span>
|<span data-ttu-id="627a1-108">成员</span><span class="sxs-lookup"><span data-stu-id="627a1-108">Member</span></span>|<span data-ttu-id="627a1-109">值</span><span class="sxs-lookup"><span data-stu-id="627a1-109">Value</span></span>|<span data-ttu-id="627a1-110">Description</span><span class="sxs-lookup"><span data-stu-id="627a1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="627a1-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="627a1-111">userDefined</span></span>|<span data-ttu-id="627a1-112">0</span><span class="sxs-lookup"><span data-stu-id="627a1-112">0</span></span>|<span data-ttu-id="627a1-113">用户定义，默认值，无意图。</span><span class="sxs-lookup"><span data-stu-id="627a1-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="627a1-114">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="627a1-114">alwaysPrompt</span></span>|<span data-ttu-id="627a1-115">1</span><span class="sxs-lookup"><span data-stu-id="627a1-115">1</span></span>|<span data-ttu-id="627a1-116">始终提示。</span><span class="sxs-lookup"><span data-stu-id="627a1-116">Always prompt.</span></span>|
|<span data-ttu-id="627a1-117">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="627a1-117">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="627a1-118">2</span><span class="sxs-lookup"><span data-stu-id="627a1-118">2</span></span>|<span data-ttu-id="627a1-119">自动发送安全示例。</span><span class="sxs-lookup"><span data-stu-id="627a1-119">Send safe samples automatically.</span></span>|
|<span data-ttu-id="627a1-120">neverSendData</span><span class="sxs-lookup"><span data-stu-id="627a1-120">neverSendData</span></span>|<span data-ttu-id="627a1-121">3</span><span class="sxs-lookup"><span data-stu-id="627a1-121">3</span></span>|<span data-ttu-id="627a1-122">从不发送数据。</span><span class="sxs-lookup"><span data-stu-id="627a1-122">Never send data.</span></span>|
|<span data-ttu-id="627a1-123">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="627a1-123">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="627a1-124">4 </span><span class="sxs-lookup"><span data-stu-id="627a1-124">4</span></span>|<span data-ttu-id="627a1-125">在不提示的情况下发送所有数据。</span><span class="sxs-lookup"><span data-stu-id="627a1-125">Send all data without prompting.</span></span>|




