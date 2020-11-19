---
title: deviceManagementSettingEnrollmentTypeConstraint 资源类型
description: 强制实施应用于设置的注册类型的约束
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 604f9210cf81947617d40b0baec8fe8c5715347f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49307449"
---
# <a name="devicemanagementsettingenrollmenttypeconstraint-resource-type"></a><span data-ttu-id="54587-103">deviceManagementSettingEnrollmentTypeConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="54587-103">deviceManagementSettingEnrollmentTypeConstraint resource type</span></span>

<span data-ttu-id="54587-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54587-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54587-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="54587-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54587-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="54587-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54587-107">强制实施应用于设置的注册类型的约束</span><span class="sxs-lookup"><span data-stu-id="54587-107">Constraint that enforces the enrollment types applied to a setting</span></span>


<span data-ttu-id="54587-108">继承自 [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="54587-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="54587-109">属性</span><span class="sxs-lookup"><span data-stu-id="54587-109">Properties</span></span>
|<span data-ttu-id="54587-110">属性</span><span class="sxs-lookup"><span data-stu-id="54587-110">Property</span></span>|<span data-ttu-id="54587-111">类型</span><span class="sxs-lookup"><span data-stu-id="54587-111">Type</span></span>|<span data-ttu-id="54587-112">Description</span><span class="sxs-lookup"><span data-stu-id="54587-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54587-113">enrollmentTypes</span><span class="sxs-lookup"><span data-stu-id="54587-113">enrollmentTypes</span></span>|<span data-ttu-id="54587-114">String 集合</span><span class="sxs-lookup"><span data-stu-id="54587-114">String collection</span></span>|<span data-ttu-id="54587-115">注册类型列表</span><span class="sxs-lookup"><span data-stu-id="54587-115">List of enrollment types</span></span>|

## <a name="relationships"></a><span data-ttu-id="54587-116">关系</span><span class="sxs-lookup"><span data-stu-id="54587-116">Relationships</span></span>
<span data-ttu-id="54587-117">无</span><span class="sxs-lookup"><span data-stu-id="54587-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54587-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54587-118">JSON Representation</span></span>
<span data-ttu-id="54587-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54587-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingEnrollmentTypeConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingEnrollmentTypeConstraint",
  "enrollmentTypes": [
    "String"
  ]
}
```




