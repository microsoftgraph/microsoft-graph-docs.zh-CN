---
title: subjectAlternativeNameType 枚举类型
description: 使用者替代名称选项。
ms.openlocfilehash: 385ee36111907dd2e48bc18a2efda9552eb61924
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042951"
---
# <a name="subjectalternativenametype-enum-type"></a><span data-ttu-id="c41ba-103">subjectAlternativeNameType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c41ba-103">subjectAlternativeNameType enum type</span></span>

> <span data-ttu-id="c41ba-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c41ba-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c41ba-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c41ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c41ba-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c41ba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c41ba-107">使用者替代名称选项。</span><span class="sxs-lookup"><span data-stu-id="c41ba-107">Subject Alternative Name Options.</span></span>
## <a name="members"></a><span data-ttu-id="c41ba-108">成员</span><span class="sxs-lookup"><span data-stu-id="c41ba-108">Members</span></span>
|<span data-ttu-id="c41ba-109">成员</span><span class="sxs-lookup"><span data-stu-id="c41ba-109">Member</span></span>|<span data-ttu-id="c41ba-110">值</span><span class="sxs-lookup"><span data-stu-id="c41ba-110">Value</span></span>|<span data-ttu-id="c41ba-111">说明</span><span class="sxs-lookup"><span data-stu-id="c41ba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c41ba-112">无</span><span class="sxs-lookup"><span data-stu-id="c41ba-112">none</span></span>|<span data-ttu-id="c41ba-113">0</span><span class="sxs-lookup"><span data-stu-id="c41ba-113">0</span></span>|<span data-ttu-id="c41ba-114">没有使用者替代名称。</span><span class="sxs-lookup"><span data-stu-id="c41ba-114">No subject alternative name.</span></span>|
|<span data-ttu-id="c41ba-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c41ba-115">emailAddress</span></span>|<span data-ttu-id="c41ba-116">1</span><span class="sxs-lookup"><span data-stu-id="c41ba-116">1</span></span>|<span data-ttu-id="c41ba-117">电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="c41ba-117">Email address.</span></span>|
|<span data-ttu-id="c41ba-118">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c41ba-118">userPrincipalName</span></span>|<span data-ttu-id="c41ba-119">2</span><span class="sxs-lookup"><span data-stu-id="c41ba-119">2</span></span>|<span data-ttu-id="c41ba-120">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="c41ba-120">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="c41ba-121">customAzureADAttribute</span><span class="sxs-lookup"><span data-stu-id="c41ba-121">customAzureADAttribute</span></span>|<span data-ttu-id="c41ba-122">4</span><span class="sxs-lookup"><span data-stu-id="c41ba-122">4</span></span>|<span data-ttu-id="c41ba-123">自定义的 Azure AD 属性。</span><span class="sxs-lookup"><span data-stu-id="c41ba-123">Custom Azure AD Attribute.</span></span>|
|<span data-ttu-id="c41ba-124">domainNameService</span><span class="sxs-lookup"><span data-stu-id="c41ba-124">domainNameService</span></span>|<span data-ttu-id="c41ba-125">8</span><span class="sxs-lookup"><span data-stu-id="c41ba-125">8</span></span>|<span data-ttu-id="c41ba-126">域名服务 (DNS)。</span><span class="sxs-lookup"><span data-stu-id="c41ba-126">Domain Name Service (DNS).</span></span>|





