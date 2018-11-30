---
title: secureAssessmentAccountType 枚举类型
description: Windows10SecureAssessment ConfigurationAccount 允许的帐户的类型。
ms.openlocfilehash: 97dc60d8d15e90c43923d939cf957e1092b2cc45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047547"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="ffd22-103">secureAssessmentAccountType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ffd22-103">secureAssessmentAccountType enum type</span></span>

> <span data-ttu-id="ffd22-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ffd22-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ffd22-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ffd22-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ffd22-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ffd22-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ffd22-107">Windows10SecureAssessment ConfigurationAccount 允许的帐户的类型。</span><span class="sxs-lookup"><span data-stu-id="ffd22-107">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>
## <a name="members"></a><span data-ttu-id="ffd22-108">成员</span><span class="sxs-lookup"><span data-stu-id="ffd22-108">Members</span></span>
|<span data-ttu-id="ffd22-109">成员</span><span class="sxs-lookup"><span data-stu-id="ffd22-109">Member</span></span>|<span data-ttu-id="ffd22-110">值</span><span class="sxs-lookup"><span data-stu-id="ffd22-110">Value</span></span>|<span data-ttu-id="ffd22-111">说明</span><span class="sxs-lookup"><span data-stu-id="ffd22-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffd22-112">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="ffd22-112">azureADAccount</span></span>|<span data-ttu-id="ffd22-113">0</span><span class="sxs-lookup"><span data-stu-id="ffd22-113">0</span></span>|<span data-ttu-id="ffd22-114">指示的 AzureAD\ username@tenant.com 格式中的 Azure AD 帐户。</span><span class="sxs-lookup"><span data-stu-id="ffd22-114">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="ffd22-115">domainAccount</span><span class="sxs-lookup"><span data-stu-id="ffd22-115">domainAccount</span></span>|<span data-ttu-id="ffd22-116">1</span><span class="sxs-lookup"><span data-stu-id="ffd22-116">1</span></span>|<span data-ttu-id="ffd22-117">指示以 domain\user 或 user@domain.com 格式为域帐户。</span><span class="sxs-lookup"><span data-stu-id="ffd22-117">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="ffd22-118">本地帐户</span><span class="sxs-lookup"><span data-stu-id="ffd22-118">localAccount</span></span>|<span data-ttu-id="ffd22-119">2</span><span class="sxs-lookup"><span data-stu-id="ffd22-119">2</span></span>|<span data-ttu-id="ffd22-120">指示本地帐户的用户名的格式。</span><span class="sxs-lookup"><span data-stu-id="ffd22-120">Indicates a local account in format of username.</span></span>|





