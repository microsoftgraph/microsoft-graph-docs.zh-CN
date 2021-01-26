---
title: Microsoft 365 激活报告
description: Microsoft 365 激活报告可让你查看哪些用户在至少一台设备上激活了 Microsoft 365 订阅。 它提供了 Microsoft 365 专业增强版、Project 和 Visio Pro for Microsoft 365 订阅激活的细目，以及跨桌面和设备激活的细分。 此报告可以帮助您识别可能需要额外支持才能激活其 Office 订阅的用户。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 32fb2f1397218a5d6c99b071b7a398cf00cd54f7
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980792"
---
# <a name="microsoft-365-activations-reports"></a><span data-ttu-id="894ef-105">Microsoft 365 激活报告</span><span class="sxs-lookup"><span data-stu-id="894ef-105">Microsoft 365 activations reports</span></span>

<span data-ttu-id="894ef-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="894ef-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="894ef-107">Microsoft 365 激活报告可让你查看哪些用户在至少一台设备上激活了 Microsoft 365 订阅。</span><span class="sxs-lookup"><span data-stu-id="894ef-107">The Microsoft 365 activation report gives you a view of which users have activated their Microsoft 365 subscriptions on at least one device.</span></span> <span data-ttu-id="894ef-108">它提供了 Microsoft 365 专业增强版、Project 和 Visio Pro for Microsoft 365 订阅激活的细目，以及跨桌面和设备激活的细分。</span><span class="sxs-lookup"><span data-stu-id="894ef-108">It provides a breakdown of the Microsoft 365 ProPlus, Project, and Visio Pro for Microsoft 365 subscription activations, as well as the breakdown of activations across desktop and devices.</span></span> <span data-ttu-id="894ef-109">此报告可以帮助您识别可能需要额外支持才能激活其 Office 订阅的用户。</span><span class="sxs-lookup"><span data-stu-id="894ef-109">This report could help you identify users who might need additional support to activate their Office subscription.</span></span>

> <span data-ttu-id="894ef-110">**注意：** 有关不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 -](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)Microsoft Office激活。</span><span class="sxs-lookup"><span data-stu-id="894ef-110">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="reports"></a><span data-ttu-id="894ef-111">报告</span><span class="sxs-lookup"><span data-stu-id="894ef-111">Reports</span></span>
| <span data-ttu-id="894ef-112">函数</span><span class="sxs-lookup"><span data-stu-id="894ef-112">Function</span></span>                                 | <span data-ttu-id="894ef-113">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="894ef-113">CSV return type</span></span> | <span data-ttu-id="894ef-114">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="894ef-114">JSON return type</span></span>                         | <span data-ttu-id="894ef-115">说明</span><span class="sxs-lookup"><span data-stu-id="894ef-115">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="894ef-116">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="894ef-116">Get user detail</span></span>](../api/reportroot-getoffice365activationsuserdetail.md) | <span data-ttu-id="894ef-117">Stream</span><span class="sxs-lookup"><span data-stu-id="894ef-117">Stream</span></span>          | [<span data-ttu-id="894ef-118">office365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="894ef-118">office365ActivationsUserDetail</span></span>](../resources/office365activationsuserdetail.md) | <span data-ttu-id="894ef-119">获取有关已激活 Microsoft 365 的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="894ef-119">Get details about users who have activated Microsoft 365.</span></span> |
| [<span data-ttu-id="894ef-120">获取激活数</span><span class="sxs-lookup"><span data-stu-id="894ef-120">Get activation counts</span></span>](../api/reportroot-getoffice365activationcounts.md) | <span data-ttu-id="894ef-121">Stream</span><span class="sxs-lookup"><span data-stu-id="894ef-121">Stream</span></span>          | [<span data-ttu-id="894ef-122">office365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="894ef-122">office365ActivationCounts</span></span>](../resources/office365activationcounts.md) | <span data-ttu-id="894ef-123">获取桌面和设备上 Microsoft 365 激活的计数。</span><span class="sxs-lookup"><span data-stu-id="894ef-123">Get the count of Microsoft 365 activations on desktops and devices.</span></span> |
| [<span data-ttu-id="894ef-124">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="894ef-124">Get user counts</span></span>](../api/reportroot-getoffice365activationsusercounts.md) | <span data-ttu-id="894ef-125">Stream</span><span class="sxs-lookup"><span data-stu-id="894ef-125">Stream</span></span>          | [<span data-ttu-id="894ef-126">office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="894ef-126">office365ActivationsUserCounts</span></span>](../resources/office365activationsusercounts.md) | <span data-ttu-id="894ef-127">获取在桌面或设备上激活 Office 订阅的已启用用户数。</span><span class="sxs-lookup"><span data-stu-id="894ef-127">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices.</span></span> |


