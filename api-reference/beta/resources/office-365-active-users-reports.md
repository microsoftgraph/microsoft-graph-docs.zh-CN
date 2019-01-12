---
title: Office 365 活跃用户报表
description: 您可以使用 Office 365 活动用户报告以找出多少个产品许可证正在使用的组织中的个人和向下钻取有关哪些用户正在使用哪些产品的信息。 此报告可帮助管理员识别未充分利用的产品或可能需要其他培训或信息的用户。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 958cf769a2b54f1d22cdc315ee250cb1e677c301
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970505"
---
# <a name="office-365-active-users-reports"></a><span data-ttu-id="c9b51-104">Office 365 活跃用户报表</span><span class="sxs-lookup"><span data-stu-id="c9b51-104">Office 365 active users reports</span></span>

> <span data-ttu-id="c9b51-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c9b51-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9b51-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c9b51-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c9b51-107">您可以使用 Office 365 活动用户报告以找出多少个产品许可证正在使用的组织中的个人和向下钻取有关哪些用户正在使用哪些产品的信息。</span><span class="sxs-lookup"><span data-stu-id="c9b51-107">You can use the Office 365 active users report to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="c9b51-108">此报告可帮助管理员识别未充分利用的产品或可能需要其他培训或信息的用户。</span><span class="sxs-lookup"><span data-stu-id="c9b51-108">This report can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="c9b51-109">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="c9b51-109">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="c9b51-110">报表</span><span class="sxs-lookup"><span data-stu-id="c9b51-110">Reports</span></span>
| <span data-ttu-id="c9b51-111">函数</span><span class="sxs-lookup"><span data-stu-id="c9b51-111">Function</span></span>                                 | <span data-ttu-id="c9b51-112">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="c9b51-112">CSV return type</span></span> | <span data-ttu-id="c9b51-113">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="c9b51-113">JSON return type</span></span>                         | <span data-ttu-id="c9b51-114">说明</span><span class="sxs-lookup"><span data-stu-id="c9b51-114">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="c9b51-115">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="c9b51-115">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="c9b51-116">Stream</span><span class="sxs-lookup"><span data-stu-id="c9b51-116">Stream</span></span>          | [<span data-ttu-id="c9b51-117">office365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="c9b51-117">office365ActiveUserDetail</span></span>](../resources/office365activeuserdetail.md) | <span data-ttu-id="c9b51-118">获取 Office 365 活跃用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c9b51-118">Get details about Office 365 active users.</span></span> |
| [<span data-ttu-id="c9b51-119">获取用户数</span><span class="sxs-lookup"><span data-stu-id="c9b51-119">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="c9b51-120">Stream</span><span class="sxs-lookup"><span data-stu-id="c9b51-120">Stream</span></span>          | [<span data-ttu-id="c9b51-121">office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="c9b51-121">office365ActiveUserCounts</span></span>](../resources/office365activeusercounts.md) | <span data-ttu-id="c9b51-122">按产品获取报表周期内的每日活跃用户数。</span><span class="sxs-lookup"><span data-stu-id="c9b51-122">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="c9b51-123">获取服务用户数</span><span class="sxs-lookup"><span data-stu-id="c9b51-123">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="c9b51-124">Stream</span><span class="sxs-lookup"><span data-stu-id="c9b51-124">Stream</span></span>          | [<span data-ttu-id="c9b51-125">office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="c9b51-125">office365ServicesUserCounts</span></span>](../resources/office365servicesusercounts.md) | <span data-ttu-id="c9b51-126">按活动类型和服务获取用户数。</span><span class="sxs-lookup"><span data-stu-id="c9b51-126">Get the count of users by activity type and service.</span></span> |
