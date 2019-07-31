---
author: daspek
description: itemActivity 上存在 VersionAction 资源指示活动导致要创建一个新版本。
ms.date: 09/14/2017
title: VersionAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8eeec313ac4ed901d7552e2ad65d02edcaa821cd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007394"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="5a65b-103">VersionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="5a65b-103">VersionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a65b-104">[**itemActivity**][activity] 上存在 **VersionAction** 资源指示活动导致要创建一个新版本。</span><span class="sxs-lookup"><span data-stu-id="5a65b-104">The presence of the **VersionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="5a65b-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a65b-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="5a65b-106">属性</span><span class="sxs-lookup"><span data-stu-id="5a65b-106">Properties</span></span>

| <span data-ttu-id="5a65b-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="5a65b-107">Property name</span></span> | <span data-ttu-id="5a65b-108">类型</span><span class="sxs-lookup"><span data-stu-id="5a65b-108">Type</span></span>   | <span data-ttu-id="5a65b-109">说明</span><span class="sxs-lookup"><span data-stu-id="5a65b-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="5a65b-110">newVersion</span><span class="sxs-lookup"><span data-stu-id="5a65b-110">newVersion</span></span>    | <span data-ttu-id="5a65b-111">string</span><span class="sxs-lookup"><span data-stu-id="5a65b-111">string</span></span> | <span data-ttu-id="5a65b-112">此操作创建的新版本的名称。</span><span class="sxs-lookup"><span data-stu-id="5a65b-112">The name of the new version that was created by this action.</span></span>

## <a name="remarks"></a><span data-ttu-id="5a65b-113">注解</span><span class="sxs-lookup"><span data-stu-id="5a65b-113">Remarks</span></span>

<span data-ttu-id="5a65b-114">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="5a65b-114">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
