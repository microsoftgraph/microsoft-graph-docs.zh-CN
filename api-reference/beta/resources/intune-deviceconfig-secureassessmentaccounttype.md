---
title: secureAssessmentAccountType 枚举类型
description: Windows10SecureAssessment ConfigurationAccount 允许的帐户类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4fa14d90465ed9278fd20362800d5d111de62950
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31795007"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="1276a-103">secureAssessmentAccountType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1276a-103">secureAssessmentAccountType enum type</span></span>

> <span data-ttu-id="1276a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1276a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1276a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1276a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1276a-106">Windows10SecureAssessment ConfigurationAccount 允许的帐户类型。</span><span class="sxs-lookup"><span data-stu-id="1276a-106">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>

## <a name="members"></a><span data-ttu-id="1276a-107">成员</span><span class="sxs-lookup"><span data-stu-id="1276a-107">Members</span></span>
|<span data-ttu-id="1276a-108">成员</span><span class="sxs-lookup"><span data-stu-id="1276a-108">Member</span></span>|<span data-ttu-id="1276a-109">值</span><span class="sxs-lookup"><span data-stu-id="1276a-109">Value</span></span>|<span data-ttu-id="1276a-110">说明</span><span class="sxs-lookup"><span data-stu-id="1276a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1276a-111">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="1276a-111">azureADAccount</span></span>|<span data-ttu-id="1276a-112">0</span><span class="sxs-lookup"><span data-stu-id="1276a-112">0</span></span>|<span data-ttu-id="1276a-113">指示的 Azure AD 帐户的格式为AzureAD\username@tenant.com。</span><span class="sxs-lookup"><span data-stu-id="1276a-113">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="1276a-114">domainAccount</span><span class="sxs-lookup"><span data-stu-id="1276a-114">domainAccount</span></span>|<span data-ttu-id="1276a-115">1</span><span class="sxs-lookup"><span data-stu-id="1276a-115">1</span></span>|<span data-ttu-id="1276a-116">指示域帐户的格式为 domain\user 或user@domain.com。</span><span class="sxs-lookup"><span data-stu-id="1276a-116">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="1276a-117">localAccount</span><span class="sxs-lookup"><span data-stu-id="1276a-117">localAccount</span></span>|<span data-ttu-id="1276a-118">双面</span><span class="sxs-lookup"><span data-stu-id="1276a-118">2</span></span>|<span data-ttu-id="1276a-119">指示本地帐户的用户名格式。</span><span class="sxs-lookup"><span data-stu-id="1276a-119">Indicates a local account in format of username.</span></span>|





