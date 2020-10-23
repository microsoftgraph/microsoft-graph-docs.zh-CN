---
title: Microsoft Intune 中的公司条款和条件-Microsoft Graph API
description: 列出用于定义租户组织的条款和条件 (REST) 的适用于 Intune 终结点的 Microsoft Graph API。
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 439fd1b4a59a196057210aafd56d9a938573cc45
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723967"
---
# <a name="company-terms-and-conditions-in-microsoft-intune"></a><span data-ttu-id="328ca-103">Microsoft Intune 中的公司条款和条件</span><span class="sxs-lookup"><span data-stu-id="328ca-103">Company terms and conditions in Microsoft Intune</span></span>

<span data-ttu-id="328ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="328ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="328ca-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="328ca-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="328ca-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="328ca-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="328ca-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="328ca-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="328ca-108">你可以将 Intune 条款和条件部署到用户组，以说明注册、访问工作资源和公司门户应用对设备和用户有何影响。</span><span class="sxs-lookup"><span data-stu-id="328ca-108">You can deploy Intune terms and conditions to user groups to explain how enrollment, access to work resources, and the Company Portal app affect devices and users.</span></span> <span data-ttu-id="328ca-109">用户必须接受条款和条件，才能使用公司门户注册和访问其工作。</span><span class="sxs-lookup"><span data-stu-id="328ca-109">Users must accept the terms and conditions before they can use the Company Portal to enroll and access their work.</span></span>

<span data-ttu-id="328ca-110">你可以创建和部署多个包含不同条款和条件的策略。</span><span class="sxs-lookup"><span data-stu-id="328ca-110">You can create and deploy multiple policies containing different terms and conditions.</span></span> <span data-ttu-id="328ca-111">也可以生成相同条款和条件的不同语言版本，并将其部署到相应组。</span><span class="sxs-lookup"><span data-stu-id="328ca-111">You can also produce versions of the same terms and conditions in different languages and then deploy these to their appropriate groups.</span></span>

<span data-ttu-id="328ca-112">以下 Graph 资源可用于管理 Intune 中的公司条款和条件：</span><span class="sxs-lookup"><span data-stu-id="328ca-112">The following Graph resources are available to manage company terms and conditions in Intune:</span></span>

- [<span data-ttu-id="328ca-113">条款和条件</span><span class="sxs-lookup"><span data-stu-id="328ca-113">Terms and conditions</span></span>](intune-companyterms-termsandconditions.md)
- [<span data-ttu-id="328ca-114">条款和条件接受状态</span><span class="sxs-lookup"><span data-stu-id="328ca-114">Terms and conditions acceptance status</span></span>](intune-companyterms-termsandconditionsacceptancestatus.md)
- [<span data-ttu-id="328ca-115">条款和条件分配</span><span class="sxs-lookup"><span data-stu-id="328ca-115">Terms and conditions assignment</span></span>](intune-companyterms-termsandconditionsassignment.md)
- [<span data-ttu-id="328ca-116">条款和条件组分配</span><span class="sxs-lookup"><span data-stu-id="328ca-116">Terms and conditions group assignment</span></span>](intune-companyterms-termsandconditionsgroupassignment.md)