---
title: Office 365 活跃用户报表
description: 您可以使用 Office 365 活动用户报告以找出多少个产品许可证正在使用的组织中的个人和向下钻取有关哪些用户正在使用哪些产品的信息。 此报告可帮助管理员识别未充分利用的产品或可能需要其他培训或信息的用户。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: e85924b7066dde92f0db5fd0b3f1f83dd32fd0c1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516208"
---
# <a name="office-365-active-users-reports"></a><span data-ttu-id="4af82-104">Office 365 活跃用户报表</span><span class="sxs-lookup"><span data-stu-id="4af82-104">Office 365 active users reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4af82-105">您可以使用 Office 365 活动用户报告以找出多少个产品许可证正在使用的组织中的个人和向下钻取有关哪些用户正在使用哪些产品的信息。</span><span class="sxs-lookup"><span data-stu-id="4af82-105">You can use the Office 365 active users report to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="4af82-106">此报告可帮助管理员识别未充分利用的产品或可能需要其他培训或信息的用户。</span><span class="sxs-lookup"><span data-stu-id="4af82-106">This report can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="4af82-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="4af82-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="4af82-108">报表</span><span class="sxs-lookup"><span data-stu-id="4af82-108">Reports</span></span>
| <span data-ttu-id="4af82-109">函数</span><span class="sxs-lookup"><span data-stu-id="4af82-109">Function</span></span>                                 | <span data-ttu-id="4af82-110">CSV 返回类型</span><span class="sxs-lookup"><span data-stu-id="4af82-110">CSV return type</span></span> | <span data-ttu-id="4af82-111">JSON 返回类型</span><span class="sxs-lookup"><span data-stu-id="4af82-111">JSON return type</span></span>                         | <span data-ttu-id="4af82-112">说明</span><span class="sxs-lookup"><span data-stu-id="4af82-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="4af82-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="4af82-113">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="4af82-114">Stream</span><span class="sxs-lookup"><span data-stu-id="4af82-114">Stream</span></span>          | [<span data-ttu-id="4af82-115">office365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="4af82-115">office365ActiveUserDetail</span></span>](../resources/office365activeuserdetail.md) | <span data-ttu-id="4af82-116">获取 Office 365 活跃用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4af82-116">Get details about Office 365 active users.</span></span> |
| [<span data-ttu-id="4af82-117">获取用户数</span><span class="sxs-lookup"><span data-stu-id="4af82-117">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="4af82-118">Stream</span><span class="sxs-lookup"><span data-stu-id="4af82-118">Stream</span></span>          | [<span data-ttu-id="4af82-119">office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="4af82-119">office365ActiveUserCounts</span></span>](../resources/office365activeusercounts.md) | <span data-ttu-id="4af82-120">按产品获取报表周期内的每日活跃用户数。</span><span class="sxs-lookup"><span data-stu-id="4af82-120">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="4af82-121">获取服务用户数</span><span class="sxs-lookup"><span data-stu-id="4af82-121">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="4af82-122">Stream</span><span class="sxs-lookup"><span data-stu-id="4af82-122">Stream</span></span>          | [<span data-ttu-id="4af82-123">office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="4af82-123">office365ServicesUserCounts</span></span>](../resources/office365servicesusercounts.md) | <span data-ttu-id="4af82-124">按活动类型和服务获取用户数。</span><span class="sxs-lookup"><span data-stu-id="4af82-124">Get the count of users by activity type and service.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-active-users-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
