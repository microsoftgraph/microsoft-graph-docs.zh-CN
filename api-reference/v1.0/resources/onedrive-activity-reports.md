---
title: OneDrive 活动报表
description: OneDrive 活动报表可用于获取每个有权使用 OneDrive 的用户的活动，具体是以用户与 OneDrive 文件的交互为依据。 此类报表也有助于了解以共享文件数为依据的协作级别。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 24a2e74e9e117c13fa49efc6fba4323f75716ffe
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898147"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="b1608-104">OneDrive 活动报表</span><span class="sxs-lookup"><span data-stu-id="b1608-104">OneDrive activity reports</span></span>

<span data-ttu-id="b1608-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1608-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b1608-106">OneDrive 活动报表可用于获取每个有权使用 OneDrive 的用户的活动，具体是以用户与 OneDrive 文件的交互为依据。</span><span class="sxs-lookup"><span data-stu-id="b1608-106">Use the OneDrive activity reports to get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="b1608-107">此类报表也有助于了解以共享文件数为依据的协作级别。</span><span class="sxs-lookup"><span data-stu-id="b1608-107">These reports can help you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="b1608-108">**注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 reports-OneDrive For business 活动](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)。</span><span class="sxs-lookup"><span data-stu-id="b1608-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="b1608-109">报表</span><span class="sxs-lookup"><span data-stu-id="b1608-109">Reports</span></span>

| <span data-ttu-id="b1608-110">函数</span><span class="sxs-lookup"><span data-stu-id="b1608-110">Function</span></span>                                 | <span data-ttu-id="b1608-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="b1608-111">Return Type</span></span> | <span data-ttu-id="b1608-112">说明</span><span class="sxs-lookup"><span data-stu-id="b1608-112">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="b1608-113">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="b1608-113">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="b1608-114">Stream</span><span class="sxs-lookup"><span data-stu-id="b1608-114">Stream</span></span>      | <span data-ttu-id="b1608-115">获取用户执行的 OneDrive 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b1608-115">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="b1608-116">获取用户数</span><span class="sxs-lookup"><span data-stu-id="b1608-116">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="b1608-117">Stream</span><span class="sxs-lookup"><span data-stu-id="b1608-117">Stream</span></span>      | <span data-ttu-id="b1608-118">获取 OneDrive 活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="b1608-118">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="b1608-119">获取文件数</span><span class="sxs-lookup"><span data-stu-id="b1608-119">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="b1608-120">Stream</span><span class="sxs-lookup"><span data-stu-id="b1608-120">Stream</span></span>      | <span data-ttu-id="b1608-121">获取对任意 OneDrive 帐户执行文件交互的唯一许可用户数。</span><span class="sxs-lookup"><span data-stu-id="b1608-121">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |

