---
title: deviceManagementSettingProfileConstraint 资源类型
description: 强制实施给定配置文件元数据的约束
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2244b0fcafb1eb983388a220662c0ce7c874c73f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061159"
---
# <a name="devicemanagementsettingprofileconstraint-resource-type"></a><span data-ttu-id="7a2ed-103">deviceManagementSettingProfileConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="7a2ed-103">deviceManagementSettingProfileConstraint resource type</span></span>

<span data-ttu-id="7a2ed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a2ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a2ed-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7a2ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a2ed-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7a2ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a2ed-107">强制实施给定配置文件元数据的约束</span><span class="sxs-lookup"><span data-stu-id="7a2ed-107">Constraint enforcing a given profile metadata</span></span>


<span data-ttu-id="7a2ed-108">继承自 [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="7a2ed-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7a2ed-109">属性</span><span class="sxs-lookup"><span data-stu-id="7a2ed-109">Properties</span></span>
|<span data-ttu-id="7a2ed-110">属性</span><span class="sxs-lookup"><span data-stu-id="7a2ed-110">Property</span></span>|<span data-ttu-id="7a2ed-111">类型</span><span class="sxs-lookup"><span data-stu-id="7a2ed-111">Type</span></span>|<span data-ttu-id="7a2ed-112">说明</span><span class="sxs-lookup"><span data-stu-id="7a2ed-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a2ed-113">source</span><span class="sxs-lookup"><span data-stu-id="7a2ed-113">source</span></span>|<span data-ttu-id="7a2ed-114">String</span><span class="sxs-lookup"><span data-stu-id="7a2ed-114">String</span></span>|<span data-ttu-id="7a2ed-115">实体的来源</span><span class="sxs-lookup"><span data-stu-id="7a2ed-115">The source of the entity</span></span>|
|<span data-ttu-id="7a2ed-116">types</span><span class="sxs-lookup"><span data-stu-id="7a2ed-116">types</span></span>|<span data-ttu-id="7a2ed-117">String collection</span><span class="sxs-lookup"><span data-stu-id="7a2ed-117">String collection</span></span>|<span data-ttu-id="7a2ed-118">此实体所携带的类型的集合</span><span class="sxs-lookup"><span data-stu-id="7a2ed-118">A collection of types this entity carries</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a2ed-119">关系</span><span class="sxs-lookup"><span data-stu-id="7a2ed-119">Relationships</span></span>
<span data-ttu-id="7a2ed-120">无</span><span class="sxs-lookup"><span data-stu-id="7a2ed-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a2ed-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a2ed-121">JSON Representation</span></span>
<span data-ttu-id="7a2ed-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a2ed-122">Here is a JSON representation of the resource.</span></span>
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






