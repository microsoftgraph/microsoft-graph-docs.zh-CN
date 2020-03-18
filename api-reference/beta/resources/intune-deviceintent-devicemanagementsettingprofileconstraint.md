---
title: deviceManagementSettingProfileConstraint 资源类型
description: 强制实施给定配置文件元数据的约束
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f4b565321069c27949fbd5814c4ddc1c4eb1451b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785300"
---
# <a name="devicemanagementsettingprofileconstraint-resource-type"></a><span data-ttu-id="6f3c8-103">deviceManagementSettingProfileConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="6f3c8-103">deviceManagementSettingProfileConstraint resource type</span></span>

> <span data-ttu-id="6f3c8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6f3c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f3c8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6f3c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f3c8-106">强制实施给定配置文件元数据的约束</span><span class="sxs-lookup"><span data-stu-id="6f3c8-106">Constraint enforcing a given profile metadata</span></span>


<span data-ttu-id="6f3c8-107">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="6f3c8-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6f3c8-108">属性</span><span class="sxs-lookup"><span data-stu-id="6f3c8-108">Properties</span></span>
|<span data-ttu-id="6f3c8-109">属性</span><span class="sxs-lookup"><span data-stu-id="6f3c8-109">Property</span></span>|<span data-ttu-id="6f3c8-110">类型</span><span class="sxs-lookup"><span data-stu-id="6f3c8-110">Type</span></span>|<span data-ttu-id="6f3c8-111">说明</span><span class="sxs-lookup"><span data-stu-id="6f3c8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f3c8-112">source</span><span class="sxs-lookup"><span data-stu-id="6f3c8-112">source</span></span>|<span data-ttu-id="6f3c8-113">String</span><span class="sxs-lookup"><span data-stu-id="6f3c8-113">String</span></span>|<span data-ttu-id="6f3c8-114">实体的来源</span><span class="sxs-lookup"><span data-stu-id="6f3c8-114">The source of the entity</span></span>|
|<span data-ttu-id="6f3c8-115">types</span><span class="sxs-lookup"><span data-stu-id="6f3c8-115">types</span></span>|<span data-ttu-id="6f3c8-116">String collection</span><span class="sxs-lookup"><span data-stu-id="6f3c8-116">String collection</span></span>|<span data-ttu-id="6f3c8-117">此实体所携带的类型的集合</span><span class="sxs-lookup"><span data-stu-id="6f3c8-117">A collection of types this entity carries</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f3c8-118">关系</span><span class="sxs-lookup"><span data-stu-id="6f3c8-118">Relationships</span></span>
<span data-ttu-id="6f3c8-119">无</span><span class="sxs-lookup"><span data-stu-id="6f3c8-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f3c8-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6f3c8-120">JSON Representation</span></span>
<span data-ttu-id="6f3c8-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f3c8-121">Here is a JSON representation of the resource.</span></span>
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



