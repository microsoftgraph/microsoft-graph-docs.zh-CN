---
title: secureAssessmentAccountType 枚举类型
description: Windows10SecureAssessment ConfigurationAccount 允许的帐户类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7a459e086b0b6ec44e625ca8a0932ea96422699a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787577"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="42c34-103">secureAssessmentAccountType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="42c34-103">secureAssessmentAccountType enum type</span></span>

> <span data-ttu-id="42c34-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="42c34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42c34-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="42c34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42c34-106">Windows10SecureAssessment ConfigurationAccount 允许的帐户类型。</span><span class="sxs-lookup"><span data-stu-id="42c34-106">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>

## <a name="members"></a><span data-ttu-id="42c34-107">成员</span><span class="sxs-lookup"><span data-stu-id="42c34-107">Members</span></span>
|<span data-ttu-id="42c34-108">成员</span><span class="sxs-lookup"><span data-stu-id="42c34-108">Member</span></span>|<span data-ttu-id="42c34-109">值</span><span class="sxs-lookup"><span data-stu-id="42c34-109">Value</span></span>|<span data-ttu-id="42c34-110">说明</span><span class="sxs-lookup"><span data-stu-id="42c34-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42c34-111">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="42c34-111">azureADAccount</span></span>|<span data-ttu-id="42c34-112">0</span><span class="sxs-lookup"><span data-stu-id="42c34-112">0</span></span>|<span data-ttu-id="42c34-113">指示 AzureAD\username@tenant.com 格式的 Azure AD 帐户。</span><span class="sxs-lookup"><span data-stu-id="42c34-113">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="42c34-114">domainAccount</span><span class="sxs-lookup"><span data-stu-id="42c34-114">domainAccount</span></span>|<span data-ttu-id="42c34-115">1</span><span class="sxs-lookup"><span data-stu-id="42c34-115">1</span></span>|<span data-ttu-id="42c34-116">指示域帐户的格式为 domain\user 或 user@domain.com。</span><span class="sxs-lookup"><span data-stu-id="42c34-116">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="42c34-117">localAccount</span><span class="sxs-lookup"><span data-stu-id="42c34-117">localAccount</span></span>|<span data-ttu-id="42c34-118">双面</span><span class="sxs-lookup"><span data-stu-id="42c34-118">2</span></span>|<span data-ttu-id="42c34-119">指示本地帐户的用户名格式。</span><span class="sxs-lookup"><span data-stu-id="42c34-119">Indicates a local account in format of username.</span></span>|
|<span data-ttu-id="42c34-120">localGuestAccount</span><span class="sxs-lookup"><span data-stu-id="42c34-120">localGuestAccount</span></span>|<span data-ttu-id="42c34-121">第三章</span><span class="sxs-lookup"><span data-stu-id="42c34-121">3</span></span>|<span data-ttu-id="42c34-122">以测试名称的格式指示本地来宾帐户。</span><span class="sxs-lookup"><span data-stu-id="42c34-122">Indicates a local guest account in format of test name.</span></span>|



