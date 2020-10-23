---
title: subjectAlternativeNameType 枚举类型
description: "\"主题备用名称\" 选项。"
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 435c65ed27245aa1f899a129a13a443c6a69396c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693792"
---
# <a name="subjectalternativenametype-enum-type"></a><span data-ttu-id="14551-103">subjectAlternativeNameType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="14551-103">subjectAlternativeNameType enum type</span></span>

<span data-ttu-id="14551-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14551-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14551-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="14551-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14551-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="14551-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14551-107">"主题备用名称" 选项。</span><span class="sxs-lookup"><span data-stu-id="14551-107">Subject Alternative Name Options.</span></span>

## <a name="members"></a><span data-ttu-id="14551-108">成员</span><span class="sxs-lookup"><span data-stu-id="14551-108">Members</span></span>
|<span data-ttu-id="14551-109">成员</span><span class="sxs-lookup"><span data-stu-id="14551-109">Member</span></span>|<span data-ttu-id="14551-110">值</span><span class="sxs-lookup"><span data-stu-id="14551-110">Value</span></span>|<span data-ttu-id="14551-111">说明</span><span class="sxs-lookup"><span data-stu-id="14551-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14551-112">无</span><span class="sxs-lookup"><span data-stu-id="14551-112">none</span></span>|<span data-ttu-id="14551-113">0</span><span class="sxs-lookup"><span data-stu-id="14551-113">0</span></span>|<span data-ttu-id="14551-114">无使用者可选名称。</span><span class="sxs-lookup"><span data-stu-id="14551-114">No subject alternative name.</span></span>|
|<span data-ttu-id="14551-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="14551-115">emailAddress</span></span>|<span data-ttu-id="14551-116">1</span><span class="sxs-lookup"><span data-stu-id="14551-116">1</span></span>|<span data-ttu-id="14551-117">电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="14551-117">Email address.</span></span>|
|<span data-ttu-id="14551-118">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="14551-118">userPrincipalName</span></span>|<span data-ttu-id="14551-119">双面</span><span class="sxs-lookup"><span data-stu-id="14551-119">2</span></span>|<span data-ttu-id="14551-120">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="14551-120">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="14551-121">customAzureADAttribute</span><span class="sxs-lookup"><span data-stu-id="14551-121">customAzureADAttribute</span></span>|<span data-ttu-id="14551-122">4 </span><span class="sxs-lookup"><span data-stu-id="14551-122">4</span></span>|<span data-ttu-id="14551-123">自定义 Azure AD 属性。</span><span class="sxs-lookup"><span data-stu-id="14551-123">Custom Azure AD Attribute.</span></span>|
|<span data-ttu-id="14551-124">domainNameService</span><span class="sxs-lookup"><span data-stu-id="14551-124">domainNameService</span></span>|<span data-ttu-id="14551-125">8 </span><span class="sxs-lookup"><span data-stu-id="14551-125">8</span></span>|<span data-ttu-id="14551-126">域名服务 (DNS) 。</span><span class="sxs-lookup"><span data-stu-id="14551-126">Domain Name Service (DNS).</span></span>|
|<span data-ttu-id="14551-127">universalResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="14551-127">universalResourceIdentifier</span></span>|<span data-ttu-id="14551-128">16 </span><span class="sxs-lookup"><span data-stu-id="14551-128">16</span></span>|<span data-ttu-id="14551-129"> (URI) 的通用资源标识符。</span><span class="sxs-lookup"><span data-stu-id="14551-129">Universal Resource Identifier (URI).</span></span>|





