---
title: educationSynchronizationError 资源类型
description: 表示学校数据配置文件验证和/或同步过程中出现的错误。对于无法验证和/或与 azure Active Directory (azure AD) 同步的每个条目, 都会生成一个唯一的错误。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3c512f921e77468bb30e5109eec29afa9b395b7e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340518"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="2a33e-103">educationSynchronizationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a33e-103">educationSynchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a33e-104">表示学校数据配置文件验证和/或同步过程中出现的错误。对于无法验证和/或与 azure Active Directory (azure AD) 同步的每个条目, 都会生成一个唯一的错误。</span><span class="sxs-lookup"><span data-stu-id="2a33e-104">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="2a33e-105">方法</span><span class="sxs-lookup"><span data-stu-id="2a33e-105">Methods</span></span>

| <span data-ttu-id="2a33e-106">方法</span><span class="sxs-lookup"><span data-stu-id="2a33e-106">Method</span></span> | <span data-ttu-id="2a33e-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="2a33e-107">Return Type</span></span> | <span data-ttu-id="2a33e-108">说明</span><span class="sxs-lookup"><span data-stu-id="2a33e-108">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="2a33e-109">获取同步错误</span><span class="sxs-lookup"><span data-stu-id="2a33e-109">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="2a33e-110">**educationSynchronizationError**集合</span><span class="sxs-lookup"><span data-stu-id="2a33e-110">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="2a33e-111">返回与配置文件关联的同步错误的列表。</span><span class="sxs-lookup"><span data-stu-id="2a33e-111">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="2a33e-112">属性</span><span class="sxs-lookup"><span data-stu-id="2a33e-112">Properties</span></span>

| <span data-ttu-id="2a33e-113">属性</span><span class="sxs-lookup"><span data-stu-id="2a33e-113">Property</span></span> | <span data-ttu-id="2a33e-114">类型</span><span class="sxs-lookup"><span data-stu-id="2a33e-114">Type</span></span> | <span data-ttu-id="2a33e-115">说明</span><span class="sxs-lookup"><span data-stu-id="2a33e-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="2a33e-116">**entryType**</span><span class="sxs-lookup"><span data-stu-id="2a33e-116">**entryType**</span></span> | <span data-ttu-id="2a33e-117">string</span><span class="sxs-lookup"><span data-stu-id="2a33e-117">string</span></span> |  <span data-ttu-id="2a33e-118">表示 sync 实体 (学校、节、学生、教师)。</span><span class="sxs-lookup"><span data-stu-id="2a33e-118">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="2a33e-119">**错误**</span><span class="sxs-lookup"><span data-stu-id="2a33e-119">**errorCode**</span></span> | <span data-ttu-id="2a33e-120">string</span><span class="sxs-lookup"><span data-stu-id="2a33e-120">string</span></span> |  <span data-ttu-id="2a33e-121">表示此错误的错误代码。</span><span class="sxs-lookup"><span data-stu-id="2a33e-121">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="2a33e-122">**errorMessage**</span><span class="sxs-lookup"><span data-stu-id="2a33e-122">**errorMessage**</span></span> | <span data-ttu-id="2a33e-123">string</span><span class="sxs-lookup"><span data-stu-id="2a33e-123">string</span></span> |  <span data-ttu-id="2a33e-124">包含错误的说明。</span><span class="sxs-lookup"><span data-stu-id="2a33e-124">Contains a description of the error.</span></span>        |
| <span data-ttu-id="2a33e-125">**joiningValue**</span><span class="sxs-lookup"><span data-stu-id="2a33e-125">**joiningValue**</span></span> | <span data-ttu-id="2a33e-126">string</span><span class="sxs-lookup"><span data-stu-id="2a33e-126">string</span></span> |  <span data-ttu-id="2a33e-127">条目的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2a33e-127">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="2a33e-128">**recordedDateTime**</span><span class="sxs-lookup"><span data-stu-id="2a33e-128">**recordedDateTime**</span></span> | <span data-ttu-id="2a33e-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a33e-129">DateTimeOffset</span></span> | <span data-ttu-id="2a33e-130">出现此错误的时间。</span><span class="sxs-lookup"><span data-stu-id="2a33e-130">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="2a33e-131">**reportableIdentifier**</span><span class="sxs-lookup"><span data-stu-id="2a33e-131">**reportableIdentifier**</span></span> | <span data-ttu-id="2a33e-132">string</span><span class="sxs-lookup"><span data-stu-id="2a33e-132">string</span></span> | <span data-ttu-id="2a33e-133">此错误项的标识符。</span><span class="sxs-lookup"><span data-stu-id="2a33e-133">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="2a33e-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a33e-134">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationError"
}-->

```json
{
    "entryType": "String",
    "errorCode": "String",
    "errorMessage": "String",
    "joiningValue": "String",
    "recordedDateTime": "DateTimeOffset",
    "reportableIdentifier": "String"
}
```
