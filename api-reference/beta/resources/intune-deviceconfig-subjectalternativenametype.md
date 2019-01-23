---
title: subjectAlternativeNameType 枚举类型
description: 使用者替代名称选项。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 812aacf65bc73aade6eafc441fafda914ea6a3b5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423298"
---
# <a name="subjectalternativenametype-enum-type"></a><span data-ttu-id="82a31-103">subjectAlternativeNameType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="82a31-103">subjectAlternativeNameType enum type</span></span>

> <span data-ttu-id="82a31-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="82a31-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="82a31-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="82a31-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="82a31-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="82a31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82a31-107">使用者替代名称选项。</span><span class="sxs-lookup"><span data-stu-id="82a31-107">Subject Alternative Name Options.</span></span>

## <a name="members"></a><span data-ttu-id="82a31-108">成员</span><span class="sxs-lookup"><span data-stu-id="82a31-108">Members</span></span>
|<span data-ttu-id="82a31-109">成员</span><span class="sxs-lookup"><span data-stu-id="82a31-109">Member</span></span>|<span data-ttu-id="82a31-110">值</span><span class="sxs-lookup"><span data-stu-id="82a31-110">Value</span></span>|<span data-ttu-id="82a31-111">说明</span><span class="sxs-lookup"><span data-stu-id="82a31-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82a31-112">无</span><span class="sxs-lookup"><span data-stu-id="82a31-112">none</span></span>|<span data-ttu-id="82a31-113">0</span><span class="sxs-lookup"><span data-stu-id="82a31-113">0</span></span>|<span data-ttu-id="82a31-114">没有使用者替代名称。</span><span class="sxs-lookup"><span data-stu-id="82a31-114">No subject alternative name.</span></span>|
|<span data-ttu-id="82a31-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="82a31-115">emailAddress</span></span>|<span data-ttu-id="82a31-116">1</span><span class="sxs-lookup"><span data-stu-id="82a31-116">1</span></span>|<span data-ttu-id="82a31-117">电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="82a31-117">Email address.</span></span>|
|<span data-ttu-id="82a31-118">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="82a31-118">userPrincipalName</span></span>|<span data-ttu-id="82a31-119">2</span><span class="sxs-lookup"><span data-stu-id="82a31-119">2</span></span>|<span data-ttu-id="82a31-120">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="82a31-120">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="82a31-121">customAzureADAttribute</span><span class="sxs-lookup"><span data-stu-id="82a31-121">customAzureADAttribute</span></span>|<span data-ttu-id="82a31-122">4</span><span class="sxs-lookup"><span data-stu-id="82a31-122">4</span></span>|<span data-ttu-id="82a31-123">自定义的 Azure AD 属性。</span><span class="sxs-lookup"><span data-stu-id="82a31-123">Custom Azure AD Attribute.</span></span>|
|<span data-ttu-id="82a31-124">domainNameService</span><span class="sxs-lookup"><span data-stu-id="82a31-124">domainNameService</span></span>|<span data-ttu-id="82a31-125">8</span><span class="sxs-lookup"><span data-stu-id="82a31-125">8</span></span>|<span data-ttu-id="82a31-126">域名服务 (DNS)。</span><span class="sxs-lookup"><span data-stu-id="82a31-126">Domain Name Service (DNS).</span></span>|




