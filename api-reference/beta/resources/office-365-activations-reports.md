---
title: Office 365 激活报表
description: Office 365 激活报告提供的用户已激活其至少一个设备上的 Office 365 订阅的视图。 它提供了 Office 365 ProPlus、 Project 和 Visio Pro for Office 365 订阅激活的细分以及激活的细分结构跨桌面和设备。 此报告可帮助您识别可能需要其他支持激活其 Office 订阅的用户。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 345ab500ef5986471bb801a88ee5886473a3dd60
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573675"
---
# <a name="office-365-activations-reports"></a><span data-ttu-id="db916-105">Office 365 激活报表</span><span class="sxs-lookup"><span data-stu-id="db916-105">Office 365 activations reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db916-106">Office 365 激活报告提供的用户已激活其至少一个设备上的 Office 365 订阅的视图。</span><span class="sxs-lookup"><span data-stu-id="db916-106">The Office 365 activation report gives you a view of which users have activated their Office 365 subscriptions on at least one device.</span></span> <span data-ttu-id="db916-107">它提供了 Office 365 ProPlus、 Project 和 Visio Pro for Office 365 订阅激活的细分以及激活的细分结构跨桌面和设备。</span><span class="sxs-lookup"><span data-stu-id="db916-107">It provides a breakdown of the Office 365 ProPlus, Project, and Visio Pro for Office 365 subscription activations, as well as the breakdown of activations across desktop and devices.</span></span> <span data-ttu-id="db916-108">此报告可帮助您识别可能需要其他支持激活其 Office 订阅的用户。</span><span class="sxs-lookup"><span data-stu-id="db916-108">This report could help you identify users who might need additional support to activate their Office subscription.</span></span>

> <span data-ttu-id="db916-109">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="db916-109">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="reports"></a><span data-ttu-id="db916-110">报表</span><span class="sxs-lookup"><span data-stu-id="db916-110">Reports</span></span>
| <span data-ttu-id="db916-111">函数</span><span class="sxs-lookup"><span data-stu-id="db916-111">Function</span></span>                                 | <span data-ttu-id="db916-112">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="db916-112">CSV return type</span></span> | <span data-ttu-id="db916-113">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="db916-113">JSON return type</span></span>                         | <span data-ttu-id="db916-114">说明</span><span class="sxs-lookup"><span data-stu-id="db916-114">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="db916-115">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="db916-115">Get user detail</span></span>](../api/reportroot-getoffice365activationsuserdetail.md) | <span data-ttu-id="db916-116">Stream</span><span class="sxs-lookup"><span data-stu-id="db916-116">Stream</span></span>          | [<span data-ttu-id="db916-117">office365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="db916-117">office365ActivationsUserDetail</span></span>](../resources/office365activationsuserdetail.md) | <span data-ttu-id="db916-118">获取已激活 Office 365 的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="db916-118">Get details about users who have activated Office 365.</span></span> |
| [<span data-ttu-id="db916-119">获取激活数</span><span class="sxs-lookup"><span data-stu-id="db916-119">Get activation counts</span></span>](../api/reportroot-getoffice365activationcounts.md) | <span data-ttu-id="db916-120">Stream</span><span class="sxs-lookup"><span data-stu-id="db916-120">Stream</span></span>          | [<span data-ttu-id="db916-121">office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="db916-121">office365ActivationCounts</span></span>](../resources/office365activationcounts.md) | <span data-ttu-id="db916-122">获取桌面和设备上激活的 Office 365 订阅数。</span><span class="sxs-lookup"><span data-stu-id="db916-122">Get the count of Office 365 activations on desktops and devices.</span></span> |
| [<span data-ttu-id="db916-123">获取用户数</span><span class="sxs-lookup"><span data-stu-id="db916-123">Get user counts</span></span>](../api/reportroot-getoffice365activationsusercounts.md) | <span data-ttu-id="db916-124">Stream</span><span class="sxs-lookup"><span data-stu-id="db916-124">Stream</span></span>          | [<span data-ttu-id="db916-125">office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="db916-125">office365ActivationsUserCounts</span></span>](../resources/office365activationsusercounts.md) | <span data-ttu-id="db916-126">获取在桌面或设备上激活 Office 订阅的已启用用户数。</span><span class="sxs-lookup"><span data-stu-id="db916-126">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-activations-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
