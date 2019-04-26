---
title: educationSynchronizationProfileStatus 资源类型
description: '表示学校数据同步配置文件的同步状态。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e54a80df832eba66dcdc5eb08b38feee6f4cd57a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340490"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="3d6fc-103">educationSynchronizationProfileStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d6fc-103">educationSynchronizationProfileStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d6fc-104">表示学校数据[同步配置文件](educationsynchronizationprofile.md)的同步状态。</span><span class="sxs-lookup"><span data-stu-id="3d6fc-104">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="3d6fc-105">**注意:** 由于后台同步处理的异步特性, 对**educationSynchronizationProfileStatus**的更新可能会延迟。</span><span class="sxs-lookup"><span data-stu-id="3d6fc-105">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="3d6fc-106">方法</span><span class="sxs-lookup"><span data-stu-id="3d6fc-106">Methods</span></span>

| <span data-ttu-id="3d6fc-107">方法</span><span class="sxs-lookup"><span data-stu-id="3d6fc-107">Method</span></span> | <span data-ttu-id="3d6fc-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3d6fc-108">Return Type</span></span> | <span data-ttu-id="3d6fc-109">说明</span><span class="sxs-lookup"><span data-stu-id="3d6fc-109">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="3d6fc-110">获取同步状态</span><span class="sxs-lookup"><span data-stu-id="3d6fc-110">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="3d6fc-111">**educationSynchronizationProfileStatus**</span><span class="sxs-lookup"><span data-stu-id="3d6fc-111">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="3d6fc-112">返回特定同步配置文件的状态。</span><span class="sxs-lookup"><span data-stu-id="3d6fc-112">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="3d6fc-113">属性</span><span class="sxs-lookup"><span data-stu-id="3d6fc-113">Properties</span></span>

| <span data-ttu-id="3d6fc-114">属性</span><span class="sxs-lookup"><span data-stu-id="3d6fc-114">Property</span></span> | <span data-ttu-id="3d6fc-115">类型</span><span class="sxs-lookup"><span data-stu-id="3d6fc-115">Type</span></span> | <span data-ttu-id="3d6fc-116">说明</span><span class="sxs-lookup"><span data-stu-id="3d6fc-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="3d6fc-117">**status**</span><span class="sxs-lookup"><span data-stu-id="3d6fc-117">**status**</span></span> | <span data-ttu-id="3d6fc-118">educationSynchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="3d6fc-118">educationSynchronizationStatus</span></span> | <span data-ttu-id="3d6fc-119">同步的状态。可能的值为`paused`: `inProgress`、 `success`、 `error`、 `quarantined`、 `validationError`、。</span><span class="sxs-lookup"><span data-stu-id="3d6fc-119">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="3d6fc-120">**lastSynchronizationDateTime**</span><span class="sxs-lookup"><span data-stu-id="3d6fc-120">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="3d6fc-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d6fc-121">DateTimeOffset</span></span> | <span data-ttu-id="3d6fc-122">表示在目录中观察到的最新更改的时间。</span><span class="sxs-lookup"><span data-stu-id="3d6fc-122">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="3d6fc-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d6fc-123">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": {"@odata.type":"microsoft.graph.educationSynchronizationStatus"},
    "lastSynchronizationDateTime": "DateTimeOffset"
}
```
