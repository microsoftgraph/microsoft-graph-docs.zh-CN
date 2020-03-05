---
title: educationSynchronizationProfileStatus 资源类型
description: '表示学校数据同步配置文件的同步状态。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 88e2f85cc4b24bd55cdfc1fbc5aeecd7bee8c461
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500028"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="7098f-103">educationSynchronizationProfileStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="7098f-103">educationSynchronizationProfileStatus resource type</span></span>

<span data-ttu-id="7098f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7098f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7098f-105">表示学校数据[同步配置文件](educationsynchronizationprofile.md)的同步状态。</span><span class="sxs-lookup"><span data-stu-id="7098f-105">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="7098f-106">**注意：** 由于后台同步处理的异步特性，对**educationSynchronizationProfileStatus**的更新可能会延迟。</span><span class="sxs-lookup"><span data-stu-id="7098f-106">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="7098f-107">方法</span><span class="sxs-lookup"><span data-stu-id="7098f-107">Methods</span></span>

| <span data-ttu-id="7098f-108">方法</span><span class="sxs-lookup"><span data-stu-id="7098f-108">Method</span></span> | <span data-ttu-id="7098f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="7098f-109">Return Type</span></span> | <span data-ttu-id="7098f-110">说明</span><span class="sxs-lookup"><span data-stu-id="7098f-110">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="7098f-111">获取同步状态</span><span class="sxs-lookup"><span data-stu-id="7098f-111">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="7098f-112">**educationSynchronizationProfileStatus**</span><span class="sxs-lookup"><span data-stu-id="7098f-112">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="7098f-113">返回特定同步配置文件的状态。</span><span class="sxs-lookup"><span data-stu-id="7098f-113">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="7098f-114">属性</span><span class="sxs-lookup"><span data-stu-id="7098f-114">Properties</span></span>

| <span data-ttu-id="7098f-115">属性</span><span class="sxs-lookup"><span data-stu-id="7098f-115">Property</span></span> | <span data-ttu-id="7098f-116">类型</span><span class="sxs-lookup"><span data-stu-id="7098f-116">Type</span></span> | <span data-ttu-id="7098f-117">说明</span><span class="sxs-lookup"><span data-stu-id="7098f-117">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="7098f-118">**status**</span><span class="sxs-lookup"><span data-stu-id="7098f-118">**status**</span></span> | <span data-ttu-id="7098f-119">educationSynchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="7098f-119">educationSynchronizationStatus</span></span> | <span data-ttu-id="7098f-120">同步的状态。可能的值为`paused`： `inProgress`、 `success`、 `error`、 `quarantined`、 `validationError`、。</span><span class="sxs-lookup"><span data-stu-id="7098f-120">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="7098f-121">**lastSynchronizationDateTime**</span><span class="sxs-lookup"><span data-stu-id="7098f-121">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="7098f-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7098f-122">DateTimeOffset</span></span> | <span data-ttu-id="7098f-123">表示在目录中观察到的最新更改的时间。</span><span class="sxs-lookup"><span data-stu-id="7098f-123">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="7098f-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7098f-124">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/profileStatus/$entity",
    "status": {"@odata.type":"microsoft.graph.educationSynchronizationStatus"},
    "lastSynchronizationDateTime": "DateTimeOffset"
}
```
