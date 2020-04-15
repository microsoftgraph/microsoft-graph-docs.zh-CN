---
title: resourceAction 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 899075a8ac494daf345fa6f8d91e3cc38126ec53
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441621"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="53bfa-103">resourceAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="53bfa-103">resourceAction resource type</span></span>

<span data-ttu-id="53bfa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53bfa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53bfa-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="53bfa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53bfa-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="53bfa-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="53bfa-107">属性</span><span class="sxs-lookup"><span data-stu-id="53bfa-107">Properties</span></span>
|<span data-ttu-id="53bfa-108">属性</span><span class="sxs-lookup"><span data-stu-id="53bfa-108">Property</span></span>|<span data-ttu-id="53bfa-109">类型</span><span class="sxs-lookup"><span data-stu-id="53bfa-109">Type</span></span>|<span data-ttu-id="53bfa-110">说明</span><span class="sxs-lookup"><span data-stu-id="53bfa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53bfa-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="53bfa-111">allowedResourceActions</span></span>|<span data-ttu-id="53bfa-112">String 集合</span><span class="sxs-lookup"><span data-stu-id="53bfa-112">String collection</span></span>|<span data-ttu-id="53bfa-113">允许的操作</span><span class="sxs-lookup"><span data-stu-id="53bfa-113">Allowed Actions</span></span>|
|<span data-ttu-id="53bfa-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="53bfa-114">notAllowedResourceActions</span></span>|<span data-ttu-id="53bfa-115">字符串集合</span><span class="sxs-lookup"><span data-stu-id="53bfa-115">String collection</span></span>|<span data-ttu-id="53bfa-116">不允许的操作</span><span class="sxs-lookup"><span data-stu-id="53bfa-116">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="53bfa-117">关系</span><span class="sxs-lookup"><span data-stu-id="53bfa-117">Relationships</span></span>
<span data-ttu-id="53bfa-118">无</span><span class="sxs-lookup"><span data-stu-id="53bfa-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53bfa-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53bfa-119">JSON Representation</span></span>
<span data-ttu-id="53bfa-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53bfa-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```







