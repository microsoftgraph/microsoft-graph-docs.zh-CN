---
title: Microsoft 365 激活报告
description: Microsoft 365 激活报告可让你查看在至少一个设备上已激活其 Microsoft 365 订阅的用户。 这些报告提供了 Microsoft 365 专业增强版、Project 和 Visio Pro for Office 365 订阅激活的细目，以及跨桌面和设备的激活细目。 此类报表有助于发现可能需要额外支持才能激活 Office 订阅的用户。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: ebca76ca3fe9356839636e7dca29293b083c13ff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970668"
---
# <a name="microsoft-365-activations-reports"></a><span data-ttu-id="7ca1c-105">Microsoft 365 激活报告</span><span class="sxs-lookup"><span data-stu-id="7ca1c-105">Microsoft 365 activations reports</span></span>

<span data-ttu-id="7ca1c-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ca1c-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7ca1c-107">Microsoft 365 激活报告可让你查看在至少一个设备上已激活其 Microsoft 365 订阅的用户。</span><span class="sxs-lookup"><span data-stu-id="7ca1c-107">The Microsoft 365 activation reports can give you a view of which users have activated their Microsoft 365 subscriptions on at least one device.</span></span> <span data-ttu-id="7ca1c-108">这些报告提供了 Microsoft 365 专业增强版、Project 和 Visio Pro for Office 365 订阅激活的细目，以及跨桌面和设备的激活细目。</span><span class="sxs-lookup"><span data-stu-id="7ca1c-108">These reports provide a breakdown of the Microsoft 365 ProPlus, Project, and Visio Pro for Office 365 subscription activations, as well as the breakdown of activations across desktop and devices.</span></span> <span data-ttu-id="7ca1c-109">此类报表有助于发现可能需要额外支持才能激活 Office 订阅的用户。</span><span class="sxs-lookup"><span data-stu-id="7ca1c-109">These reports could help you identify users who might need additional support to activate their Office subscription.</span></span>

> <span data-ttu-id="7ca1c-110">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [microsoft 365 报表-Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。</span><span class="sxs-lookup"><span data-stu-id="7ca1c-110">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="reports"></a><span data-ttu-id="7ca1c-111">报表</span><span class="sxs-lookup"><span data-stu-id="7ca1c-111">Reports</span></span>
| <span data-ttu-id="7ca1c-112">函数</span><span class="sxs-lookup"><span data-stu-id="7ca1c-112">Function</span></span>                                 | <span data-ttu-id="7ca1c-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="7ca1c-113">Return Type</span></span> | <span data-ttu-id="7ca1c-114">说明</span><span class="sxs-lookup"><span data-stu-id="7ca1c-114">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="7ca1c-115">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="7ca1c-115">Get user detail</span></span>](../api/reportroot-getoffice365activationsuserdetail.md) | <span data-ttu-id="7ca1c-116">Stream</span><span class="sxs-lookup"><span data-stu-id="7ca1c-116">Stream</span></span>      | <span data-ttu-id="7ca1c-117">获取已激活 Microsoft 365 的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7ca1c-117">Get details about users who have activated Microsoft 365.</span></span> |
| [<span data-ttu-id="7ca1c-118">获取激活数</span><span class="sxs-lookup"><span data-stu-id="7ca1c-118">Get activation counts</span></span>](../api/reportroot-getoffice365activationcounts.md) | <span data-ttu-id="7ca1c-119">Stream</span><span class="sxs-lookup"><span data-stu-id="7ca1c-119">Stream</span></span>      | <span data-ttu-id="7ca1c-120">获取桌面和设备上的 Microsoft 365 激活次数。</span><span class="sxs-lookup"><span data-stu-id="7ca1c-120">Get the count of Microsoft 365 activations on desktops and devices.</span></span> |
| [<span data-ttu-id="7ca1c-121">获取用户数</span><span class="sxs-lookup"><span data-stu-id="7ca1c-121">Get user counts</span></span>](../api/reportroot-getoffice365activationsusercounts.md) | <span data-ttu-id="7ca1c-122">Stream</span><span class="sxs-lookup"><span data-stu-id="7ca1c-122">Stream</span></span>      | <span data-ttu-id="7ca1c-123">获取在桌面或设备上激活 Office 订阅的已启用用户数。</span><span class="sxs-lookup"><span data-stu-id="7ca1c-123">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices.</span></span> |

