---
title: educationSynchronizationError 资源类型
description: 表示学校数据配置文件验证和/或同步过程中出现的错误。对于无法验证和/或与 Azure Active Directory （Azure AD）同步的每个条目，都会生成一个唯一的错误。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d46d1160ae59174d9fcb4df89559531e3a032e55
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500322"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="7a1e4-103">educationSynchronizationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="7a1e4-103">educationSynchronizationError resource type</span></span>

<span data-ttu-id="7a1e4-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7a1e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a1e4-105">表示学校数据配置文件验证和/或同步过程中出现的错误。对于无法验证和/或与 Azure Active Directory （Azure AD）同步的每个条目，都会生成一个唯一的错误。</span><span class="sxs-lookup"><span data-stu-id="7a1e4-105">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="7a1e4-106">方法</span><span class="sxs-lookup"><span data-stu-id="7a1e4-106">Methods</span></span>

| <span data-ttu-id="7a1e4-107">方法</span><span class="sxs-lookup"><span data-stu-id="7a1e4-107">Method</span></span> | <span data-ttu-id="7a1e4-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="7a1e4-108">Return Type</span></span> | <span data-ttu-id="7a1e4-109">说明</span><span class="sxs-lookup"><span data-stu-id="7a1e4-109">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="7a1e4-110">获取同步错误</span><span class="sxs-lookup"><span data-stu-id="7a1e4-110">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="7a1e4-111">**educationSynchronizationError**集合</span><span class="sxs-lookup"><span data-stu-id="7a1e4-111">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="7a1e4-112">返回与配置文件关联的同步错误的列表。</span><span class="sxs-lookup"><span data-stu-id="7a1e4-112">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="7a1e4-113">属性</span><span class="sxs-lookup"><span data-stu-id="7a1e4-113">Properties</span></span>

| <span data-ttu-id="7a1e4-114">属性</span><span class="sxs-lookup"><span data-stu-id="7a1e4-114">Property</span></span> | <span data-ttu-id="7a1e4-115">类型</span><span class="sxs-lookup"><span data-stu-id="7a1e4-115">Type</span></span> | <span data-ttu-id="7a1e4-116">说明</span><span class="sxs-lookup"><span data-stu-id="7a1e4-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="7a1e4-117">**entryType**</span><span class="sxs-lookup"><span data-stu-id="7a1e4-117">**entryType**</span></span> | <span data-ttu-id="7a1e4-118">string</span><span class="sxs-lookup"><span data-stu-id="7a1e4-118">string</span></span> |  <span data-ttu-id="7a1e4-119">表示 sync 实体（学校、节、学生、教师）。</span><span class="sxs-lookup"><span data-stu-id="7a1e4-119">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="7a1e4-120">**errorCode**</span><span class="sxs-lookup"><span data-stu-id="7a1e4-120">**errorCode**</span></span> | <span data-ttu-id="7a1e4-121">string</span><span class="sxs-lookup"><span data-stu-id="7a1e4-121">string</span></span> |  <span data-ttu-id="7a1e4-122">表示此错误的错误代码。</span><span class="sxs-lookup"><span data-stu-id="7a1e4-122">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="7a1e4-123">**errorMessage**</span><span class="sxs-lookup"><span data-stu-id="7a1e4-123">**errorMessage**</span></span> | <span data-ttu-id="7a1e4-124">string</span><span class="sxs-lookup"><span data-stu-id="7a1e4-124">string</span></span> |  <span data-ttu-id="7a1e4-125">包含错误的说明。</span><span class="sxs-lookup"><span data-stu-id="7a1e4-125">Contains a description of the error.</span></span>        |
| <span data-ttu-id="7a1e4-126">**joiningValue**</span><span class="sxs-lookup"><span data-stu-id="7a1e4-126">**joiningValue**</span></span> | <span data-ttu-id="7a1e4-127">string</span><span class="sxs-lookup"><span data-stu-id="7a1e4-127">string</span></span> |  <span data-ttu-id="7a1e4-128">条目的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7a1e4-128">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="7a1e4-129">**recordedDateTime**</span><span class="sxs-lookup"><span data-stu-id="7a1e4-129">**recordedDateTime**</span></span> | <span data-ttu-id="7a1e4-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a1e4-130">DateTimeOffset</span></span> | <span data-ttu-id="7a1e4-131">出现此错误的时间。</span><span class="sxs-lookup"><span data-stu-id="7a1e4-131">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="7a1e4-132">**reportableIdentifier**</span><span class="sxs-lookup"><span data-stu-id="7a1e4-132">**reportableIdentifier**</span></span> | <span data-ttu-id="7a1e4-133">string</span><span class="sxs-lookup"><span data-stu-id="7a1e4-133">string</span></span> | <span data-ttu-id="7a1e4-134">此错误项的标识符。</span><span class="sxs-lookup"><span data-stu-id="7a1e4-134">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="7a1e4-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a1e4-135">JSON representation</span></span>
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
