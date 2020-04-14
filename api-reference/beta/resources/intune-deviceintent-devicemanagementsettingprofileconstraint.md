---
title: deviceManagementSettingProfileConstraint 资源类型
description: 强制实施给定配置文件元数据的约束
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b181760ea01b1fc46437ba67f295e50138ef12d3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420113"
---
# <a name="devicemanagementsettingprofileconstraint-resource-type"></a><span data-ttu-id="f5a09-103">deviceManagementSettingProfileConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="f5a09-103">deviceManagementSettingProfileConstraint resource type</span></span>

<span data-ttu-id="f5a09-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5a09-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5a09-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f5a09-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5a09-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f5a09-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5a09-107">强制实施给定配置文件元数据的约束</span><span class="sxs-lookup"><span data-stu-id="f5a09-107">Constraint enforcing a given profile metadata</span></span>


<span data-ttu-id="f5a09-108">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="f5a09-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f5a09-109">属性</span><span class="sxs-lookup"><span data-stu-id="f5a09-109">Properties</span></span>
|<span data-ttu-id="f5a09-110">属性</span><span class="sxs-lookup"><span data-stu-id="f5a09-110">Property</span></span>|<span data-ttu-id="f5a09-111">类型</span><span class="sxs-lookup"><span data-stu-id="f5a09-111">Type</span></span>|<span data-ttu-id="f5a09-112">说明</span><span class="sxs-lookup"><span data-stu-id="f5a09-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5a09-113">source</span><span class="sxs-lookup"><span data-stu-id="f5a09-113">source</span></span>|<span data-ttu-id="f5a09-114">String</span><span class="sxs-lookup"><span data-stu-id="f5a09-114">String</span></span>|<span data-ttu-id="f5a09-115">实体的来源</span><span class="sxs-lookup"><span data-stu-id="f5a09-115">The source of the entity</span></span>|
|<span data-ttu-id="f5a09-116">types</span><span class="sxs-lookup"><span data-stu-id="f5a09-116">types</span></span>|<span data-ttu-id="f5a09-117">String collection</span><span class="sxs-lookup"><span data-stu-id="f5a09-117">String collection</span></span>|<span data-ttu-id="f5a09-118">此实体所携带的类型的集合</span><span class="sxs-lookup"><span data-stu-id="f5a09-118">A collection of types this entity carries</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5a09-119">关系</span><span class="sxs-lookup"><span data-stu-id="f5a09-119">Relationships</span></span>
<span data-ttu-id="f5a09-120">无</span><span class="sxs-lookup"><span data-stu-id="f5a09-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5a09-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f5a09-121">JSON Representation</span></span>
<span data-ttu-id="f5a09-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5a09-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingProfileConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingProfileConstraint",
  "source": "String",
  "types": [
    "String"
  ]
}
```



