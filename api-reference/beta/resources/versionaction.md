---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: VersionAction
ms.openlocfilehash: f22761dd713b6d09d5e6fafb765d6d43bfc81bf9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043405"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="fb73e-102">VersionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb73e-102">VersionAction resource type</span></span>

> <span data-ttu-id="fb73e-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fb73e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb73e-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fb73e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fb73e-105">[**itemActivity**][activity] 上存在 **VersionAction** 资源指示活动导致要创建一个新版本。</span><span class="sxs-lookup"><span data-stu-id="fb73e-105">The presence of the **VersionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="fb73e-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb73e-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="fb73e-107">属性</span><span class="sxs-lookup"><span data-stu-id="fb73e-107">Properties</span></span>

| <span data-ttu-id="fb73e-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="fb73e-108">Property name</span></span> | <span data-ttu-id="fb73e-109">类型</span><span class="sxs-lookup"><span data-stu-id="fb73e-109">Type</span></span>   | <span data-ttu-id="fb73e-110">说明</span><span class="sxs-lookup"><span data-stu-id="fb73e-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="fb73e-111">newVersion</span><span class="sxs-lookup"><span data-stu-id="fb73e-111">newVersion</span></span>    | <span data-ttu-id="fb73e-112">string</span><span class="sxs-lookup"><span data-stu-id="fb73e-112">string</span></span> | <span data-ttu-id="fb73e-113">此操作创建的新版本的名称。</span><span class="sxs-lookup"><span data-stu-id="fb73e-113">The name of the new version that was created by this action.</span></span>

## <a name="remarks"></a><span data-ttu-id="fb73e-114">注解</span><span class="sxs-lookup"><span data-stu-id="fb73e-114">Remarks</span></span>

<span data-ttu-id="fb73e-115">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="fb73e-115">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction"
} -->
