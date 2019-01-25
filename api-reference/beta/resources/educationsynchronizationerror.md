---
title: educationSynchronizationError 资源类型
description: 代表在学校数据配置文件的验证和/或同步过程中的错误。无法验证和/或与 Azure Active Directory (Azure AD) 将同步的每个条目生成是唯一的错误。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c937e95441132e4633b0f5e48a75b0597b8f08d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525141"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="ae4ce-103">educationSynchronizationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="ae4ce-103">educationSynchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae4ce-104">代表在学校数据配置文件的验证和/或同步过程中的错误。无法验证和/或与 Azure Active Directory (Azure AD) 将同步的每个条目生成是唯一的错误。</span><span class="sxs-lookup"><span data-stu-id="ae4ce-104">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="ae4ce-105">方法</span><span class="sxs-lookup"><span data-stu-id="ae4ce-105">Methods</span></span>

| <span data-ttu-id="ae4ce-106">方法</span><span class="sxs-lookup"><span data-stu-id="ae4ce-106">Method</span></span> | <span data-ttu-id="ae4ce-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="ae4ce-107">Return Type</span></span> | <span data-ttu-id="ae4ce-108">说明</span><span class="sxs-lookup"><span data-stu-id="ae4ce-108">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="ae4ce-109">获取同步错误</span><span class="sxs-lookup"><span data-stu-id="ae4ce-109">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="ae4ce-110">**educationSynchronizationError**集合</span><span class="sxs-lookup"><span data-stu-id="ae4ce-110">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="ae4ce-111">返回一个配置文件相关联的同步错误的列表。</span><span class="sxs-lookup"><span data-stu-id="ae4ce-111">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="ae4ce-112">属性</span><span class="sxs-lookup"><span data-stu-id="ae4ce-112">Properties</span></span>

| <span data-ttu-id="ae4ce-113">属性</span><span class="sxs-lookup"><span data-stu-id="ae4ce-113">Property</span></span> | <span data-ttu-id="ae4ce-114">类型</span><span class="sxs-lookup"><span data-stu-id="ae4ce-114">Type</span></span> | <span data-ttu-id="ae4ce-115">说明</span><span class="sxs-lookup"><span data-stu-id="ae4ce-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="ae4ce-116">**entryType**</span><span class="sxs-lookup"><span data-stu-id="ae4ce-116">**entryType**</span></span> | <span data-ttu-id="ae4ce-117">string</span><span class="sxs-lookup"><span data-stu-id="ae4ce-117">string</span></span> |  <span data-ttu-id="ae4ce-118">代表同步实体 （学校、 节、 学生、 教师）。</span><span class="sxs-lookup"><span data-stu-id="ae4ce-118">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="ae4ce-119">errorCode</span><span class="sxs-lookup"><span data-stu-id="ae4ce-119">**errorCode**</span></span> | <span data-ttu-id="ae4ce-120">string</span><span class="sxs-lookup"><span data-stu-id="ae4ce-120">string</span></span> |  <span data-ttu-id="ae4ce-121">表示此错误的错误代码。</span><span class="sxs-lookup"><span data-stu-id="ae4ce-121">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="ae4ce-122">**ErrorMessage**</span><span class="sxs-lookup"><span data-stu-id="ae4ce-122">**errorMessage**</span></span> | <span data-ttu-id="ae4ce-123">string</span><span class="sxs-lookup"><span data-stu-id="ae4ce-123">string</span></span> |  <span data-ttu-id="ae4ce-124">包含错误的说明。</span><span class="sxs-lookup"><span data-stu-id="ae4ce-124">Contains a description of the error.</span></span>        |
| <span data-ttu-id="ae4ce-125">**joiningValue**</span><span class="sxs-lookup"><span data-stu-id="ae4ce-125">**joiningValue**</span></span> | <span data-ttu-id="ae4ce-126">string</span><span class="sxs-lookup"><span data-stu-id="ae4ce-126">string</span></span> |  <span data-ttu-id="ae4ce-127">条目的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ae4ce-127">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="ae4ce-128">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae4ce-128">**recordedDateTime**</span></span> | <span data-ttu-id="ae4ce-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae4ce-129">DateTimeOffset</span></span> | <span data-ttu-id="ae4ce-130">出现此错误的时间。</span><span class="sxs-lookup"><span data-stu-id="ae4ce-130">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="ae4ce-131">**reportableIdentifier**</span><span class="sxs-lookup"><span data-stu-id="ae4ce-131">**reportableIdentifier**</span></span> | <span data-ttu-id="ae4ce-132">string</span><span class="sxs-lookup"><span data-stu-id="ae4ce-132">string</span></span> | <span data-ttu-id="ae4ce-133">此错误条目的标识符。</span><span class="sxs-lookup"><span data-stu-id="ae4ce-133">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="ae4ce-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ae4ce-134">JSON representation</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
