---
title: deviceManagementSettingEnrollmentTypeConstraint 资源类型
description: 强制实施应用于设置的注册类型的约束
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5c5d34f381e7f4b52039551fb120e4691bc40026
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785328"
---
# <a name="devicemanagementsettingenrollmenttypeconstraint-resource-type"></a><span data-ttu-id="014b6-103">deviceManagementSettingEnrollmentTypeConstraint 资源类型</span><span class="sxs-lookup"><span data-stu-id="014b6-103">deviceManagementSettingEnrollmentTypeConstraint resource type</span></span>

> <span data-ttu-id="014b6-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="014b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="014b6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="014b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="014b6-106">强制实施应用于设置的注册类型的约束</span><span class="sxs-lookup"><span data-stu-id="014b6-106">Constraint that enforces the enrollment types applied to a setting</span></span>


<span data-ttu-id="014b6-107">继承自[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="014b6-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="014b6-108">属性</span><span class="sxs-lookup"><span data-stu-id="014b6-108">Properties</span></span>
|<span data-ttu-id="014b6-109">属性</span><span class="sxs-lookup"><span data-stu-id="014b6-109">Property</span></span>|<span data-ttu-id="014b6-110">类型</span><span class="sxs-lookup"><span data-stu-id="014b6-110">Type</span></span>|<span data-ttu-id="014b6-111">说明</span><span class="sxs-lookup"><span data-stu-id="014b6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="014b6-112">enrollmentTypes</span><span class="sxs-lookup"><span data-stu-id="014b6-112">enrollmentTypes</span></span>|<span data-ttu-id="014b6-113">String collection</span><span class="sxs-lookup"><span data-stu-id="014b6-113">String collection</span></span>|<span data-ttu-id="014b6-114">注册类型列表</span><span class="sxs-lookup"><span data-stu-id="014b6-114">List of enrollment types</span></span>|

## <a name="relationships"></a><span data-ttu-id="014b6-115">关系</span><span class="sxs-lookup"><span data-stu-id="014b6-115">Relationships</span></span>
<span data-ttu-id="014b6-116">无</span><span class="sxs-lookup"><span data-stu-id="014b6-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="014b6-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="014b6-117">JSON Representation</span></span>
<span data-ttu-id="014b6-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="014b6-118">Here is a JSON representation of the resource.</span></span>
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



