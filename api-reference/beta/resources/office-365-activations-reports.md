---
title: Office 365 激活报表
description: Office 365 激活报告为您提供了一个用户在至少一个设备上激活其 Office 365 订阅的视图。 它提供了 office 365 专业增强版、Project 和 Visio Pro for office 365 订阅激活的细目, 以及跨桌面和设备的激活细目。 此报告可帮助您确定可能需要其他支持才能激活 Office 订阅的用户。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 345ab500ef5986471bb801a88ee5886473a3dd60
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581545"
---
# <a name="office-365-activations-reports"></a><span data-ttu-id="3e627-105">Office 365 激活报表</span><span class="sxs-lookup"><span data-stu-id="3e627-105">Office 365 activations reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e627-106">Office 365 激活报告为您提供了一个用户在至少一个设备上激活其 Office 365 订阅的视图。</span><span class="sxs-lookup"><span data-stu-id="3e627-106">The Office 365 activation report gives you a view of which users have activated their Office 365 subscriptions on at least one device.</span></span> <span data-ttu-id="3e627-107">它提供了 office 365 专业增强版、Project 和 Visio Pro for office 365 订阅激活的细目, 以及跨桌面和设备的激活细目。</span><span class="sxs-lookup"><span data-stu-id="3e627-107">It provides a breakdown of the Office 365 ProPlus, Project, and Visio Pro for Office 365 subscription activations, as well as the breakdown of activations across desktop and devices.</span></span> <span data-ttu-id="3e627-108">此报告可帮助您确定可能需要其他支持才能激活 Office 订阅的用户。</span><span class="sxs-lookup"><span data-stu-id="3e627-108">This report could help you identify users who might need additional support to activate their Office subscription.</span></span>

> <span data-ttu-id="3e627-109">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="3e627-109">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="reports"></a><span data-ttu-id="3e627-110">报表</span><span class="sxs-lookup"><span data-stu-id="3e627-110">Reports</span></span>
| <span data-ttu-id="3e627-111">函数</span><span class="sxs-lookup"><span data-stu-id="3e627-111">Function</span></span>                                 | <span data-ttu-id="3e627-112">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="3e627-112">CSV return type</span></span> | <span data-ttu-id="3e627-113">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="3e627-113">JSON return type</span></span>                         | <span data-ttu-id="3e627-114">说明</span><span class="sxs-lookup"><span data-stu-id="3e627-114">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="3e627-115">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="3e627-115">Get user detail</span></span>](../api/reportroot-getoffice365activationsuserdetail.md) | <span data-ttu-id="3e627-116">Stream</span><span class="sxs-lookup"><span data-stu-id="3e627-116">Stream</span></span>          | [<span data-ttu-id="3e627-117">office365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="3e627-117">office365ActivationsUserDetail</span></span>](../resources/office365activationsuserdetail.md) | <span data-ttu-id="3e627-118">获取已激活 Office 365 的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3e627-118">Get details about users who have activated Office 365.</span></span> |
| [<span data-ttu-id="3e627-119">获取激活数</span><span class="sxs-lookup"><span data-stu-id="3e627-119">Get activation counts</span></span>](../api/reportroot-getoffice365activationcounts.md) | <span data-ttu-id="3e627-120">Stream</span><span class="sxs-lookup"><span data-stu-id="3e627-120">Stream</span></span>          | [<span data-ttu-id="3e627-121">office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="3e627-121">office365ActivationCounts</span></span>](../resources/office365activationcounts.md) | <span data-ttu-id="3e627-122">获取桌面和设备上激活的 Office 365 订阅数。</span><span class="sxs-lookup"><span data-stu-id="3e627-122">Get the count of Office 365 activations on desktops and devices.</span></span> |
| [<span data-ttu-id="3e627-123">获取用户数</span><span class="sxs-lookup"><span data-stu-id="3e627-123">Get user counts</span></span>](../api/reportroot-getoffice365activationsusercounts.md) | <span data-ttu-id="3e627-124">Stream</span><span class="sxs-lookup"><span data-stu-id="3e627-124">Stream</span></span>          | [<span data-ttu-id="3e627-125">office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="3e627-125">office365ActivationsUserCounts</span></span>](../resources/office365activationsusercounts.md) | <span data-ttu-id="3e627-126">获取在桌面或设备上激活 Office 订阅的已启用用户数。</span><span class="sxs-lookup"><span data-stu-id="3e627-126">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-activations-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
