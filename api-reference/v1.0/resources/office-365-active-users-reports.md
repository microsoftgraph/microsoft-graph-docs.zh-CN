---
title: Microsoft 365 活动用户报告
description: 您可以使用 Microsoft 365 活动用户报告来确定组织中的个人使用了多少产品许可证，并向下钻取有关哪些用户正在使用哪些产品的信息。 此类报表有助于管理员发现未充分利用的产品或可能需要获取额外培训或信息的用户。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 041bbe180df2225383d704002d06359334fb8d84
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898161"
---
# <a name="microsoft-365-active-users-reports"></a><span data-ttu-id="0f386-104">Microsoft 365 活动用户报告</span><span class="sxs-lookup"><span data-stu-id="0f386-104">Microsoft 365 active users reports</span></span>

<span data-ttu-id="0f386-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f386-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f386-106">您可以使用 Microsoft 365 活动用户报告来确定组织中的个人使用了多少产品许可证，并向下钻取有关哪些用户正在使用哪些产品的信息。</span><span class="sxs-lookup"><span data-stu-id="0f386-106">You can use the Microsoft 365 active users reports to find out how many product licenses are being used by individuals in your organization, and drill down for information about which users are using what products.</span></span> <span data-ttu-id="0f386-107">此类报表有助于管理员发现未充分利用的产品或可能需要获取额外培训或信息的用户。</span><span class="sxs-lookup"><span data-stu-id="0f386-107">These reports can help administrators identify underutilized products or users that might need additional training or information.</span></span>

> <span data-ttu-id="0f386-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 报表-活动用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="0f386-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="reports"></a><span data-ttu-id="0f386-109">报表</span><span class="sxs-lookup"><span data-stu-id="0f386-109">Reports</span></span>
| <span data-ttu-id="0f386-110">函数</span><span class="sxs-lookup"><span data-stu-id="0f386-110">Function</span></span>                                 | <span data-ttu-id="0f386-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="0f386-111">Return Type</span></span> | <span data-ttu-id="0f386-112">说明</span><span class="sxs-lookup"><span data-stu-id="0f386-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="0f386-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="0f386-113">Get user detail</span></span>](../api/reportroot-getoffice365activeuserdetail.md) | <span data-ttu-id="0f386-114">Stream</span><span class="sxs-lookup"><span data-stu-id="0f386-114">Stream</span></span>      | <span data-ttu-id="0f386-115">获取有关 Microsoft 365 活动用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0f386-115">Get details about Microsoft 365 active users.</span></span> |
| [<span data-ttu-id="0f386-116">获取用户数</span><span class="sxs-lookup"><span data-stu-id="0f386-116">Get user counts</span></span>](../api/reportroot-getoffice365activeusercounts.md) | <span data-ttu-id="0f386-117">Stream</span><span class="sxs-lookup"><span data-stu-id="0f386-117">Stream</span></span>      | <span data-ttu-id="0f386-118">按产品获取报表周期内的每日活跃用户数。</span><span class="sxs-lookup"><span data-stu-id="0f386-118">Get the count of daily active users in the reporting period by product.</span></span> |
| [<span data-ttu-id="0f386-119">获取服务用户数</span><span class="sxs-lookup"><span data-stu-id="0f386-119">Get services user counts</span></span>](../api/reportroot-getoffice365servicesusercounts.md) | <span data-ttu-id="0f386-120">Stream</span><span class="sxs-lookup"><span data-stu-id="0f386-120">Stream</span></span>      | <span data-ttu-id="0f386-121">按活动类型和服务获取用户数。</span><span class="sxs-lookup"><span data-stu-id="0f386-121">Get the count of users by activity type and service.</span></span> |
