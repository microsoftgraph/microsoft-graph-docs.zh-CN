---
author: daspek
title: versionAction 资源类型
description: VersionAction 对象提供有关导致新项版本的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f47d90c899ea9eb011837ae3c47dd6ec7ae22f30
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238986"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="82cc6-103">versionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="82cc6-103">versionAction resource type</span></span>

<span data-ttu-id="82cc6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82cc6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="82cc6-105">[**itemActivity**][activity]上 **存在 versionAction** 资源指示活动导致创建新版本。</span><span class="sxs-lookup"><span data-stu-id="82cc6-105">The presence of the **versionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

><span data-ttu-id="82cc6-106">**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="82cc6-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="82cc6-107">属性</span><span class="sxs-lookup"><span data-stu-id="82cc6-107">Properties</span></span>

| <span data-ttu-id="82cc6-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="82cc6-108">Property name</span></span> | <span data-ttu-id="82cc6-109">类型</span><span class="sxs-lookup"><span data-stu-id="82cc6-109">Type</span></span>   | <span data-ttu-id="82cc6-110">说明</span><span class="sxs-lookup"><span data-stu-id="82cc6-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="82cc6-111">newVersion</span><span class="sxs-lookup"><span data-stu-id="82cc6-111">newVersion</span></span>    | <span data-ttu-id="82cc6-112">string</span><span class="sxs-lookup"><span data-stu-id="82cc6-112">string</span></span> | <span data-ttu-id="82cc6-113">此操作创建的新版本的名称。</span><span class="sxs-lookup"><span data-stu-id="82cc6-113">The name of the new version that was created by this action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="82cc6-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82cc6-114">JSON representation</span></span>

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

