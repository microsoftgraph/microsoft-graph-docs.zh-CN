---
title: Office 365 活跃用户报表
description: Office 365 活跃用户报表可用于确定组织中个人使用的产品许可证数，并向下钻取哪些用户使用什么产品的相关信息。 此类报表有助于管理员发现未充分利用的产品或可能需要获取额外培训或信息的用户。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 163eab83bfcb5089ec21d449d90840384c12e4ef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447344"
---
# <a name="office-365-active-users-reports"></a><span data-ttu-id="b1821-104">Office 365 活跃用户报表</span><span class="sxs-lookup"><span data-stu-id="b1821-104">Office 365 active users reports</span></span>

<span data-ttu-id="b1821-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b1821-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b1821-106">Office 365 活跃用户报表可用于确定组织中个人使用的产品许可证数，并向下钻取哪些用户使用什么产品的相关信息。</span><span class="sxs-lookup"><span data-stu-id="b1821-106">You can use the Office 365 active users reports to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="b1821-107">此类报表有助于管理员发现未充分利用的产品或可能需要获取额外培训或信息的用户。</span><span class="sxs-lookup"><span data-stu-id="b1821-107">These reports can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="b1821-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="b1821-108">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="b1821-109">报表</span><span class="sxs-lookup"><span data-stu-id="b1821-109">Reports</span></span>
| <span data-ttu-id="b1821-110">函数</span><span class="sxs-lookup"><span data-stu-id="b1821-110">Function</span></span>                                 | <span data-ttu-id="b1821-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="b1821-111">Return Type</span></span> | <span data-ttu-id="b1821-112">说明</span><span class="sxs-lookup"><span data-stu-id="b1821-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="b1821-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="b1821-113">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="b1821-114">Stream</span><span class="sxs-lookup"><span data-stu-id="b1821-114">Stream</span></span>      | <span data-ttu-id="b1821-115">获取 Office 365 活跃用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b1821-115">Get details about Office 365 active users.</span></span> |
| [<span data-ttu-id="b1821-116">获取用户数</span><span class="sxs-lookup"><span data-stu-id="b1821-116">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="b1821-117">Stream</span><span class="sxs-lookup"><span data-stu-id="b1821-117">Stream</span></span>      | <span data-ttu-id="b1821-118">按产品获取报表周期内的每日活跃用户数。</span><span class="sxs-lookup"><span data-stu-id="b1821-118">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="b1821-119">获取服务用户数</span><span class="sxs-lookup"><span data-stu-id="b1821-119">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="b1821-120">Stream</span><span class="sxs-lookup"><span data-stu-id="b1821-120">Stream</span></span>      | <span data-ttu-id="b1821-121">按活动类型和服务获取用户数。</span><span class="sxs-lookup"><span data-stu-id="b1821-121">Get the count of users by activity type and service.</span></span> |
