---
title: subjectAlternativeNameType 枚举类型
description: 使用者替代名称选项。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 47ee2bc7e8a6c53d48f0b167983f85e0a18f4f4e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984204"
---
# <a name="subjectalternativenametype-enum-type"></a><span data-ttu-id="eaee0-103">subjectAlternativeNameType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="eaee0-103">subjectAlternativeNameType enum type</span></span>

> <span data-ttu-id="eaee0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="eaee0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eaee0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="eaee0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eaee0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="eaee0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eaee0-107">使用者替代名称选项。</span><span class="sxs-lookup"><span data-stu-id="eaee0-107">Subject Alternative Name Options.</span></span>
## <a name="members"></a><span data-ttu-id="eaee0-108">成员</span><span class="sxs-lookup"><span data-stu-id="eaee0-108">Members</span></span>
|<span data-ttu-id="eaee0-109">成员</span><span class="sxs-lookup"><span data-stu-id="eaee0-109">Member</span></span>|<span data-ttu-id="eaee0-110">值</span><span class="sxs-lookup"><span data-stu-id="eaee0-110">Value</span></span>|<span data-ttu-id="eaee0-111">说明</span><span class="sxs-lookup"><span data-stu-id="eaee0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaee0-112">无</span><span class="sxs-lookup"><span data-stu-id="eaee0-112">none</span></span>|<span data-ttu-id="eaee0-113">0</span><span class="sxs-lookup"><span data-stu-id="eaee0-113">0</span></span>|<span data-ttu-id="eaee0-114">没有使用者替代名称。</span><span class="sxs-lookup"><span data-stu-id="eaee0-114">No subject alternative name.</span></span>|
|<span data-ttu-id="eaee0-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="eaee0-115">emailAddress</span></span>|<span data-ttu-id="eaee0-116">1</span><span class="sxs-lookup"><span data-stu-id="eaee0-116">1</span></span>|<span data-ttu-id="eaee0-117">电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="eaee0-117">Email address.</span></span>|
|<span data-ttu-id="eaee0-118">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="eaee0-118">userPrincipalName</span></span>|<span data-ttu-id="eaee0-119">2</span><span class="sxs-lookup"><span data-stu-id="eaee0-119">2</span></span>|<span data-ttu-id="eaee0-120">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="eaee0-120">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="eaee0-121">customAzureADAttribute</span><span class="sxs-lookup"><span data-stu-id="eaee0-121">customAzureADAttribute</span></span>|<span data-ttu-id="eaee0-122">4</span><span class="sxs-lookup"><span data-stu-id="eaee0-122">4</span></span>|<span data-ttu-id="eaee0-123">自定义的 Azure AD 属性。</span><span class="sxs-lookup"><span data-stu-id="eaee0-123">Custom Azure AD Attribute.</span></span>|
|<span data-ttu-id="eaee0-124">domainNameService</span><span class="sxs-lookup"><span data-stu-id="eaee0-124">domainNameService</span></span>|<span data-ttu-id="eaee0-125">8</span><span class="sxs-lookup"><span data-stu-id="eaee0-125">8</span></span>|<span data-ttu-id="eaee0-126">域名服务 (DNS)。</span><span class="sxs-lookup"><span data-stu-id="eaee0-126">Domain Name Service (DNS).</span></span>|





