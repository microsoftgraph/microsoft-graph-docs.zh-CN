---
title: microsoft Intune 中的公司条款和条件-microsoft Graph API
description: 列出支持公司条款和条件的适用于 Intune (REST) 终结点的 Microsoft Graph API。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 3de3cdf4ac55177bceb56e59743d0bef9bd4cb50
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253531"
---
# <a name="company-terms-and-conditions-in-microsoft-intune"></a><span data-ttu-id="8ca1b-103">Microsoft Intune 中的公司条款和条件</span><span class="sxs-lookup"><span data-stu-id="8ca1b-103">Company terms and conditions in Microsoft Intune</span></span>

> <span data-ttu-id="8ca1b-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8ca1b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="8ca1b-105">你可以将 Intune 条款和条件部署到用户组，以说明注册、访问工作资源和公司门户应用对设备和用户有何影响。</span><span class="sxs-lookup"><span data-stu-id="8ca1b-105">You can deploy Intune terms and conditions to user groups to explain how enrollment, access to work resources, and the Company Portal app affect devices and users.</span></span> <span data-ttu-id="8ca1b-106">用户必须接受条款和条件，才能使用公司门户注册和访问其工作。</span><span class="sxs-lookup"><span data-stu-id="8ca1b-106">Users must accept the terms and conditions before they can use the Company Portal to enroll and access their work.</span></span>

<span data-ttu-id="8ca1b-107">你可以创建和部署多个包含不同条款和条件的策略。</span><span class="sxs-lookup"><span data-stu-id="8ca1b-107">You can create and deploy multiple policies containing different terms and conditions.</span></span> <span data-ttu-id="8ca1b-108">也可以生成相同条款和条件的不同语言版本，并将其部署到相应组。</span><span class="sxs-lookup"><span data-stu-id="8ca1b-108">You can also produce versions of the same terms and conditions in different languages and then deploy these to their appropriate groups.</span></span>

<span data-ttu-id="8ca1b-109">以下 Graph 资源可用于管理 Intune 中的公司条款和条件：</span><span class="sxs-lookup"><span data-stu-id="8ca1b-109">The following Graph resources are available to manage company terms and conditions in Intune:</span></span>

- [<span data-ttu-id="8ca1b-110">条款和条件</span><span class="sxs-lookup"><span data-stu-id="8ca1b-110">Terms and conditions</span></span>](intune-companyterms-termsandconditions.md)
- [<span data-ttu-id="8ca1b-111">条款和条件接受状态</span><span class="sxs-lookup"><span data-stu-id="8ca1b-111">Terms and conditions acceptance status</span></span>](intune-companyterms-termsandconditionsacceptancestatus.md)
- [<span data-ttu-id="8ca1b-112">条款和条件分配</span><span class="sxs-lookup"><span data-stu-id="8ca1b-112">Terms and conditions assignment</span></span>](intune-companyterms-termsandconditionsassignment.md)
