---
title: Microsoft 365 激活报告
description: Microsoft 365 激活报告可让你查看哪些用户在至少一台设备上激活了 Microsoft 365 订阅。 这些报告提供了 Microsoft 365 专业增强版、Project 和 Visio Pro for Office 365 订阅激活的细目，以及跨桌面和设备激活的细分。 此类报表有助于发现可能需要额外支持才能激活 Office 订阅的用户。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 30d9fa1799367e0589115c56dd069db6ca7b1ff9
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981044"
---
# <a name="microsoft-365-activations-reports"></a><span data-ttu-id="42e34-105">Microsoft 365 激活报告</span><span class="sxs-lookup"><span data-stu-id="42e34-105">Microsoft 365 activations reports</span></span>

<span data-ttu-id="42e34-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42e34-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="42e34-107">Microsoft 365 激活报告可让你查看哪些用户在至少一台设备上激活了 Microsoft 365 订阅。</span><span class="sxs-lookup"><span data-stu-id="42e34-107">The Microsoft 365 activation reports can give you a view of which users have activated their Microsoft 365 subscriptions on at least one device.</span></span> <span data-ttu-id="42e34-108">这些报告提供了 Microsoft 365 专业增强版、Project 和 Visio Pro for Office 365 订阅激活的细目，以及跨桌面和设备激活的细分。</span><span class="sxs-lookup"><span data-stu-id="42e34-108">These reports provide a breakdown of the Microsoft 365 ProPlus, Project, and Visio Pro for Office 365 subscription activations, as well as the breakdown of activations across desktop and devices.</span></span> <span data-ttu-id="42e34-109">此类报表有助于发现可能需要额外支持才能激活 Office 订阅的用户。</span><span class="sxs-lookup"><span data-stu-id="42e34-109">These reports could help you identify users who might need additional support to activate their Office subscription.</span></span>

> <span data-ttu-id="42e34-110">**注意：** 有关不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 -](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)Microsoft Office激活。</span><span class="sxs-lookup"><span data-stu-id="42e34-110">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="reports"></a><span data-ttu-id="42e34-111">报告</span><span class="sxs-lookup"><span data-stu-id="42e34-111">Reports</span></span>
| <span data-ttu-id="42e34-112">函数</span><span class="sxs-lookup"><span data-stu-id="42e34-112">Function</span></span>                                 | <span data-ttu-id="42e34-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="42e34-113">Return Type</span></span> | <span data-ttu-id="42e34-114">说明</span><span class="sxs-lookup"><span data-stu-id="42e34-114">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="42e34-115">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="42e34-115">Get user detail</span></span>](../api/reportroot-getoffice365activationsuserdetail.md) | <span data-ttu-id="42e34-116">Stream</span><span class="sxs-lookup"><span data-stu-id="42e34-116">Stream</span></span>      | <span data-ttu-id="42e34-117">获取有关已激活 Microsoft 365 的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="42e34-117">Get details about users who have activated Microsoft 365.</span></span> |
| [<span data-ttu-id="42e34-118">获取激活数</span><span class="sxs-lookup"><span data-stu-id="42e34-118">Get activation counts</span></span>](../api/reportroot-getoffice365activationcounts.md) | <span data-ttu-id="42e34-119">Stream</span><span class="sxs-lookup"><span data-stu-id="42e34-119">Stream</span></span>      | <span data-ttu-id="42e34-120">获取桌面和设备上 Microsoft 365 激活的计数。</span><span class="sxs-lookup"><span data-stu-id="42e34-120">Get the count of Microsoft 365 activations on desktops and devices.</span></span> |
| [<span data-ttu-id="42e34-121">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="42e34-121">Get user counts</span></span>](../api/reportroot-getoffice365activationsusercounts.md) | <span data-ttu-id="42e34-122">Stream</span><span class="sxs-lookup"><span data-stu-id="42e34-122">Stream</span></span>      | <span data-ttu-id="42e34-123">获取在桌面或设备上激活 Office 订阅的已启用用户数。</span><span class="sxs-lookup"><span data-stu-id="42e34-123">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices.</span></span> |

