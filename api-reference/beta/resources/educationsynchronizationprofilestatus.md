---
title: educationSynchronizationProfileStatus 资源类型
description: '代表学校数据同步配置文件的同步状态。 '
ms.openlocfilehash: 6d2c638e1f92a6c3e090cb2bf3bb55e8482bbc4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049279"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="86a27-103">educationSynchronizationProfileStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="86a27-103">educationSynchronizationProfileStatus resource type</span></span>

> <span data-ttu-id="86a27-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="86a27-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86a27-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="86a27-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="86a27-106">代表学校数据[同步配置文件](educationsynchronizationprofile.md)的同步状态。</span><span class="sxs-lookup"><span data-stu-id="86a27-106">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="86a27-107">**注意：** 更新**educationSynchronizationProfileStatus**可能由于后台同步处理的异步特性延迟。</span><span class="sxs-lookup"><span data-stu-id="86a27-107">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="86a27-108">方法</span><span class="sxs-lookup"><span data-stu-id="86a27-108">Methods</span></span>

| <span data-ttu-id="86a27-109">方法</span><span class="sxs-lookup"><span data-stu-id="86a27-109">Method</span></span> | <span data-ttu-id="86a27-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="86a27-110">Return Type</span></span> | <span data-ttu-id="86a27-111">说明</span><span class="sxs-lookup"><span data-stu-id="86a27-111">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="86a27-112">要获取同步的状态</span><span class="sxs-lookup"><span data-stu-id="86a27-112">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="86a27-113">**educationSynchronizationProfileStatus**</span><span class="sxs-lookup"><span data-stu-id="86a27-113">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="86a27-114">返回一个特定的同步配置文件的状态。</span><span class="sxs-lookup"><span data-stu-id="86a27-114">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="86a27-115">属性</span><span class="sxs-lookup"><span data-stu-id="86a27-115">Properties</span></span>

| <span data-ttu-id="86a27-116">属性</span><span class="sxs-lookup"><span data-stu-id="86a27-116">Property</span></span> | <span data-ttu-id="86a27-117">类型</span><span class="sxs-lookup"><span data-stu-id="86a27-117">Type</span></span> | <span data-ttu-id="86a27-118">说明</span><span class="sxs-lookup"><span data-stu-id="86a27-118">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="86a27-119">**status**</span><span class="sxs-lookup"><span data-stu-id="86a27-119">**status**</span></span> | <span data-ttu-id="86a27-120">string</span><span class="sxs-lookup"><span data-stu-id="86a27-120">string</span></span> | <span data-ttu-id="86a27-121">同步状态。可能的值为： `paused`， `inProgress`， `success`， `error`， `quarantined`， `validationError`。</span><span class="sxs-lookup"><span data-stu-id="86a27-121">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="86a27-122">**lastSynchronizationDateTime**</span><span class="sxs-lookup"><span data-stu-id="86a27-122">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="86a27-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86a27-123">DateTimeOffset</span></span> | <span data-ttu-id="86a27-124">表示当观察的目录中最新更改的时间。</span><span class="sxs-lookup"><span data-stu-id="86a27-124">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="86a27-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="86a27-125">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": {"@odata.type":"microsoft.graph.educationSynchronizationStatus"},
    "lastSynchronizationDateTime": "DateTimeOffset"
}
```