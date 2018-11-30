---
title: OneDrive 活动报表
description: OneDrive 活动报表可用于获取每个有权使用 OneDrive 的用户的活动，具体是以用户与 OneDrive 文件的交互为依据。 此类报表也有助于了解以共享文件数为依据的协作级别。
ms.openlocfilehash: 8568ccb0b77c8eb5f33bc44a72d9ccc5ae8dda0e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010749"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="cef92-104">OneDrive 活动报表</span><span class="sxs-lookup"><span data-stu-id="cef92-104">OneDrive activity reports</span></span>

<span data-ttu-id="cef92-105">OneDrive 活动报表可用于获取每个有权使用 OneDrive 的用户的活动，具体是以用户与 OneDrive 文件的交互为依据。</span><span class="sxs-lookup"><span data-stu-id="cef92-105">Use the OneDrive activity reports to get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="cef92-106">此类报表也有助于了解以共享文件数为依据的协作级别。</span><span class="sxs-lookup"><span data-stu-id="cef92-106">These reports can help you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="cef92-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 活动](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)。</span><span class="sxs-lookup"><span data-stu-id="cef92-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="cef92-108">报表</span><span class="sxs-lookup"><span data-stu-id="cef92-108">Reports</span></span>

| <span data-ttu-id="cef92-109">函数</span><span class="sxs-lookup"><span data-stu-id="cef92-109">Function</span></span>                                 | <span data-ttu-id="cef92-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="cef92-110">Return Type</span></span> | <span data-ttu-id="cef92-111">说明</span><span class="sxs-lookup"><span data-stu-id="cef92-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="cef92-112">获取用户详细信息</span><span class="sxs-lookup"><span data-stu-id="cef92-112">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="cef92-113">Stream</span><span class="sxs-lookup"><span data-stu-id="cef92-113">Stream</span></span>      | <span data-ttu-id="cef92-114">获取用户执行的 OneDrive 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="cef92-114">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="cef92-115">获取用户数</span><span class="sxs-lookup"><span data-stu-id="cef92-115">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="cef92-116">Stream</span><span class="sxs-lookup"><span data-stu-id="cef92-116">Stream</span></span>      | <span data-ttu-id="cef92-117">获取 OneDrive 活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="cef92-117">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="cef92-118">获取文件数</span><span class="sxs-lookup"><span data-stu-id="cef92-118">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="cef92-119">Stream</span><span class="sxs-lookup"><span data-stu-id="cef92-119">Stream</span></span>      | <span data-ttu-id="cef92-120">获取对任意 OneDrive 帐户执行文件交互的唯一许可用户数。</span><span class="sxs-lookup"><span data-stu-id="cef92-120">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |

