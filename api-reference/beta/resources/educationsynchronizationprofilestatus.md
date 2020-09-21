---
title: educationSynchronizationProfileStatus 资源类型
description: '表示学校数据同步配置文件的同步状态。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0e792b55cddaee3069eaaf53cc9dce68aae041e9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979544"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="a3f19-103">educationSynchronizationProfileStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="a3f19-103">educationSynchronizationProfileStatus resource type</span></span>

<span data-ttu-id="a3f19-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3f19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3f19-105">表示学校数据 [同步配置文件](educationsynchronizationprofile.md)的同步状态。</span><span class="sxs-lookup"><span data-stu-id="a3f19-105">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span>

> <span data-ttu-id="a3f19-106">**注意：** 由于后台同步处理的异步特性，对 **educationSynchronizationProfileStatus** 的更新可能会延迟。</span><span class="sxs-lookup"><span data-stu-id="a3f19-106">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="a3f19-107">方法</span><span class="sxs-lookup"><span data-stu-id="a3f19-107">Methods</span></span>

| <span data-ttu-id="a3f19-108">方法</span><span class="sxs-lookup"><span data-stu-id="a3f19-108">Method</span></span>                                                                      | <span data-ttu-id="a3f19-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a3f19-109">Return Type</span></span>                               | <span data-ttu-id="a3f19-110">说明</span><span class="sxs-lookup"><span data-stu-id="a3f19-110">Description</span></span>                                              |
| :-------------------------------------------------------------------------- | :---------------------------------------- | :------------------------------------------------------- |
| [<span data-ttu-id="a3f19-111">获取同步状态</span><span class="sxs-lookup"><span data-stu-id="a3f19-111">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="a3f19-112">**educationSynchronizationProfileStatus**</span><span class="sxs-lookup"><span data-stu-id="a3f19-112">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="a3f19-113">返回特定同步配置文件的状态。</span><span class="sxs-lookup"><span data-stu-id="a3f19-113">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="a3f19-114">属性</span><span class="sxs-lookup"><span data-stu-id="a3f19-114">Properties</span></span>

| <span data-ttu-id="a3f19-115">属性</span><span class="sxs-lookup"><span data-stu-id="a3f19-115">Property</span></span>                    | <span data-ttu-id="a3f19-116">类型</span><span class="sxs-lookup"><span data-stu-id="a3f19-116">Type</span></span>                           | <span data-ttu-id="a3f19-117">说明</span><span class="sxs-lookup"><span data-stu-id="a3f19-117">Description</span></span>                                                                                                              |
| :-------------------------- | :----------------------------- | :----------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="a3f19-118">id</span><span class="sxs-lookup"><span data-stu-id="a3f19-118">id</span></span>                          | <span data-ttu-id="a3f19-119">String</span><span class="sxs-lookup"><span data-stu-id="a3f19-119">String</span></span>                         | <span data-ttu-id="a3f19-120">资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a3f19-120">The unique identifier for the resource.</span></span> <span data-ttu-id="a3f19-121"> (只读) </span><span class="sxs-lookup"><span data-stu-id="a3f19-121">(read-only)</span></span>                                                                      |
| <span data-ttu-id="a3f19-122">状态</span><span class="sxs-lookup"><span data-stu-id="a3f19-122">status</span></span>                      | <span data-ttu-id="a3f19-123">educationSynchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="a3f19-123">educationSynchronizationStatus</span></span> | <span data-ttu-id="a3f19-124">同步的状态。可能的值为： `paused` 、、、、 `inProgress` `success` `error` `quarantined` 、 `validationError` 。</span><span class="sxs-lookup"><span data-stu-id="a3f19-124">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="a3f19-125">lastSynchronizationDateTime</span><span class="sxs-lookup"><span data-stu-id="a3f19-125">lastSynchronizationDateTime</span></span> | <span data-ttu-id="a3f19-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3f19-126">DateTimeOffset</span></span>                 | <span data-ttu-id="a3f19-127">表示在目录中观察到的最新更改的时间。</span><span class="sxs-lookup"><span data-stu-id="a3f19-127">Represents the time when most recent changes have been observed in the directory.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="a3f19-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3f19-128">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/profileStatus/$entity",
  "id": "String",
  "status": { "@odata.type": "microsoft.graph.educationSynchronizationStatus" },
  "lastSynchronizationDateTime": "DateTimeOffset"
}
```


