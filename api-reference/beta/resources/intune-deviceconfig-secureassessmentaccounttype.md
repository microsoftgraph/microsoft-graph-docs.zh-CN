---
title: secureAssessmentAccountType 枚举类型
description: Windows10SecureAssessment ConfigurationAccount 允许的帐户的类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2f9e620f87173708b852bd7eac79bee5a45e432c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409879"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="3eb9d-103">secureAssessmentAccountType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3eb9d-103">secureAssessmentAccountType enum type</span></span>

> <span data-ttu-id="3eb9d-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="3eb9d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3eb9d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3eb9d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3eb9d-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3eb9d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3eb9d-107">Windows10SecureAssessment ConfigurationAccount 允许的帐户的类型。</span><span class="sxs-lookup"><span data-stu-id="3eb9d-107">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>

## <a name="members"></a><span data-ttu-id="3eb9d-108">成员</span><span class="sxs-lookup"><span data-stu-id="3eb9d-108">Members</span></span>
|<span data-ttu-id="3eb9d-109">成员</span><span class="sxs-lookup"><span data-stu-id="3eb9d-109">Member</span></span>|<span data-ttu-id="3eb9d-110">值</span><span class="sxs-lookup"><span data-stu-id="3eb9d-110">Value</span></span>|<span data-ttu-id="3eb9d-111">说明</span><span class="sxs-lookup"><span data-stu-id="3eb9d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3eb9d-112">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="3eb9d-112">azureADAccount</span></span>|<span data-ttu-id="3eb9d-113">0</span><span class="sxs-lookup"><span data-stu-id="3eb9d-113">0</span></span>|<span data-ttu-id="3eb9d-114">指示的 AzureAD\ username@tenant.com 格式中的 Azure AD 帐户。</span><span class="sxs-lookup"><span data-stu-id="3eb9d-114">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="3eb9d-115">domainAccount</span><span class="sxs-lookup"><span data-stu-id="3eb9d-115">domainAccount</span></span>|<span data-ttu-id="3eb9d-116">1</span><span class="sxs-lookup"><span data-stu-id="3eb9d-116">1</span></span>|<span data-ttu-id="3eb9d-117">指示以 domain\user 或 user@domain.com 格式为域帐户。</span><span class="sxs-lookup"><span data-stu-id="3eb9d-117">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="3eb9d-118">本地帐户</span><span class="sxs-lookup"><span data-stu-id="3eb9d-118">localAccount</span></span>|<span data-ttu-id="3eb9d-119">2</span><span class="sxs-lookup"><span data-stu-id="3eb9d-119">2</span></span>|<span data-ttu-id="3eb9d-120">指示本地帐户的用户名的格式。</span><span class="sxs-lookup"><span data-stu-id="3eb9d-120">Indicates a local account in format of username.</span></span>|




