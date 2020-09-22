---
author: daspek
description: itemActivity 上存在 VersionAction 资源指示活动导致要创建一个新版本。
ms.date: 09/14/2017
title: VersionAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 0f16858c8b62f327019d2523488827fa6b20dced
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057739"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="90c3d-103">VersionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="90c3d-103">VersionAction resource type</span></span>

<span data-ttu-id="90c3d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90c3d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90c3d-105">[**itemActivity**][activity] 上存在 **VersionAction** 资源指示活动导致要创建一个新版本。</span><span class="sxs-lookup"><span data-stu-id="90c3d-105">The presence of the **VersionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="90c3d-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90c3d-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.versionAction"
}-->

```json
{
  "newVersion": "string"
}
```

## <a name="properties"></a><span data-ttu-id="90c3d-107">属性</span><span class="sxs-lookup"><span data-stu-id="90c3d-107">Properties</span></span>

| <span data-ttu-id="90c3d-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="90c3d-108">Property name</span></span> | <span data-ttu-id="90c3d-109">类型</span><span class="sxs-lookup"><span data-stu-id="90c3d-109">Type</span></span>   | <span data-ttu-id="90c3d-110">说明</span><span class="sxs-lookup"><span data-stu-id="90c3d-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="90c3d-111">newVersion</span><span class="sxs-lookup"><span data-stu-id="90c3d-111">newVersion</span></span>    | <span data-ttu-id="90c3d-112">string</span><span class="sxs-lookup"><span data-stu-id="90c3d-112">string</span></span> | <span data-ttu-id="90c3d-113">此操作创建的新版本的名称。</span><span class="sxs-lookup"><span data-stu-id="90c3d-113">The name of the new version that was created by this action.</span></span>

## <a name="remarks"></a><span data-ttu-id="90c3d-114">注解</span><span class="sxs-lookup"><span data-stu-id="90c3d-114">Remarks</span></span>

<span data-ttu-id="90c3d-115">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="90c3d-115">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction",
  "suppressions": []
}
-->


