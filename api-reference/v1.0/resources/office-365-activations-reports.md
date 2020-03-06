---
title: Office 365 激活报表
description: Office 365 激活报表可用于了解哪些用户在至少一台设备上激活了 Office 365 订阅。 此类报表包含 Office 365 专业增强版、Project 和 Visio Pro for Office 365 订阅激活细目，以及跨桌面和设备激活细目。 此类报表有助于发现可能需要额外支持才能激活 Office 订阅的用户。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: d01f3116f6a6a12753384ec41c2cee609b9b7f8a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534181"
---
# <a name="office-365-activations-reports"></a><span data-ttu-id="dc36e-105">Office 365 激活报表</span><span class="sxs-lookup"><span data-stu-id="dc36e-105">Office 365 activations reports</span></span>

<span data-ttu-id="dc36e-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc36e-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dc36e-107">Office 365 激活报表可用于了解哪些用户在至少一台设备上激活了 Office 365 订阅。</span><span class="sxs-lookup"><span data-stu-id="dc36e-107">The Office 365 activation reports can give you a view of which users have activated their Office 365 subscriptions on at least one device.</span></span> <span data-ttu-id="dc36e-108">此类报表包含 Office 365 专业增强版、Project 和 Visio Pro for Office 365 订阅激活细目，以及跨桌面和设备激活细目。</span><span class="sxs-lookup"><span data-stu-id="dc36e-108">These reports provide a breakdown of the Office 365 ProPlus, Project, and Visio Pro for Office 365 subscription activations, as well as the breakdown of activations across desktop and devices.</span></span> <span data-ttu-id="dc36e-109">此类报表有助于发现可能需要额外支持才能激活 Office 订阅的用户。</span><span class="sxs-lookup"><span data-stu-id="dc36e-109">These reports could help you identify users who might need additional support to activate their Office subscription.</span></span>

> <span data-ttu-id="dc36e-110">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="dc36e-110">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="reports"></a><span data-ttu-id="dc36e-111">报表</span><span class="sxs-lookup"><span data-stu-id="dc36e-111">Reports</span></span>
| <span data-ttu-id="dc36e-112">函数</span><span class="sxs-lookup"><span data-stu-id="dc36e-112">Function</span></span>                                 | <span data-ttu-id="dc36e-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="dc36e-113">Return Type</span></span> | <span data-ttu-id="dc36e-114">说明</span><span class="sxs-lookup"><span data-stu-id="dc36e-114">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="dc36e-115">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="dc36e-115">Get user detail</span></span>](../api/reportroot-getoffice365activationsuserdetail.md) | <span data-ttu-id="dc36e-116">Stream</span><span class="sxs-lookup"><span data-stu-id="dc36e-116">Stream</span></span>      | <span data-ttu-id="dc36e-117">获取已激活 Office 365 的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="dc36e-117">Get details about users who have activated Office 365.</span></span> |
| [<span data-ttu-id="dc36e-118">获取激活数</span><span class="sxs-lookup"><span data-stu-id="dc36e-118">Get activation counts</span></span>](../api/reportroot-getoffice365activationcounts.md) | <span data-ttu-id="dc36e-119">Stream</span><span class="sxs-lookup"><span data-stu-id="dc36e-119">Stream</span></span>      | <span data-ttu-id="dc36e-120">获取桌面和设备上激活的 Office 365 订阅数。</span><span class="sxs-lookup"><span data-stu-id="dc36e-120">Get the count of Office 365 activations on desktops and devices.</span></span> |
| [<span data-ttu-id="dc36e-121">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="dc36e-121">Get user counts</span></span>](../api/reportroot-getoffice365activationsusercounts.md) | <span data-ttu-id="dc36e-122">Stream</span><span class="sxs-lookup"><span data-stu-id="dc36e-122">Stream</span></span>      | <span data-ttu-id="dc36e-123">获取在桌面或设备上激活 Office 订阅的已启用用户数。</span><span class="sxs-lookup"><span data-stu-id="dc36e-123">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices.</span></span> |
