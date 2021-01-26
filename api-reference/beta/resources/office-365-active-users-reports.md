---
title: Microsoft 365 活动用户报告
description: 可以使用 Microsoft 365 活动用户报告了解组织中个人使用的产品许可证数量，并深入了解哪些用户使用哪些产品。 此报表可帮助管理员确定未被充分利用的产品或是可能需要其他培训或信息的用户。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: ee227bf0413944bdd648de64f32bf4f6ab9f3d70
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980768"
---
# <a name="microsoft-365-active-users-reports"></a><span data-ttu-id="0230d-104">Microsoft 365 活动用户报告</span><span class="sxs-lookup"><span data-stu-id="0230d-104">Microsoft 365 active users reports</span></span>

<span data-ttu-id="0230d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0230d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0230d-106">可以使用 Microsoft 365 活动用户报告了解组织中个人使用的产品许可证数量，并深入了解哪些用户使用哪些产品。</span><span class="sxs-lookup"><span data-stu-id="0230d-106">You can use the Microsoft 365 active users report to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="0230d-107">此报表可帮助管理员确定未被充分利用的产品或是可能需要其他培训或信息的用户。</span><span class="sxs-lookup"><span data-stu-id="0230d-107">This report can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="0230d-108">**备注：** 若要了解不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - 活动用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="0230d-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="0230d-109">报告</span><span class="sxs-lookup"><span data-stu-id="0230d-109">Reports</span></span>
| <span data-ttu-id="0230d-110">函数</span><span class="sxs-lookup"><span data-stu-id="0230d-110">Function</span></span>                                 | <span data-ttu-id="0230d-111">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="0230d-111">CSV return type</span></span> | <span data-ttu-id="0230d-112">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="0230d-112">JSON return type</span></span>                         | <span data-ttu-id="0230d-113">说明</span><span class="sxs-lookup"><span data-stu-id="0230d-113">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="0230d-114">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="0230d-114">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="0230d-115">Stream</span><span class="sxs-lookup"><span data-stu-id="0230d-115">Stream</span></span>          | [<span data-ttu-id="0230d-116">office365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="0230d-116">office365ActiveUserDetail</span></span>](../resources/office365activeuserdetail.md) | <span data-ttu-id="0230d-117">获取有关 Microsoft 365 活动用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0230d-117">Get details about Microsoft 365 active users.</span></span> |
| [<span data-ttu-id="0230d-118">获取用户计数</span><span class="sxs-lookup"><span data-stu-id="0230d-118">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="0230d-119">Stream</span><span class="sxs-lookup"><span data-stu-id="0230d-119">Stream</span></span>          | [<span data-ttu-id="0230d-120">office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="0230d-120">office365ActiveUserCounts</span></span>](../resources/office365activeusercounts.md) | <span data-ttu-id="0230d-121">按产品获取报表周期内的每日活跃用户数。</span><span class="sxs-lookup"><span data-stu-id="0230d-121">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="0230d-122">获取服务用户数</span><span class="sxs-lookup"><span data-stu-id="0230d-122">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="0230d-123">Stream</span><span class="sxs-lookup"><span data-stu-id="0230d-123">Stream</span></span>          | [<span data-ttu-id="0230d-124">office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="0230d-124">office365ServicesUserCounts</span></span>](../resources/office365servicesusercounts.md) | <span data-ttu-id="0230d-125">按活动类型和服务获取用户数。</span><span class="sxs-lookup"><span data-stu-id="0230d-125">Get the count of users by activity type and service.</span></span> |


