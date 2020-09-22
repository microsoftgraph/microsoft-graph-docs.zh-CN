---
title: Microsoft 365 激活报告
description: Microsoft 365 激活报告为您提供了一个用户在至少一个设备上激活其 Microsoft 365 订阅的视图。 它提供了 Microsoft 365 专业增强版、Project 和 Visio Pro for Microsoft 365 订阅激活的细目，以及跨桌面和设备的激活细目。 此报告可帮助您确定可能需要其他支持才能激活 Office 订阅的用户。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 86a418e75fee70d16009f0ab6f8a3f0f474760cd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021257"
---
# <a name="microsoft-365-activations-reports"></a><span data-ttu-id="1b728-105">Microsoft 365 激活报告</span><span class="sxs-lookup"><span data-stu-id="1b728-105">Microsoft 365 activations reports</span></span>

<span data-ttu-id="1b728-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b728-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b728-107">Microsoft 365 激活报告为您提供了一个用户在至少一个设备上激活其 Microsoft 365 订阅的视图。</span><span class="sxs-lookup"><span data-stu-id="1b728-107">The Microsoft 365 activation report gives you a view of which users have activated their Microsoft 365 subscriptions on at least one device.</span></span> <span data-ttu-id="1b728-108">它提供了 Microsoft 365 专业增强版、Project 和 Visio Pro for Microsoft 365 订阅激活的细目，以及跨桌面和设备的激活细目。</span><span class="sxs-lookup"><span data-stu-id="1b728-108">It provides a breakdown of the Microsoft 365 ProPlus, Project, and Visio Pro for Microsoft 365 subscription activations, as well as the breakdown of activations across desktop and devices.</span></span> <span data-ttu-id="1b728-109">此报告可帮助您确定可能需要其他支持才能激活 Office 订阅的用户。</span><span class="sxs-lookup"><span data-stu-id="1b728-109">This report could help you identify users who might need additional support to activate their Office subscription.</span></span>

> <span data-ttu-id="1b728-110">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [microsoft 365 报表-Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="1b728-110">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="reports"></a><span data-ttu-id="1b728-111">报表</span><span class="sxs-lookup"><span data-stu-id="1b728-111">Reports</span></span>
| <span data-ttu-id="1b728-112">函数</span><span class="sxs-lookup"><span data-stu-id="1b728-112">Function</span></span>                                 | <span data-ttu-id="1b728-113">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="1b728-113">CSV return type</span></span> | <span data-ttu-id="1b728-114">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="1b728-114">JSON return type</span></span>                         | <span data-ttu-id="1b728-115">说明</span><span class="sxs-lookup"><span data-stu-id="1b728-115">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="1b728-116">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="1b728-116">Get user detail</span></span>](../api/reportroot-getoffice365activationsuserdetail.md) | <span data-ttu-id="1b728-117">Stream</span><span class="sxs-lookup"><span data-stu-id="1b728-117">Stream</span></span>          | [<span data-ttu-id="1b728-118">office365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="1b728-118">office365ActivationsUserDetail</span></span>](../resources/office365activationsuserdetail.md) | <span data-ttu-id="1b728-119">获取已激活 Microsoft 365 的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1b728-119">Get details about users who have activated Microsoft 365.</span></span> |
| [<span data-ttu-id="1b728-120">获取激活数</span><span class="sxs-lookup"><span data-stu-id="1b728-120">Get activation counts</span></span>](../api/reportroot-getoffice365activationcounts.md) | <span data-ttu-id="1b728-121">Stream</span><span class="sxs-lookup"><span data-stu-id="1b728-121">Stream</span></span>          | [<span data-ttu-id="1b728-122">office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="1b728-122">office365ActivationCounts</span></span>](../resources/office365activationcounts.md) | <span data-ttu-id="1b728-123">获取桌面和设备上的 Microsoft 365 激活次数。</span><span class="sxs-lookup"><span data-stu-id="1b728-123">Get the count of Microsoft 365 activations on desktops and devices.</span></span> |
| [<span data-ttu-id="1b728-124">获取用户数</span><span class="sxs-lookup"><span data-stu-id="1b728-124">Get user counts</span></span>](../api/reportroot-getoffice365activationsusercounts.md) | <span data-ttu-id="1b728-125">Stream</span><span class="sxs-lookup"><span data-stu-id="1b728-125">Stream</span></span>          | [<span data-ttu-id="1b728-126">office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="1b728-126">office365ActivationsUserCounts</span></span>](../resources/office365activationsusercounts.md) | <span data-ttu-id="1b728-127">获取在桌面或设备上激活 Office 订阅的已启用用户数。</span><span class="sxs-lookup"><span data-stu-id="1b728-127">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices.</span></span> |


