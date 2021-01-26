---
title: Microsoft 365 活动用户报告
description: 可以使用 Microsoft 365 活动用户报告来了解组织中个人使用的产品许可证数量，并深入了解哪些用户正在使用哪些产品。 此类报表有助于管理员发现未充分利用的产品或可能需要获取额外培训或信息的用户。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: e795b58eaae7ecd428f1473b277cd6bc65cbf09d
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981023"
---
# <a name="microsoft-365-active-users-reports"></a><span data-ttu-id="75ca2-104">Microsoft 365 活动用户报告</span><span class="sxs-lookup"><span data-stu-id="75ca2-104">Microsoft 365 active users reports</span></span>

<span data-ttu-id="75ca2-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75ca2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="75ca2-106">可以使用 Microsoft 365 活动用户报告来了解组织中个人使用的产品许可证数量，并深入了解哪些用户正在使用哪些产品。</span><span class="sxs-lookup"><span data-stu-id="75ca2-106">You can use the Microsoft 365 active users reports to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="75ca2-107">此类报表有助于管理员发现未充分利用的产品或可能需要获取额外培训或信息的用户。</span><span class="sxs-lookup"><span data-stu-id="75ca2-107">These reports can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="75ca2-108">**备注：** 若要了解不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - 活动用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="75ca2-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="75ca2-109">报告</span><span class="sxs-lookup"><span data-stu-id="75ca2-109">Reports</span></span>
| <span data-ttu-id="75ca2-110">函数</span><span class="sxs-lookup"><span data-stu-id="75ca2-110">Function</span></span>                                 | <span data-ttu-id="75ca2-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="75ca2-111">Return Type</span></span> | <span data-ttu-id="75ca2-112">说明</span><span class="sxs-lookup"><span data-stu-id="75ca2-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="75ca2-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="75ca2-113">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="75ca2-114">Stream</span><span class="sxs-lookup"><span data-stu-id="75ca2-114">Stream</span></span>      | <span data-ttu-id="75ca2-115">获取有关 Microsoft 365 活动用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="75ca2-115">Get details about Microsoft 365 active users.</span></span> |
| [<span data-ttu-id="75ca2-116">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="75ca2-116">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="75ca2-117">Stream</span><span class="sxs-lookup"><span data-stu-id="75ca2-117">Stream</span></span>      | <span data-ttu-id="75ca2-118">按产品获取报表周期内的每日活跃用户数。</span><span class="sxs-lookup"><span data-stu-id="75ca2-118">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="75ca2-119">获取服务用户数</span><span class="sxs-lookup"><span data-stu-id="75ca2-119">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="75ca2-120">Stream</span><span class="sxs-lookup"><span data-stu-id="75ca2-120">Stream</span></span>      | <span data-ttu-id="75ca2-121">按活动类型和服务获取用户数。</span><span class="sxs-lookup"><span data-stu-id="75ca2-121">Get the count of users by activity type and service.</span></span> |

