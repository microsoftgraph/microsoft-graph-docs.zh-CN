---
title: informationProtectionContentLabel 资源类型
description: 介绍在对象上定义 MIP 元数据的信息ProtectionContentLabel 对象。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: b4d113e0f8f6d8f057a93d9094533e7fa2d5be6c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962600"
---
# <a name="informationprotectioncontentlabel-resource-type"></a><span data-ttu-id="a83e4-103">informationProtectionContentLabel 资源类型</span><span class="sxs-lookup"><span data-stu-id="a83e4-103">informationProtectionContentLabel resource type</span></span>

<span data-ttu-id="a83e4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a83e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a83e4-105">介绍在对象上定义 MIP 元数据的信息ProtectionContentLabel 对象。</span><span class="sxs-lookup"><span data-stu-id="a83e4-105">Describes the informationProtectionContentLabel object that defines MIP metadata on an object.</span></span> <span data-ttu-id="a83e4-106">**informationProtectionContentLabel** 由 [extractLabel](../api/informationprotectionlabel-extractLabel.md) API 解析为当前应用于文件的标签返回。</span><span class="sxs-lookup"><span data-stu-id="a83e4-106">**informationProtectionContentLabel** is returned by the [extractLabel](../api/informationprotectionlabel-extractLabel.md) API resolve to the label that is currently applied to a file.</span></span> 

## <a name="properties"></a><span data-ttu-id="a83e4-107">属性</span><span class="sxs-lookup"><span data-stu-id="a83e4-107">Properties</span></span>

| <span data-ttu-id="a83e4-108">属性</span><span class="sxs-lookup"><span data-stu-id="a83e4-108">Property</span></span>     | <span data-ttu-id="a83e4-109">类型</span><span class="sxs-lookup"><span data-stu-id="a83e4-109">Type</span></span>        | <span data-ttu-id="a83e4-110">说明</span><span class="sxs-lookup"><span data-stu-id="a83e4-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a83e4-111">assignmentMethod</span><span class="sxs-lookup"><span data-stu-id="a83e4-111">assignmentMethod</span></span>|<span data-ttu-id="a83e4-112">String</span><span class="sxs-lookup"><span data-stu-id="a83e4-112">String</span></span>| <span data-ttu-id="a83e4-113">可取值为：`standard`、`privileged`、`auto`。</span><span class="sxs-lookup"><span data-stu-id="a83e4-113">Possible values are: `standard`, `privileged`, `auto`.</span></span>|
|<span data-ttu-id="a83e4-114">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="a83e4-114">creationDateTime</span></span>|<span data-ttu-id="a83e4-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a83e4-115">DateTimeOffset</span></span>|<span data-ttu-id="a83e4-116">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="a83e4-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a83e4-117">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="a83e4-117">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="a83e4-118">label</span><span class="sxs-lookup"><span data-stu-id="a83e4-118">label</span></span>|[<span data-ttu-id="a83e4-119">labelDetails</span><span class="sxs-lookup"><span data-stu-id="a83e4-119">labelDetails</span></span>](labeldetails.md)| <span data-ttu-id="a83e4-120">有关当前应用于文件的标签的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a83e4-120">Details on the label that is currently applied to the file.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a83e4-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a83e4-121">JSON representation</span></span>

<span data-ttu-id="a83e4-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a83e4-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.informationProtectionContentLabel",
  "baseType": null
}-->

```json
{
  "assignmentMethod": "String",
  "creationDateTime": "String (timestamp)",
  "label": {"@odata.type": "microsoft.graph.labelDetails"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionContentLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

