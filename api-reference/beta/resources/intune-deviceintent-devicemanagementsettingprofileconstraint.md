---
title: deviceManagementSettingProfileConstraint 资源类型
description: 强制实施给定配置文件元数据的约束
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fdd9e308f332d446ad9032736e5f08e8e3545d9e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955685"
---
# <a name="devicemanagementsettingprofileconstraint-resource-type"></a><span data-ttu-id="3dcc5-103">deviceManagementSettingProfileConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="3dcc5-103">deviceManagementSettingProfileConstraint resource type</span></span>

> <span data-ttu-id="3dcc5-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3dcc5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3dcc5-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3dcc5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3dcc5-106">强制实施给定配置文件元数据的约束</span><span class="sxs-lookup"><span data-stu-id="3dcc5-106">Constraint enforcing a given profile metadata</span></span>


<span data-ttu-id="3dcc5-107">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="3dcc5-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3dcc5-108">属性</span><span class="sxs-lookup"><span data-stu-id="3dcc5-108">Properties</span></span>
|<span data-ttu-id="3dcc5-109">属性</span><span class="sxs-lookup"><span data-stu-id="3dcc5-109">Property</span></span>|<span data-ttu-id="3dcc5-110">类型</span><span class="sxs-lookup"><span data-stu-id="3dcc5-110">Type</span></span>|<span data-ttu-id="3dcc5-111">说明</span><span class="sxs-lookup"><span data-stu-id="3dcc5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3dcc5-112">source</span><span class="sxs-lookup"><span data-stu-id="3dcc5-112">source</span></span>|<span data-ttu-id="3dcc5-113">字符串</span><span class="sxs-lookup"><span data-stu-id="3dcc5-113">String</span></span>|<span data-ttu-id="3dcc5-114">实体的来源</span><span class="sxs-lookup"><span data-stu-id="3dcc5-114">The source of the entity</span></span>|
|<span data-ttu-id="3dcc5-115">types</span><span class="sxs-lookup"><span data-stu-id="3dcc5-115">types</span></span>|<span data-ttu-id="3dcc5-116">String collection</span><span class="sxs-lookup"><span data-stu-id="3dcc5-116">String collection</span></span>|<span data-ttu-id="3dcc5-117">此实体所携带的类型的集合</span><span class="sxs-lookup"><span data-stu-id="3dcc5-117">A collection of types this entity carries</span></span>|

## <a name="relationships"></a><span data-ttu-id="3dcc5-118">关系</span><span class="sxs-lookup"><span data-stu-id="3dcc5-118">Relationships</span></span>
<span data-ttu-id="3dcc5-119">无</span><span class="sxs-lookup"><span data-stu-id="3dcc5-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3dcc5-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3dcc5-120">JSON Representation</span></span>
<span data-ttu-id="3dcc5-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3dcc5-121">Here is a JSON representation of the resource.</span></span>
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



