---
title: subjectAlternativeNameType 枚举类型
description: "\"主题备用名称\" 选项。"
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7837c1027a6711a0614c0329c46c5a9e41b9f265
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787472"
---
# <a name="subjectalternativenametype-enum-type"></a><span data-ttu-id="d00a3-103">subjectAlternativeNameType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d00a3-103">subjectAlternativeNameType enum type</span></span>

> <span data-ttu-id="d00a3-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d00a3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d00a3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d00a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d00a3-106">"主题备用名称" 选项。</span><span class="sxs-lookup"><span data-stu-id="d00a3-106">Subject Alternative Name Options.</span></span>

## <a name="members"></a><span data-ttu-id="d00a3-107">成员</span><span class="sxs-lookup"><span data-stu-id="d00a3-107">Members</span></span>
|<span data-ttu-id="d00a3-108">成员</span><span class="sxs-lookup"><span data-stu-id="d00a3-108">Member</span></span>|<span data-ttu-id="d00a3-109">值</span><span class="sxs-lookup"><span data-stu-id="d00a3-109">Value</span></span>|<span data-ttu-id="d00a3-110">说明</span><span class="sxs-lookup"><span data-stu-id="d00a3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d00a3-111">无</span><span class="sxs-lookup"><span data-stu-id="d00a3-111">none</span></span>|<span data-ttu-id="d00a3-112">0</span><span class="sxs-lookup"><span data-stu-id="d00a3-112">0</span></span>|<span data-ttu-id="d00a3-113">无使用者可选名称。</span><span class="sxs-lookup"><span data-stu-id="d00a3-113">No subject alternative name.</span></span>|
|<span data-ttu-id="d00a3-114">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d00a3-114">emailAddress</span></span>|<span data-ttu-id="d00a3-115">1</span><span class="sxs-lookup"><span data-stu-id="d00a3-115">1</span></span>|<span data-ttu-id="d00a3-116">电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="d00a3-116">Email address.</span></span>|
|<span data-ttu-id="d00a3-117">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d00a3-117">userPrincipalName</span></span>|<span data-ttu-id="d00a3-118">双面</span><span class="sxs-lookup"><span data-stu-id="d00a3-118">2</span></span>|<span data-ttu-id="d00a3-119">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="d00a3-119">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="d00a3-120">customAzureADAttribute</span><span class="sxs-lookup"><span data-stu-id="d00a3-120">customAzureADAttribute</span></span>|<span data-ttu-id="d00a3-121">4 </span><span class="sxs-lookup"><span data-stu-id="d00a3-121">4</span></span>|<span data-ttu-id="d00a3-122">自定义 Azure AD 属性。</span><span class="sxs-lookup"><span data-stu-id="d00a3-122">Custom Azure AD Attribute.</span></span>|
|<span data-ttu-id="d00a3-123">domainNameService</span><span class="sxs-lookup"><span data-stu-id="d00a3-123">domainNameService</span></span>|<span data-ttu-id="d00a3-124">8 </span><span class="sxs-lookup"><span data-stu-id="d00a3-124">8</span></span>|<span data-ttu-id="d00a3-125">域名服务（DNS）。</span><span class="sxs-lookup"><span data-stu-id="d00a3-125">Domain Name Service (DNS).</span></span>|



