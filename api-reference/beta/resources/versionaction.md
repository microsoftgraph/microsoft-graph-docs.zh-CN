---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: VersionAction
localization_priority: Normal
ms.openlocfilehash: c65b3cf021321a7e021c5fa4193abdcdce6c635a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520604"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="8b5cb-102">VersionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="8b5cb-102">VersionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b5cb-103">[**itemActivity**][activity] 上存在 **VersionAction** 资源指示活动导致要创建一个新版本。</span><span class="sxs-lookup"><span data-stu-id="8b5cb-103">The presence of the **VersionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="8b5cb-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8b5cb-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="8b5cb-105">属性</span><span class="sxs-lookup"><span data-stu-id="8b5cb-105">Properties</span></span>

| <span data-ttu-id="8b5cb-106">属性名称</span><span class="sxs-lookup"><span data-stu-id="8b5cb-106">Property name</span></span> | <span data-ttu-id="8b5cb-107">类型</span><span class="sxs-lookup"><span data-stu-id="8b5cb-107">Type</span></span>   | <span data-ttu-id="8b5cb-108">说明</span><span class="sxs-lookup"><span data-stu-id="8b5cb-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="8b5cb-109">newVersion</span><span class="sxs-lookup"><span data-stu-id="8b5cb-109">newVersion</span></span>    | <span data-ttu-id="8b5cb-110">string</span><span class="sxs-lookup"><span data-stu-id="8b5cb-110">string</span></span> | <span data-ttu-id="8b5cb-111">此操作创建的新版本的名称。</span><span class="sxs-lookup"><span data-stu-id="8b5cb-111">The name of the new version that was created by this action.</span></span>

## <a name="remarks"></a><span data-ttu-id="8b5cb-112">注解</span><span class="sxs-lookup"><span data-stu-id="8b5cb-112">Remarks</span></span>

<span data-ttu-id="8b5cb-113">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="8b5cb-113">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/versionaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
