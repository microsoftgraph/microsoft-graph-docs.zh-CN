---
title: educationSynchronizationError 资源类型
description: 代表在学校数据配置文件的验证和/或同步过程中的错误。无法验证和/或与 Azure Active Directory (Azure AD) 将同步的每个条目生成是唯一的错误。
author: mmast-msft
ms.openlocfilehash: d950e906a506c3cf1ee5bc5b627200dc79c1d0fb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335999"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="13cc9-103">educationSynchronizationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="13cc9-103">educationSynchronizationError resource type</span></span>

> <span data-ttu-id="13cc9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="13cc9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13cc9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="13cc9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13cc9-106">代表在学校数据配置文件的验证和/或同步过程中的错误。无法验证和/或与 Azure Active Directory (Azure AD) 将同步的每个条目生成是唯一的错误。</span><span class="sxs-lookup"><span data-stu-id="13cc9-106">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="13cc9-107">方法</span><span class="sxs-lookup"><span data-stu-id="13cc9-107">Methods</span></span>

| <span data-ttu-id="13cc9-108">方法</span><span class="sxs-lookup"><span data-stu-id="13cc9-108">Method</span></span> | <span data-ttu-id="13cc9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="13cc9-109">Return Type</span></span> | <span data-ttu-id="13cc9-110">说明</span><span class="sxs-lookup"><span data-stu-id="13cc9-110">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="13cc9-111">获取同步错误</span><span class="sxs-lookup"><span data-stu-id="13cc9-111">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="13cc9-112">**educationSynchronizationError**集合</span><span class="sxs-lookup"><span data-stu-id="13cc9-112">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="13cc9-113">返回一个配置文件相关联的同步错误的列表。</span><span class="sxs-lookup"><span data-stu-id="13cc9-113">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="13cc9-114">属性</span><span class="sxs-lookup"><span data-stu-id="13cc9-114">Properties</span></span>

| <span data-ttu-id="13cc9-115">属性</span><span class="sxs-lookup"><span data-stu-id="13cc9-115">Property</span></span> | <span data-ttu-id="13cc9-116">类型</span><span class="sxs-lookup"><span data-stu-id="13cc9-116">Type</span></span> | <span data-ttu-id="13cc9-117">说明</span><span class="sxs-lookup"><span data-stu-id="13cc9-117">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="13cc9-118">**entryType**</span><span class="sxs-lookup"><span data-stu-id="13cc9-118">**entryType**</span></span> | <span data-ttu-id="13cc9-119">string</span><span class="sxs-lookup"><span data-stu-id="13cc9-119">string</span></span> |  <span data-ttu-id="13cc9-120">代表同步实体 （学校、 节、 学生、 教师）。</span><span class="sxs-lookup"><span data-stu-id="13cc9-120">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="13cc9-121">**errorCode**</span><span class="sxs-lookup"><span data-stu-id="13cc9-121">**errorCode**</span></span> | <span data-ttu-id="13cc9-122">string</span><span class="sxs-lookup"><span data-stu-id="13cc9-122">string</span></span> |  <span data-ttu-id="13cc9-123">表示此错误的错误代码。</span><span class="sxs-lookup"><span data-stu-id="13cc9-123">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="13cc9-124">**errorMessage**</span><span class="sxs-lookup"><span data-stu-id="13cc9-124">**errorMessage**</span></span> | <span data-ttu-id="13cc9-125">string</span><span class="sxs-lookup"><span data-stu-id="13cc9-125">string</span></span> |  <span data-ttu-id="13cc9-126">包含错误的说明。</span><span class="sxs-lookup"><span data-stu-id="13cc9-126">Contains a description of the error.</span></span>        |
| <span data-ttu-id="13cc9-127">**joiningValue**</span><span class="sxs-lookup"><span data-stu-id="13cc9-127">**joiningValue**</span></span> | <span data-ttu-id="13cc9-128">string</span><span class="sxs-lookup"><span data-stu-id="13cc9-128">string</span></span> |  <span data-ttu-id="13cc9-129">条目的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="13cc9-129">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="13cc9-130">**recordedDateTime**</span><span class="sxs-lookup"><span data-stu-id="13cc9-130">**recordedDateTime**</span></span> | <span data-ttu-id="13cc9-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13cc9-131">DateTimeOffset</span></span> | <span data-ttu-id="13cc9-132">出现此错误的时间。</span><span class="sxs-lookup"><span data-stu-id="13cc9-132">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="13cc9-133">**reportableIdentifier**</span><span class="sxs-lookup"><span data-stu-id="13cc9-133">**reportableIdentifier**</span></span> | <span data-ttu-id="13cc9-134">string</span><span class="sxs-lookup"><span data-stu-id="13cc9-134">string</span></span> | <span data-ttu-id="13cc9-135">此错误条目的标识符。</span><span class="sxs-lookup"><span data-stu-id="13cc9-135">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="13cc9-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13cc9-136">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationError"
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
