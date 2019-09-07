---
title: educationSynchronizationProfileStatus 资源类型
description: '表示学校数据同步配置文件的同步状态。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e3cc519f30b571d6c69dce48b74cd70da7f58e6f
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792808"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="07436-103">educationSynchronizationProfileStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="07436-103">educationSynchronizationProfileStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07436-104">表示学校数据[同步配置文件](educationsynchronizationprofile.md)的同步状态。</span><span class="sxs-lookup"><span data-stu-id="07436-104">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="07436-105">**注意：** 由于后台同步处理的异步特性，对**educationSynchronizationProfileStatus**的更新可能会延迟。</span><span class="sxs-lookup"><span data-stu-id="07436-105">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="07436-106">方法</span><span class="sxs-lookup"><span data-stu-id="07436-106">Methods</span></span>

| <span data-ttu-id="07436-107">方法</span><span class="sxs-lookup"><span data-stu-id="07436-107">Method</span></span> | <span data-ttu-id="07436-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="07436-108">Return Type</span></span> | <span data-ttu-id="07436-109">说明</span><span class="sxs-lookup"><span data-stu-id="07436-109">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="07436-110">获取同步状态</span><span class="sxs-lookup"><span data-stu-id="07436-110">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="07436-111">**educationSynchronizationProfileStatus**</span><span class="sxs-lookup"><span data-stu-id="07436-111">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="07436-112">返回特定同步配置文件的状态。</span><span class="sxs-lookup"><span data-stu-id="07436-112">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="07436-113">属性</span><span class="sxs-lookup"><span data-stu-id="07436-113">Properties</span></span>

| <span data-ttu-id="07436-114">属性</span><span class="sxs-lookup"><span data-stu-id="07436-114">Property</span></span> | <span data-ttu-id="07436-115">类型</span><span class="sxs-lookup"><span data-stu-id="07436-115">Type</span></span> | <span data-ttu-id="07436-116">说明</span><span class="sxs-lookup"><span data-stu-id="07436-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="07436-117">**status**</span><span class="sxs-lookup"><span data-stu-id="07436-117">**status**</span></span> | <span data-ttu-id="07436-118">educationSynchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="07436-118">educationSynchronizationStatus</span></span> | <span data-ttu-id="07436-119">同步的状态。可能的值为`paused`： `inProgress`、 `success`、 `error`、 `quarantined`、 `validationError`、。</span><span class="sxs-lookup"><span data-stu-id="07436-119">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="07436-120">**lastSynchronizationDateTime**</span><span class="sxs-lookup"><span data-stu-id="07436-120">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="07436-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07436-121">DateTimeOffset</span></span> | <span data-ttu-id="07436-122">表示在目录中观察到的最新更改的时间。</span><span class="sxs-lookup"><span data-stu-id="07436-122">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="07436-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07436-123">JSON representation</span></span>
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
