---
title: deviceManagementSettingProfileConstraint 资源类型
description: 强制实施给定配置文件元数据的约束
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 917483556c71853856ff8b70973167b2c749a3a8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267962"
---
# <a name="devicemanagementsettingprofileconstraint-resource-type"></a><span data-ttu-id="b3bc0-103">deviceManagementSettingProfileConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3bc0-103">deviceManagementSettingProfileConstraint resource type</span></span>

<span data-ttu-id="b3bc0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3bc0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3bc0-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b3bc0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3bc0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b3bc0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3bc0-107">强制实施给定配置文件元数据的约束</span><span class="sxs-lookup"><span data-stu-id="b3bc0-107">Constraint enforcing a given profile metadata</span></span>


<span data-ttu-id="b3bc0-108">继承自 [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="b3bc0-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b3bc0-109">属性</span><span class="sxs-lookup"><span data-stu-id="b3bc0-109">Properties</span></span>
|<span data-ttu-id="b3bc0-110">属性</span><span class="sxs-lookup"><span data-stu-id="b3bc0-110">Property</span></span>|<span data-ttu-id="b3bc0-111">类型</span><span class="sxs-lookup"><span data-stu-id="b3bc0-111">Type</span></span>|<span data-ttu-id="b3bc0-112">说明</span><span class="sxs-lookup"><span data-stu-id="b3bc0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3bc0-113">source</span><span class="sxs-lookup"><span data-stu-id="b3bc0-113">source</span></span>|<span data-ttu-id="b3bc0-114">字符串</span><span class="sxs-lookup"><span data-stu-id="b3bc0-114">String</span></span>|<span data-ttu-id="b3bc0-115">实体的来源</span><span class="sxs-lookup"><span data-stu-id="b3bc0-115">The source of the entity</span></span>|
|<span data-ttu-id="b3bc0-116">types</span><span class="sxs-lookup"><span data-stu-id="b3bc0-116">types</span></span>|<span data-ttu-id="b3bc0-117">String collection</span><span class="sxs-lookup"><span data-stu-id="b3bc0-117">String collection</span></span>|<span data-ttu-id="b3bc0-118">此实体所携带的类型的集合</span><span class="sxs-lookup"><span data-stu-id="b3bc0-118">A collection of types this entity carries</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3bc0-119">关系</span><span class="sxs-lookup"><span data-stu-id="b3bc0-119">Relationships</span></span>
<span data-ttu-id="b3bc0-120">无</span><span class="sxs-lookup"><span data-stu-id="b3bc0-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3bc0-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3bc0-121">JSON Representation</span></span>
<span data-ttu-id="b3bc0-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3bc0-122">Here is a JSON representation of the resource.</span></span>
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




