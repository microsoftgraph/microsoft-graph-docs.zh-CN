---
title: informationProtectionContentLabel 资源类型
description: 介绍在对象上定义 MIP 元数据的 informationProtectionContentLabel 对象。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 454dd6dd3b095c01e476f52ae38d3a9caa552192
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496080"
---
# <a name="informationprotectioncontentlabel-resource-type"></a><span data-ttu-id="9414d-103">informationProtectionContentLabel 资源类型</span><span class="sxs-lookup"><span data-stu-id="9414d-103">informationProtectionContentLabel resource type</span></span>

<span data-ttu-id="9414d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9414d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9414d-105">介绍在对象上定义 MIP 元数据的 informationProtectionContentLabel 对象。</span><span class="sxs-lookup"><span data-stu-id="9414d-105">Describes the informationProtectionContentLabel object that defines MIP metadata on an object.</span></span> <span data-ttu-id="9414d-106">**informationProtectionContentLabel**由[extractLabel](../api/informationprotectionlabel-extractLabel.md) API 返回到当前应用于文件的标签。</span><span class="sxs-lookup"><span data-stu-id="9414d-106">**informationProtectionContentLabel** is returned by the [extractLabel](../api/informationprotectionlabel-extractLabel.md) API resolve to the label that is currently applied to a file.</span></span> 

## <a name="properties"></a><span data-ttu-id="9414d-107">属性</span><span class="sxs-lookup"><span data-stu-id="9414d-107">Properties</span></span>

| <span data-ttu-id="9414d-108">属性</span><span class="sxs-lookup"><span data-stu-id="9414d-108">Property</span></span>     | <span data-ttu-id="9414d-109">类型</span><span class="sxs-lookup"><span data-stu-id="9414d-109">Type</span></span>        | <span data-ttu-id="9414d-110">说明</span><span class="sxs-lookup"><span data-stu-id="9414d-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9414d-111">assignmentMethod</span><span class="sxs-lookup"><span data-stu-id="9414d-111">assignmentMethod</span></span>|<span data-ttu-id="9414d-112">String</span><span class="sxs-lookup"><span data-stu-id="9414d-112">String</span></span>| <span data-ttu-id="9414d-113">可取值为：`standard`、`privileged`、`auto`。</span><span class="sxs-lookup"><span data-stu-id="9414d-113">Possible values are: `standard`, `privileged`, `auto`.</span></span>|
|<span data-ttu-id="9414d-114">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="9414d-114">creationDateTime</span></span>|<span data-ttu-id="9414d-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9414d-115">DateTimeOffset</span></span>|<span data-ttu-id="9414d-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9414d-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9414d-118">label</span><span class="sxs-lookup"><span data-stu-id="9414d-118">label</span></span>|[<span data-ttu-id="9414d-119">labelDetails</span><span class="sxs-lookup"><span data-stu-id="9414d-119">labelDetails</span></span>](labeldetails.md)| <span data-ttu-id="9414d-120">当前应用于文件的标签上的详细信息。</span><span class="sxs-lookup"><span data-stu-id="9414d-120">Details on the label that is currently applied to the file.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9414d-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9414d-121">JSON representation</span></span>

<span data-ttu-id="9414d-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9414d-122">The following is a JSON representation of the resource.</span></span>

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