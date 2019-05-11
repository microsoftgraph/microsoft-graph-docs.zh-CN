---
title: Microsoft Intune 中的公司条款和条件-Microsoft Graph API
description: 列出用于定义租户组织的条款和条件的 Intune 终结点 (REST) 的 Microsoft Graph API。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: 39ae30354d14fec7b056b40fc72c661b9ea7ba93
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949841"
---
# <a name="company-terms-and-conditions-in-microsoft-intune"></a><span data-ttu-id="6ba4b-103">Microsoft Intune 中的公司条款和条件</span><span class="sxs-lookup"><span data-stu-id="6ba4b-103">Company terms and conditions in Microsoft Intune</span></span>

> <span data-ttu-id="6ba4b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6ba4b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ba4b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6ba4b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6ba4b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6ba4b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="6ba4b-107">你可以将 Intune 条款和条件部署到用户组，以说明注册、访问工作资源和公司门户应用对设备和用户有何影响。</span><span class="sxs-lookup"><span data-stu-id="6ba4b-107">You can deploy Intune terms and conditions to user groups to explain how enrollment, access to work resources, and the Company Portal app affect devices and users.</span></span> <span data-ttu-id="6ba4b-108">用户必须接受条款和条件，才能使用公司门户注册和访问其工作。</span><span class="sxs-lookup"><span data-stu-id="6ba4b-108">Users must accept the terms and conditions before they can use the Company Portal to enroll and access their work.</span></span>

<span data-ttu-id="6ba4b-109">你可以创建和部署多个包含不同条款和条件的策略。</span><span class="sxs-lookup"><span data-stu-id="6ba4b-109">You can create and deploy multiple policies containing different terms and conditions.</span></span> <span data-ttu-id="6ba4b-110">也可以生成相同条款和条件的不同语言版本，并将其部署到相应组。</span><span class="sxs-lookup"><span data-stu-id="6ba4b-110">You can also produce versions of the same terms and conditions in different languages and then deploy these to their appropriate groups.</span></span>

<span data-ttu-id="6ba4b-111">以下 Graph 资源可用于管理 Intune 中的公司条款和条件：</span><span class="sxs-lookup"><span data-stu-id="6ba4b-111">The following Graph resources are available to manage company terms and conditions in Intune:</span></span>

- [<span data-ttu-id="6ba4b-112">条款和条件</span><span class="sxs-lookup"><span data-stu-id="6ba4b-112">Terms and conditions</span></span>](intune-companyterms-termsandconditions.md)
- [<span data-ttu-id="6ba4b-113">条款和条件接受状态</span><span class="sxs-lookup"><span data-stu-id="6ba4b-113">Terms and conditions acceptance status</span></span>](intune-companyterms-termsandconditionsacceptancestatus.md)
- [<span data-ttu-id="6ba4b-114">条款和条件分配</span><span class="sxs-lookup"><span data-stu-id="6ba4b-114">Terms and conditions assignment</span></span>](intune-companyterms-termsandconditionsassignment.md)
- [<span data-ttu-id="6ba4b-115">条款和条件组分配</span><span class="sxs-lookup"><span data-stu-id="6ba4b-115">Terms and conditions group assignment</span></span>](intune-companyterms-termsandconditionsgroupassignment.md)
