---
title: educationSynchronizationError 资源类型
description: 表示学校数据配置文件验证和/或同步过程中出现的错误。对于无法验证和/或与 Azure Active Directory (Azure AD) 进行同步的每个条目，都会生成一个唯一的错误。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2af4ef9f17452714373d42b67af6e87a7f87fe1d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989645"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="eaf9a-103">educationSynchronizationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="eaf9a-103">educationSynchronizationError resource type</span></span>

<span data-ttu-id="eaf9a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eaf9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eaf9a-105">表示学校数据配置文件验证和/或同步过程中出现的错误。对于无法验证和/或与 Azure Active Directory (Azure AD) 进行同步的每个条目，都会生成一个唯一的错误。</span><span class="sxs-lookup"><span data-stu-id="eaf9a-105">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="eaf9a-106">方法</span><span class="sxs-lookup"><span data-stu-id="eaf9a-106">Methods</span></span>

| <span data-ttu-id="eaf9a-107">方法</span><span class="sxs-lookup"><span data-stu-id="eaf9a-107">Method</span></span>                                                                     | <span data-ttu-id="eaf9a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="eaf9a-108">Return Type</span></span>                                  | <span data-ttu-id="eaf9a-109">说明</span><span class="sxs-lookup"><span data-stu-id="eaf9a-109">Description</span></span>                                                           |
| :------------------------------------------------------------------------- | :------------------------------------------- | :-------------------------------------------------------------------- |
| [<span data-ttu-id="eaf9a-110">获取同步错误</span><span class="sxs-lookup"><span data-stu-id="eaf9a-110">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="eaf9a-111">**educationSynchronizationError** 集合</span><span class="sxs-lookup"><span data-stu-id="eaf9a-111">**educationSynchronizationError** collection</span></span> | <span data-ttu-id="eaf9a-112">返回与配置文件关联的同步错误的列表。</span><span class="sxs-lookup"><span data-stu-id="eaf9a-112">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="eaf9a-113">属性</span><span class="sxs-lookup"><span data-stu-id="eaf9a-113">Properties</span></span>

| <span data-ttu-id="eaf9a-114">属性</span><span class="sxs-lookup"><span data-stu-id="eaf9a-114">Property</span></span>             | <span data-ttu-id="eaf9a-115">类型</span><span class="sxs-lookup"><span data-stu-id="eaf9a-115">Type</span></span>           | <span data-ttu-id="eaf9a-116">说明</span><span class="sxs-lookup"><span data-stu-id="eaf9a-116">Description</span></span>                                                     |
| :------------------- | :------------- | :-------------------------------------------------------------- |
| <span data-ttu-id="eaf9a-117">id</span><span class="sxs-lookup"><span data-stu-id="eaf9a-117">id</span></span>                   | <span data-ttu-id="eaf9a-118">String</span><span class="sxs-lookup"><span data-stu-id="eaf9a-118">String</span></span>         | <span data-ttu-id="eaf9a-119">资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="eaf9a-119">The unique identifier for the resource.</span></span> <span data-ttu-id="eaf9a-120"> (只读) </span><span class="sxs-lookup"><span data-stu-id="eaf9a-120">(read-only)</span></span>             |
| <span data-ttu-id="eaf9a-121">entryType</span><span class="sxs-lookup"><span data-stu-id="eaf9a-121">entryType</span></span>            | <span data-ttu-id="eaf9a-122">String</span><span class="sxs-lookup"><span data-stu-id="eaf9a-122">String</span></span>         | <span data-ttu-id="eaf9a-123">表示 (学校、section、student、教师) 的同步实体。</span><span class="sxs-lookup"><span data-stu-id="eaf9a-123">Represents the sync entity (school, section, student, teacher).</span></span> |
| <span data-ttu-id="eaf9a-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="eaf9a-124">errorCode</span></span>            | <span data-ttu-id="eaf9a-125">String</span><span class="sxs-lookup"><span data-stu-id="eaf9a-125">String</span></span>         | <span data-ttu-id="eaf9a-126">表示此错误的错误代码。</span><span class="sxs-lookup"><span data-stu-id="eaf9a-126">Represents the error code for this error.</span></span>                       |
| <span data-ttu-id="eaf9a-127">errorMessage</span><span class="sxs-lookup"><span data-stu-id="eaf9a-127">errorMessage</span></span>         | <span data-ttu-id="eaf9a-128">String</span><span class="sxs-lookup"><span data-stu-id="eaf9a-128">String</span></span>         | <span data-ttu-id="eaf9a-129">包含错误的说明。</span><span class="sxs-lookup"><span data-stu-id="eaf9a-129">Contains a description of the error.</span></span>                            |
| <span data-ttu-id="eaf9a-130">joiningValue</span><span class="sxs-lookup"><span data-stu-id="eaf9a-130">joiningValue</span></span>         | <span data-ttu-id="eaf9a-131">String</span><span class="sxs-lookup"><span data-stu-id="eaf9a-131">String</span></span>         | <span data-ttu-id="eaf9a-132">条目的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="eaf9a-132">The unique identifier for the entry.</span></span>                            |
| <span data-ttu-id="eaf9a-133">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="eaf9a-133">recordedDateTime</span></span>     | <span data-ttu-id="eaf9a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eaf9a-134">DateTimeOffset</span></span> | <span data-ttu-id="eaf9a-135">出现此错误的时间。</span><span class="sxs-lookup"><span data-stu-id="eaf9a-135">The time of occurrence of this error.</span></span>                           |
| <span data-ttu-id="eaf9a-136">reportableIdentifier</span><span class="sxs-lookup"><span data-stu-id="eaf9a-136">reportableIdentifier</span></span> | <span data-ttu-id="eaf9a-137">String</span><span class="sxs-lookup"><span data-stu-id="eaf9a-137">String</span></span>         | <span data-ttu-id="eaf9a-138">此错误项的标识符。</span><span class="sxs-lookup"><span data-stu-id="eaf9a-138">The identifier of this error entry.</span></span>                             |

## <a name="json-representation"></a><span data-ttu-id="eaf9a-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eaf9a-139">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationError"
}-->

```json
{
  "id": "String",
  "entryType": "String",
  "errorCode": "String",
  "errorMessage": "String",
  "joiningValue": "String",
  "recordedDateTime": "DateTimeOffset",
  "reportableIdentifier": "String"
}
```


