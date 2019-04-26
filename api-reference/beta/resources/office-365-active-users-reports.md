---
title: Office 365 活跃用户报表
description: 您可以使用 Office 365 活动用户报告来确定组织中的个人使用了多少产品许可证, 并向下钻取有关哪些用户正在使用哪些产品的信息。 此报表可帮助管理员确定未被充分利用的产品或是可能需要其他培训或信息的用户。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 638550fbc44acd0154a2dab5c062e2061fa9c582
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562611"
---
# <a name="office-365-active-users-reports"></a><span data-ttu-id="d644c-104">Office 365 活跃用户报表</span><span class="sxs-lookup"><span data-stu-id="d644c-104">Office 365 active users reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d644c-105">您可以使用 Office 365 活动用户报告来确定组织中的个人使用了多少产品许可证, 并向下钻取有关哪些用户正在使用哪些产品的信息。</span><span class="sxs-lookup"><span data-stu-id="d644c-105">You can use the Office 365 active users report to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="d644c-106">此报表可帮助管理员确定未被充分利用的产品或是可能需要其他培训或信息的用户。</span><span class="sxs-lookup"><span data-stu-id="d644c-106">This report can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="d644c-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="d644c-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="d644c-108">报表</span><span class="sxs-lookup"><span data-stu-id="d644c-108">Reports</span></span>
| <span data-ttu-id="d644c-109">函数</span><span class="sxs-lookup"><span data-stu-id="d644c-109">Function</span></span>                                 | <span data-ttu-id="d644c-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="d644c-110">CSV return type</span></span> | <span data-ttu-id="d644c-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="d644c-111">JSON return type</span></span>                         | <span data-ttu-id="d644c-112">说明</span><span class="sxs-lookup"><span data-stu-id="d644c-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="d644c-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="d644c-113">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="d644c-114">Stream</span><span class="sxs-lookup"><span data-stu-id="d644c-114">Stream</span></span>          | [<span data-ttu-id="d644c-115">office365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="d644c-115">office365ActiveUserDetail</span></span>](../resources/office365activeuserdetail.md) | <span data-ttu-id="d644c-116">获取 Office 365 活跃用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d644c-116">Get details about Office 365 active users.</span></span> |
| [<span data-ttu-id="d644c-117">获取用户数</span><span class="sxs-lookup"><span data-stu-id="d644c-117">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="d644c-118">Stream</span><span class="sxs-lookup"><span data-stu-id="d644c-118">Stream</span></span>          | [<span data-ttu-id="d644c-119">office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="d644c-119">office365ActiveUserCounts</span></span>](../resources/office365activeusercounts.md) | <span data-ttu-id="d644c-120">按产品获取报表周期内的每日活跃用户数。</span><span class="sxs-lookup"><span data-stu-id="d644c-120">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="d644c-121">获取服务用户数</span><span class="sxs-lookup"><span data-stu-id="d644c-121">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="d644c-122">Stream</span><span class="sxs-lookup"><span data-stu-id="d644c-122">Stream</span></span>          | [<span data-ttu-id="d644c-123">office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="d644c-123">office365ServicesUserCounts</span></span>](../resources/office365servicesusercounts.md) | <span data-ttu-id="d644c-124">按活动类型和服务获取用户数。</span><span class="sxs-lookup"><span data-stu-id="d644c-124">Get the count of users by activity type and service.</span></span> |
