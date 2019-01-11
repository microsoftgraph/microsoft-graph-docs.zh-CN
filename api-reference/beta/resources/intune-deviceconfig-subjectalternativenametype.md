---
title: subjectAlternativeNameType 枚举类型
description: 使用者替代名称选项。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 914c4d577cc478e42e7982b9480bc8e43b8d88de
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869543"
---
# <a name="subjectalternativenametype-enum-type"></a><span data-ttu-id="8c3e9-103">subjectAlternativeNameType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8c3e9-103">subjectAlternativeNameType enum type</span></span>

> <span data-ttu-id="8c3e9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8c3e9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c3e9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8c3e9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c3e9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8c3e9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c3e9-107">使用者替代名称选项。</span><span class="sxs-lookup"><span data-stu-id="8c3e9-107">Subject Alternative Name Options.</span></span>
## <a name="members"></a><span data-ttu-id="8c3e9-108">成员</span><span class="sxs-lookup"><span data-stu-id="8c3e9-108">Members</span></span>
|<span data-ttu-id="8c3e9-109">成员</span><span class="sxs-lookup"><span data-stu-id="8c3e9-109">Member</span></span>|<span data-ttu-id="8c3e9-110">值</span><span class="sxs-lookup"><span data-stu-id="8c3e9-110">Value</span></span>|<span data-ttu-id="8c3e9-111">Description</span><span class="sxs-lookup"><span data-stu-id="8c3e9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c3e9-112">无</span><span class="sxs-lookup"><span data-stu-id="8c3e9-112">none</span></span>|<span data-ttu-id="8c3e9-113">0</span><span class="sxs-lookup"><span data-stu-id="8c3e9-113">0</span></span>|<span data-ttu-id="8c3e9-114">没有使用者替代名称。</span><span class="sxs-lookup"><span data-stu-id="8c3e9-114">No subject alternative name.</span></span>|
|<span data-ttu-id="8c3e9-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8c3e9-115">emailAddress</span></span>|<span data-ttu-id="8c3e9-116">1</span><span class="sxs-lookup"><span data-stu-id="8c3e9-116">1</span></span>|<span data-ttu-id="8c3e9-117">电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="8c3e9-117">Email address.</span></span>|
|<span data-ttu-id="8c3e9-118">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8c3e9-118">userPrincipalName</span></span>|<span data-ttu-id="8c3e9-119">2</span><span class="sxs-lookup"><span data-stu-id="8c3e9-119">2</span></span>|<span data-ttu-id="8c3e9-120">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="8c3e9-120">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="8c3e9-121">customAzureADAttribute</span><span class="sxs-lookup"><span data-stu-id="8c3e9-121">customAzureADAttribute</span></span>|<span data-ttu-id="8c3e9-122">4</span><span class="sxs-lookup"><span data-stu-id="8c3e9-122">4</span></span>|<span data-ttu-id="8c3e9-123">自定义的 Azure AD 属性。</span><span class="sxs-lookup"><span data-stu-id="8c3e9-123">Custom Azure AD Attribute.</span></span>|
|<span data-ttu-id="8c3e9-124">domainNameService</span><span class="sxs-lookup"><span data-stu-id="8c3e9-124">domainNameService</span></span>|<span data-ttu-id="8c3e9-125">8</span><span class="sxs-lookup"><span data-stu-id="8c3e9-125">8</span></span>|<span data-ttu-id="8c3e9-126">域名服务 (DNS)。</span><span class="sxs-lookup"><span data-stu-id="8c3e9-126">Domain Name Service (DNS).</span></span>|





