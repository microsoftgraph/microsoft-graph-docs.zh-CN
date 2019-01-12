---
title: Office 365 活跃用户报表
description: Office 365 活跃用户报表可用于确定组织中个人使用的产品许可证数，并向下钻取哪些用户使用什么产品的相关信息。 此类报表有助于管理员发现未充分利用的产品或可能需要获取额外培训或信息的用户。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 0ac5c3080469b8d918ee631edaf1473141a60dca
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917998"
---
# <a name="office-365-active-users-reports"></a><span data-ttu-id="cdd5c-104">Office 365 活跃用户报表</span><span class="sxs-lookup"><span data-stu-id="cdd5c-104">Office 365 active users reports</span></span>

<span data-ttu-id="cdd5c-105">Office 365 活跃用户报表可用于确定组织中个人使用的产品许可证数，并向下钻取哪些用户使用什么产品的相关信息。</span><span class="sxs-lookup"><span data-stu-id="cdd5c-105">You can use the Office 365 active users reports to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="cdd5c-106">此类报表有助于管理员发现未充分利用的产品或可能需要获取额外培训或信息的用户。</span><span class="sxs-lookup"><span data-stu-id="cdd5c-106">These reports can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="cdd5c-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="cdd5c-107">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="cdd5c-108">报表</span><span class="sxs-lookup"><span data-stu-id="cdd5c-108">Reports</span></span>
| <span data-ttu-id="cdd5c-109">函数</span><span class="sxs-lookup"><span data-stu-id="cdd5c-109">Function</span></span>                                 | <span data-ttu-id="cdd5c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="cdd5c-110">Return Type</span></span> | <span data-ttu-id="cdd5c-111">说明</span><span class="sxs-lookup"><span data-stu-id="cdd5c-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="cdd5c-112">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="cdd5c-112">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="cdd5c-113">Stream</span><span class="sxs-lookup"><span data-stu-id="cdd5c-113">Stream</span></span>      | <span data-ttu-id="cdd5c-114">获取 Office 365 活跃用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="cdd5c-114">Get details about Office 365 active users.</span></span> |
| [<span data-ttu-id="cdd5c-115">获取用户数</span><span class="sxs-lookup"><span data-stu-id="cdd5c-115">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="cdd5c-116">Stream</span><span class="sxs-lookup"><span data-stu-id="cdd5c-116">Stream</span></span>      | <span data-ttu-id="cdd5c-117">按产品获取报表周期内的每日活跃用户数。</span><span class="sxs-lookup"><span data-stu-id="cdd5c-117">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="cdd5c-118">获取服务用户数</span><span class="sxs-lookup"><span data-stu-id="cdd5c-118">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="cdd5c-119">Stream</span><span class="sxs-lookup"><span data-stu-id="cdd5c-119">Stream</span></span>      | <span data-ttu-id="cdd5c-120">按活动类型和服务获取用户数。</span><span class="sxs-lookup"><span data-stu-id="cdd5c-120">Get the count of users by activity type and service.</span></span> |
