---
title: subjectAlternativeNameType 枚举类型
description: "\"主题备用名称\" 选项。"
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ea055171fade56361562aeac065a67b23154e207
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792508"
---
# <a name="subjectalternativenametype-enum-type"></a><span data-ttu-id="de7a2-103">subjectAlternativeNameType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="de7a2-103">subjectAlternativeNameType enum type</span></span>

> <span data-ttu-id="de7a2-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="de7a2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de7a2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="de7a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de7a2-106">"主题备用名称" 选项。</span><span class="sxs-lookup"><span data-stu-id="de7a2-106">Subject Alternative Name Options.</span></span>

## <a name="members"></a><span data-ttu-id="de7a2-107">成员</span><span class="sxs-lookup"><span data-stu-id="de7a2-107">Members</span></span>
|<span data-ttu-id="de7a2-108">成员</span><span class="sxs-lookup"><span data-stu-id="de7a2-108">Member</span></span>|<span data-ttu-id="de7a2-109">值</span><span class="sxs-lookup"><span data-stu-id="de7a2-109">Value</span></span>|<span data-ttu-id="de7a2-110">说明</span><span class="sxs-lookup"><span data-stu-id="de7a2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de7a2-111">无</span><span class="sxs-lookup"><span data-stu-id="de7a2-111">none</span></span>|<span data-ttu-id="de7a2-112">0</span><span class="sxs-lookup"><span data-stu-id="de7a2-112">0</span></span>|<span data-ttu-id="de7a2-113">无使用者可选名称。</span><span class="sxs-lookup"><span data-stu-id="de7a2-113">No subject alternative name.</span></span>|
|<span data-ttu-id="de7a2-114">emailAddress</span><span class="sxs-lookup"><span data-stu-id="de7a2-114">emailAddress</span></span>|<span data-ttu-id="de7a2-115">1</span><span class="sxs-lookup"><span data-stu-id="de7a2-115">1</span></span>|<span data-ttu-id="de7a2-116">电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="de7a2-116">Email address.</span></span>|
|<span data-ttu-id="de7a2-117">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="de7a2-117">userPrincipalName</span></span>|<span data-ttu-id="de7a2-118">双面</span><span class="sxs-lookup"><span data-stu-id="de7a2-118">2</span></span>|<span data-ttu-id="de7a2-119">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="de7a2-119">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="de7a2-120">customAzureADAttribute</span><span class="sxs-lookup"><span data-stu-id="de7a2-120">customAzureADAttribute</span></span>|<span data-ttu-id="de7a2-121">4</span><span class="sxs-lookup"><span data-stu-id="de7a2-121">4</span></span>|<span data-ttu-id="de7a2-122">自定义 Azure AD 属性。</span><span class="sxs-lookup"><span data-stu-id="de7a2-122">Custom Azure AD Attribute.</span></span>|
|<span data-ttu-id="de7a2-123">domainNameService</span><span class="sxs-lookup"><span data-stu-id="de7a2-123">domainNameService</span></span>|<span data-ttu-id="de7a2-124">utf-8</span><span class="sxs-lookup"><span data-stu-id="de7a2-124">8</span></span>|<span data-ttu-id="de7a2-125">域名服务 (DNS)。</span><span class="sxs-lookup"><span data-stu-id="de7a2-125">Domain Name Service (DNS).</span></span>|





