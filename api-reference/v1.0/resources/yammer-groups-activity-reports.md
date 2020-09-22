---
title: Yammer 组活动报表
description: Yammer 组活动报表可用于深入了解组织中的 Yammer 组活动，并了解正在创建和使用多少个 Yammer 组。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 9408029ce34a819782142d3d57b6c1720e91f8f4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47977935"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="f8054-103">Yammer 组活动报表</span><span class="sxs-lookup"><span data-stu-id="f8054-103">Yammer groups activity reports</span></span>

<span data-ttu-id="f8054-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8054-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f8054-105">Yammer 组活动报表可用于深入了解组织中的 Yammer 组活动，并了解正在创建和使用多少个 Yammer 组。</span><span class="sxs-lookup"><span data-stu-id="f8054-105">You can use the Yammer groups activity reports to gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="f8054-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Microsoft 365 报表-Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。</span><span class="sxs-lookup"><span data-stu-id="f8054-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="f8054-107">报表</span><span class="sxs-lookup"><span data-stu-id="f8054-107">Reports</span></span>

| <span data-ttu-id="f8054-108">函数</span><span class="sxs-lookup"><span data-stu-id="f8054-108">Function</span></span>                                 | <span data-ttu-id="f8054-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="f8054-109">Return Type</span></span> | <span data-ttu-id="f8054-110">说明</span><span class="sxs-lookup"><span data-stu-id="f8054-110">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="f8054-111">获取组详细信息</span><span class="sxs-lookup"><span data-stu-id="f8054-111">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="f8054-112">Stream</span><span class="sxs-lookup"><span data-stu-id="f8054-112">Stream</span></span>      | <span data-ttu-id="f8054-113">获取组执行的 Yammer 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f8054-113">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="f8054-114">获取组数</span><span class="sxs-lookup"><span data-stu-id="f8054-114">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="f8054-115">Stream</span><span class="sxs-lookup"><span data-stu-id="f8054-115">Stream</span></span>      | <span data-ttu-id="f8054-116">获取存在的总组数，以及有多少组包含组对话活动。</span><span class="sxs-lookup"><span data-stu-id="f8054-116">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="f8054-117">获取活动数</span><span class="sxs-lookup"><span data-stu-id="f8054-117">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="f8054-118">Stream</span><span class="sxs-lookup"><span data-stu-id="f8054-118">Stream</span></span>      | <span data-ttu-id="f8054-119">获取组中已发布、已阅读和已赞的 Yammer 消息数。</span><span class="sxs-lookup"><span data-stu-id="f8054-119">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |

