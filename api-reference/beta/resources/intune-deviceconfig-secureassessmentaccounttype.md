---
title: secureAssessmentAccountType 枚举类型
description: Windows10SecureAssessment ConfigurationAccount 允许的帐户类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: da9695d549b9abcdec4cb5fc4c32fd699fd1ddb4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49293855"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="7e45b-103">secureAssessmentAccountType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7e45b-103">secureAssessmentAccountType enum type</span></span>

<span data-ttu-id="7e45b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e45b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e45b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7e45b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e45b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7e45b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e45b-107">Windows10SecureAssessment ConfigurationAccount 允许的帐户类型。</span><span class="sxs-lookup"><span data-stu-id="7e45b-107">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>

## <a name="members"></a><span data-ttu-id="7e45b-108">成员</span><span class="sxs-lookup"><span data-stu-id="7e45b-108">Members</span></span>
|<span data-ttu-id="7e45b-109">成员</span><span class="sxs-lookup"><span data-stu-id="7e45b-109">Member</span></span>|<span data-ttu-id="7e45b-110">值</span><span class="sxs-lookup"><span data-stu-id="7e45b-110">Value</span></span>|<span data-ttu-id="7e45b-111">Description</span><span class="sxs-lookup"><span data-stu-id="7e45b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e45b-112">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="7e45b-112">azureADAccount</span></span>|<span data-ttu-id="7e45b-113">0</span><span class="sxs-lookup"><span data-stu-id="7e45b-113">0</span></span>|<span data-ttu-id="7e45b-114">指示 AzureAD\username@tenant.com 格式的 Azure AD 帐户。</span><span class="sxs-lookup"><span data-stu-id="7e45b-114">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="7e45b-115">domainAccount</span><span class="sxs-lookup"><span data-stu-id="7e45b-115">domainAccount</span></span>|<span data-ttu-id="7e45b-116">1</span><span class="sxs-lookup"><span data-stu-id="7e45b-116">1</span></span>|<span data-ttu-id="7e45b-117">指示域帐户的格式为 domain\user 或 user@domain.com。</span><span class="sxs-lookup"><span data-stu-id="7e45b-117">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="7e45b-118">localAccount</span><span class="sxs-lookup"><span data-stu-id="7e45b-118">localAccount</span></span>|<span data-ttu-id="7e45b-119">双面</span><span class="sxs-lookup"><span data-stu-id="7e45b-119">2</span></span>|<span data-ttu-id="7e45b-120">指示本地帐户的用户名格式。</span><span class="sxs-lookup"><span data-stu-id="7e45b-120">Indicates a local account in format of username.</span></span>|
|<span data-ttu-id="7e45b-121">localGuestAccount</span><span class="sxs-lookup"><span data-stu-id="7e45b-121">localGuestAccount</span></span>|<span data-ttu-id="7e45b-122">第三章</span><span class="sxs-lookup"><span data-stu-id="7e45b-122">3</span></span>|<span data-ttu-id="7e45b-123">以测试名称的格式指示本地来宾帐户。</span><span class="sxs-lookup"><span data-stu-id="7e45b-123">Indicates a local guest account in format of test name.</span></span>|




